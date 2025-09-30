#include <stdio.h>

int main(void) {
  int escolha;
  char resposta;
  int pontuacao = 0;
  do{
  printf("\n1-Iniciar Quiz\n");
  printf("2-Ver Regras\n");
  printf("3-Sair\n");
  printf("Escolha a opção para o jogo: ");
  scanf("%d", &escolha);
  switch(escolha){
    case 1:
      printf("1. Qual é a principal função da placa-mãe?\n");
      printf("a) Processar gráficos e vídeos\n");
      printf("b) Interconectar todos os componentes\n");
      printf("c) Armazenar dados permanentemente\n");
      printf("Resposta: ");
      scanf(" %c", &resposta);
      if(resposta == 'b' || resposta == 'B') {
          printf("✅ Correto!\n");
        pontuacao=pontuacao+2;
      } else {
          printf("❌ Errado! A resposta correta é b)\n");
      }
    printf("2. O que significa a sigla 'URL'?\n");
    printf("a) Universal Resource Link\n");
    printf("b) Uniform Resource Locator\n");
    printf("c) Unified Reference Location\n");
    printf("Resposta: ");
    scanf(" %c", &resposta);
    if(resposta == 'b' || resposta == 'B') {
        printf("✅ Correto!\n");
      pontuacao=pontuacao+2;
    } else {
        printf("❌ Errado! A resposta correta é b)\n");
    } 
    printf("3. Qual dessas NÃO é uma linguagem de programação?\n");
    printf("a) Python\n");
    printf("b) HTML\n");
    printf("c) Java\n");
    printf("Resposta: ");
    scanf(" %c", &resposta);
    if(resposta == 'b' || resposta == 'B') {
        printf("✅ Correto!\n");
      pontuacao=pontuacao+2;
    } else {
        printf("❌ Errado! A resposta correta é b)\n");
    }
    printf("4. Para que serve um roteador em redes?\n");
    printf("a) Conectar dispositivos em uma rede local\n");
    printf("b) Encaminhar dados entre redes diferentes\n");
    printf("c) Amplificar o sinal Wi-Fi\n");
    printf("Resposta: ");
    scanf(" %c", &resposta);
    if(resposta == 'b' || resposta == 'B') {
        printf("✅ Correto!\n");
      pontuacao=pontuacao+2;
    } else {
        printf("❌ Errado! A resposta correta é b)\n");
    }
    printf("5. Qual a diferença principal entre HTTP e HTTPS?\n");
    printf("a) HTTP é mais rápido\n");
    printf("b) HTTPS criptografa a comunicação\n");
    printf("c) HTTP é para sites estáticos\n");
    printf("Resposta: ");
    scanf(" %c", &resposta);
    if(resposta == 'b' || resposta == 'B') {
      pontuacao=pontuacao+2;
        printf("✅ Correto!\n");
    } else {
        printf("❌ Errado! A resposta correta é b)\n");
    }
    printf("\nSua pontuação: %d", pontuacao);
    if(0<pontuacao && pontuacao<4){
    printf("\nPrecisa estudar mais\n");
    }else if(6<pontuacao && pontuacao<8){
    printf("\nMuito bom\n");
    }else if(pontuacao==10){
    printf("\nExcelente, parabens\n");
    }
    break;
    case 2:
    printf("O objetivo é responder corretamente ao maior número de perguntas para acumular pontos.\nLembre-se: quanto mais perto de 10 pontos, melhor! Como temos 5 perguntas, cada uma valendo 2 pontos, a pontuação máxima possível é 10.");
    break;
    case 3:
    printf("\nVocê saiu do jogo");
    break;
    default:
    printf("\nEscolha Incorreta"); //
    break;
  }
  }while(escolha!=3);
    return 0;
}
