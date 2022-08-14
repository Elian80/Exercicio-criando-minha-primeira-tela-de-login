# Exercicio-criando-minha-primeira-tela-de-login
##exercicio onde fiz minha primeira tela de login com linguagem python
import PySimpleGUI as sg
layout = [
    [sg.Text("Escreva seu nome de usuario")],
    [sg.InputText ("User")],
    [sg.Text(key = "Senha")],
    [sg.InputText("****")],
    [sg.Button("Entrar"), sg.Button("Cancelar")],
    [sg.Text("Esqueci minha senha")],
    [sg.Text("Bem Vindo!")]
]

janela = sg.Window("Login", layout)

while True:

    evento, valores = janela.read()


    if evento == sg.WIN_CLOSED or evento == "Cancelar":
        break
   
janela.close()
