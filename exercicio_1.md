/*Fazer um algoritmo que:
• Leia um numero indeterminado de linhas contendo cada uma a idade de um indivıduo.
• A ultima linha que nao entrara nos calculos, contem o valor da idade igual a zero.
• Calcule e escreva a idade media deste grupo de indivıduos.
*/

#include <iostream>
using namespace std;

int main()
{
    int idade = 1; //idade inicia com 1 para cair no while
    int i = 0; //declaração do contador
    float res, soma; 

  while(idade >= 1){ 
    cout << "Insira a idade do individuo o.o:" << endl;
    cin >> idade;

      soma += idade; //armazenando a soma das idades em "soma"

    if(idade != 0){
      i++; //contador vai somando +1 conforme o usuario insere as idades
    }
  }

    //fora do loop para exibição da media
    res = soma/i;
      cout << "A media da idade desses individuos é: " << res << endl;

  return 0;
}
