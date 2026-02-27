🖥️ Tela de Cadastro - Java Swing

Aplicação desktop desenvolvida em Java utilizando a biblioteca Swing, com interface gráfica criada no NetBeans GUI Builder.

O sistema simula um formulário de cadastro de usuário, coletando dados pessoais e exibindo as informações em uma caixa de diálogo ao clicar no botão Salvar.

📌 Funcionalidades

✅ Campo para Nome

✅ Campo para Idade (controlado também por um JSlider)

✅ Campo para CPF

✅ Campo para Cidade

✅ Campo para Bairro

✅ Campo para Estado

✅ Seleção de Gênero:

Masculino

Feminino

Outro

✅ Botão Salvar que exibe os dados com JOptionPane

✅ Interface com Nimbus Look and Feel

✅ Atualização dinâmica do valor da idade pelo JSlider

🎨 Interface do Sistema

Exemplo visual da aplicação:

4
🧠 Como Funciona
🔹 Classe Principal
public class Telinha extends javax.swing.JFrame

A classe Telinha herda de JFrame, criando uma janela principal para o sistema.

🔹 Botão SALVAR

Ao clicar no botão SALVAR, o método abaixo é executado:

private void JBSalvarActionPerformed(java.awt.event.ActionEvent evt)

Ele:

Captura os valores digitados nos campos.

Verifica qual gênero foi selecionado.

Exibe todas as informações usando:

JOptionPane.showMessageDialog()
🔹 Controle de Idade com Slider

O JSlider é configurado para:

Valor mínimo: 0

Valor máximo: 100

Atualizar automaticamente o jLabel8 com o valor selecionado

private void jSlider1StateChanged(javax.swing.event.ChangeEvent evt) {
    jLabel8.setText(String.valueOf(jSlider1.getValue()));
}
🚀 Como Executar
✅ Pré-requisitos

Java JDK 8 ou superior

IDE recomendada: NetBeans

▶️ Passos

Clone o repositório:

git clone https://github.com/seuusuario/seurepositorio.git

Abra o projeto no NetBeans.

Execute a classe Telinha.java.

Preencha os dados e clique em SALVAR.

🛠️ Tecnologias Utilizadas

Java

Swing (javax.swing)

NetBeans GUI Builder

📚 Estrutura do Projeto
telalogin/
 ├── Telinha.java
🔮 Melhorias Futuras

🔹 Implementar validação de CPF

🔹 Criar ButtonGroup para os RadioButtons

🔹 Implementar botão "Fechar"

🔹 Salvar dados em arquivo ou banco de dados

🔹 Melhorar layout e responsividade

👨‍💻 Autor

Felipe Menezes Welzbacher

Se você gostou do projeto, ⭐ deixe uma estrela no repositório!
