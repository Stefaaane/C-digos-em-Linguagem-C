# C-digos-em-Linguagem-C

#include <stdio.h>
#include <stdlib.h>

int main() { 

float  CandidatoA, CandidatoB, CandidatoC, CandidatoD, VotosValidos; 

	printf("\n\n\t\t\t\tELEICAO 2018\n\n\t\t");
	printf("\nInsira a quantidade de votos do candidato A: ");
	scanf("%f",&CandidatoA);
	CandidatoA++;
	printf("\nInsira a quantidade de votos do candidato B: ");
	scanf("%f",&CandidatoB);
	CandidatoB++;
	printf("\nInsira a quantidade de votos do candidato C: ");
	scanf("%f",&CandidatoC);
	CandidatoC++;
	printf("\nInsira a quantidade de votos do candidato D: ");
	scanf("%f",&CandidatoD);
	CandidatoD++;
	
	VotosValidos= CandidatoA+CandidatoB+CandidatoC+CandidatoD;
	
	float TotalNulo, TotalBranco;
	float TotalDeVotos;
	printf("\nInsira a quantidade de votos nulos: ");
	scanf("%f",&TotalNulo);
	printf("\nInsira a quantidade de votos em Branco: ");
	scanf("%f",&TotalBranco);
	
	TotalDeVotos= VotosValidos+ TotalNulo+ TotalBranco;
	
	float PercentualDeValidos;
	PercentualDeValidos=(VotosValidos*100)/TotalDeVotos;
	printf("\nPercentual de Votos VALIDOS: %.2f%%\n", PercentualDeValidos);
	
	system("cls");
	printf("\n\t\t\t\tAPURACAO DOS VOTOS\n");
	float PercentualCandidatoA, PercentualCandidatoB, PercentualCandidatoC, PercentualCandidatoD,PercentualNulo,PercentualBranco;
	PercentualCandidatoA= (CandidatoA*100)/TotalDeVotos;
	PercentualCandidatoB=(CandidatoB*100)/TotalDeVotos;
	PercentualCandidatoC=(CandidatoC*100)/TotalDeVotos;
	PercentualCandidatoD=(CandidatoD*100)/TotalDeVotos;
	PercentualNulo=(TotalNulo*100)/TotalDeVotos;
	PercentualBranco=(TotalBranco*100)/TotalDeVotos;
	
	
	printf("\nPercentual de Votos do Candidato A: %.2f%%",PercentualCandidatoA);
	printf("\nPercentual de Votos do Candidato B: %.2f%%",PercentualCandidatoB);
	printf("\nPercentual de Votos do Candidato C: %.2f%%",PercentualCandidatoC);
	printf("\nPercentual de Votos do Candidato D: %.2f%%",PercentualCandidatoD);
	printf("\nPercentual de Votos em Brancos: %.2f%%",	  PercentualBranco);
	printf("\nPercentual de Votos Nulos: %.2f%%",	      PercentualNulo);
	
	int CandidatoVencedor=0;
	char Vencedor;
	
	if (CandidatoA> CandidatoVencedor){
		CandidatoVencedor= CandidatoA;
		Vencedor= 'A';							  
	 }
	if (CandidatoB> CandidatoVencedor){
		CandidatoVencedor= CandidatoB;
		Vencedor= 'B';		
	 }
	 if (CandidatoC> CandidatoVencedor){
		CandidatoVencedor= CandidatoC;
		Vencedor= 'C';
	 }
	 if (CandidatoD> CandidatoVencedor){
		CandidatoVencedor= CandidatoD;
		Vencedor= 'D';
     }
     
     printf("\n\t\t\t\tRESULTADO\t\n");
     printf("\nO candidato vencedor foi o: %c\n",Vencedor);
     
    
	
	
	return 0;
}
	 							

