# Gravador_tela

## Gravador de tela em python utilizando as bibliotecas (cv2, numpy e pyautogui).

### Esse código é um exemplo de como gravar a tela do computador em Python usando os módulos cv2, numpy e pyautogui. O código faz o seguinte:

+ Define o tamanho da tela em pixels como uma tupla (1920, 1080)
+ Define o codec de vídeo como ‘mp4v’, que é um formato compatível com o OpenCV e o FFMPEG
+ Cria um objeto cv2.VideoWriter chamado ‘out’ que vai gravar o vídeo no arquivo ‘gravacao.avi’ com o codec ‘mp4v’, a taxa de quadros de 20.0 e o tamanho da tela
+ Entra em um loop infinito que faz o seguinte:
+ Captura uma imagem da tela usando a função pyautogui.screenshot()
+ Converte a imagem em um array numpy usando a função np.array()
+ Converte a imagem de RGB para BGR usando a função cv2.cvtColor()
+ Escreve a imagem no objeto ‘out’ usando a função out.write()
+ Espera por uma tecla ser pressionada usando a função cv2.waitKey()
+ Se a tecla for ‘q’, sai do loop e encerra o programa
+ Libera os recursos usados pelo objeto ‘out’ usando a função out.release()
+ Fecha todas as janelas do OpenCV usando a função cv2.destroyAllWindows()

