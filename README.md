![alt tag](https://raw.githubusercontent.com/aweiand/facostex/master/figuras/logo-facos.png)

# O que é?

O **facosTex** é um projeto baseado no [abnTeX2] desenvolvido para auxiliar os alunos da Faculdade Cenecista de Osório - CNEC/Facos em seus trabalhos de monografias de graduação.
Espera-se que o projeto seja um modelo de trabalho acadêmico que implemente todas as exigências das normas da ABNT sem a necessidade de se preocupar com o estilo ou formatação do documento.

### Modelos Disponíveis

**Trabalhos Acadêmicos**

 - Trabalho de Conclusão de Curso de Graduação
 - Trabalho de Conclusão de Curso de Especialização

# Por onde começo?
Para utilizar o facosTeX você precisa seguir os seguintes passos:

1. Clique [aqui](https://github.com/aweiand/facostex/archive/master.zip) para baixar o projeto
2. Descompacte o arquivo no diretório onde você deseja guardar os arquivos do seu trabalho
3. Crie o seu texto a partir do arquivo *documento.tex* distribuído no arquivo baixado. O arquivo possui comentários e é, em certa medida, auto-explicativo.

> Você é iniciante em LaTeX ou em abnTeX2? Clique [aqui](https://code.google.com/p/abntex2/wiki/PorOndeComecar) para acessar a página desenvolvida pela equipe do abnTeX2. Nesta página é possível acessar diversos links sobre o LaTeX e sobre o abnTeX2 como, por exemplo, a história do LaTeX e alguns minicursos desenvolvidos em outras universidades

# Como compilar?

Uma vez que todas as informações foram colocadas no documento, você precisará de um programa para compilar e gerar o PDF do seu trabalho.

### Windows
 - Acesse [https://github.com/aweiand/facostex/wiki/Como-instalar-no-Windows] 
 
### Linux

 - Acesse [https://github.com/aweiand/facostex/wiki/Como-instalar-no-Linux] 
 
# Limitações
 
 O modelo atual possui algumas limitações que podem ser corrigidas ou implementadas em alguma versão futura. São elas:
 
  - O modelo permite a participação de somente um co-orientador
  
# Dicas
Veja a seguir como inserir alguns elementos no seu texto.

### Como inserir uma Tabela
```tex
\begin{table}[htb]
    \centering
    \caption{\label{tab:tabela-exemplo2}Tabela Exemplo 2}
    \begin{tabular}{lc}
        \textbf{Coluna 1} & \textbf{Coluna 2} \\
        Linha 1 Coluna 1  & Linha 1 Coluna 1  \\
        Linha 2 Coluna 1  & Linha 2 Coluna 2 
    \end{tabular}
\end{table}
```

### Como inserir uma figura
```tex
\begin{figure}[htb]
    \centering\includegraphics[width=.80\textwidth]{figuras/figura-1.jpg}
    \caption{\label{fig:exemplo-18}Exemplo.}
    
    Fonte: Exemplo%
\end{figure}
```

### Como inserir uma alínea
```tex
\begin{alineas}
	\item Lorem ipsum dolor sit amet;
    \item Praesent vitae nulla varius;
	\item Praesent quis erat eleifend;
	\item Mauris facilisis odio eu:
	\begin{subalineas}
		\item Integer non lacinia magna;
		\item Proin mattis placerat risus.
	\end{subalineas}
\end{alineas}
```

### Como criar Capítulos
```tex
\chapter{Fundamentação Teórica}
\label{cap:fundamentacao-teorica}
```

### Como criar Seções
```tex
% Seções Secundárias
\section{Objetivo Geral 2}
\label{sec:objetivo-geral-2}

% Seções Terciárias
\subsection{Objetivo Geral 3}
\label{sec:objetivo-geral-3}

% Seções Quaternárias
\subsubsection{Objetivo Geral 4}
\label{sec:objetivo-geral-4}

% Seções Quinárias
\subsubsubsection{Objetivo Geral 5}
\label{sec:objetivo-geral-5}
```

### Como inserir um algoritmo
```tex
\begin{algorithm}[h!]
	\SetSpacedAlgorithm
	\caption{\label{alg:algoritmo_de_colonica_de_formigas}Algoritmo de Otimização por Colônia de Formiga}
	\Entrada{Entrada do Algoritmo}
	\Saida{Saida do Algoritmo}
	\Inicio{
		Atribua os valores dos parâmetros\;
		Inicialize as trilhas de feromônios\;
		\Enqto{não atingir o critério de parada}{
			\Para{cada formiga}{
				Construa as Soluções\;
			}
			Aplique Busca Local (Opcional)\;
			Atualize o Feromônio\;
		}	
	}
\end{algorithm}
```

# Atenção

O facosTeX é fornecido gratuitamente e sem garantias e pode ser redistribuído livremente para fins acadêmicos. O facosTex é um produto extra-oficial e não está oficialmente vinculada à Faculdade Cenecista de Osório.


[Por Onde Comecar]:https://code.google.com/p/abntex2/wiki/PorOndeComecar
[http://www.goes.uece.br]:http://www.goes.uece.br
[abnTeX2]:https://code.google.com/p/abntex2/
[http://miktex.org/download]:http://miktex.org/download
[http://texstudio.sourceforge.net/]:http://texstudio.sourceforge.net/
