# AHoraDaMorte
Esse programa foi um projeto para a disciplina de Física Computacional, utilizando a linguagem Scilab, para calcular a quanto tempo o corpo está morto depois de ter sido encontrado.
//SEMINARIO FISÍCA COMPUTACIONAL
//LEI DO RESFRIAMENTO DE NEWTON 

clear;
disp("Programa A Hora da Morte")

p=input("Digite a Temperatura inicial do corpo encontrado(°C): ")
T0=p;

a=input("Qual a hora que foi encontrado o corpo: ")
to=a;

r=input("Digite a Temperatura do ambiente (°C) : ")
Ta=r;

c=input("Uma hora após achar o corpo, qual a atual Temperatura deste(°C) : ")
Tc=c;

k=-log((Tc-Ta)/(T0-Ta))*(1/60);//constante k
tv=-log((36.5-Ta)/(T0-Ta))*(1/k);//tempo quando o corpo estava vivo em min
tf=to+(tv/60);//tempo em horas
t0=0;
t=[0:1:300];

function y=F(t,T);
    y=-k*(T-Ta)
endfunction

T=ode(T0,t0,t,F);
