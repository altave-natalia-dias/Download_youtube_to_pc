from pytube import YouTube

def baixar_video(url):
    try:
        # Cria uma instância do objeto YouTube com a URL do vídeo
        video = YouTube(url)
        
        # Seleciona a melhor resolução disponível
        stream = video.streams.get_highest_resolution()
        
        # Baixa o vídeo
        stream.download()
        
        print("Download concluído!")
    except Exception as e:
        print(f"Ocorreu um erro durante o download: {str(e)}")

# Insira a URL do vídeo que você deseja baixar
url_video = input("Insira a URL do vídeo do YouTube: ")
baixar_video(url_video)
