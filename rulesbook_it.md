\documentclass[a4paper, 12pt, oneside]{article}
%packages%
\PassOptionsToPackage{hyphens}{url}
\usepackage{hyperref}
\usepackage[utf8]{inputenc}
\usepackage{natbib}
\usepackage{graphicx}
\usepackage{amsmath}
\usepackage{amssymb}
\usepackage{amsthm}
\usepackage{physics}
\usepackage{caption}
\usepackage{titlesec}
\usepackage[a4paper, total={6.5in, 9in}]{geometry}
\usepackage{wrapfig}
\usepackage{listings}
\usepackage{xcolor}
\usepackage{verbatim}
\usepackage{hyperref}
\usepackage{subcaption}
\usepackage{float}
\usepackage{fancyhdr}
\usepackage{subfiles}
\usepackage{cancel}
\usepackage{comment}
\usepackage{titlesec}
\usepackage{blindtext}
\usepackage{color}
\usepackage[T1]{fontenc}
\usepackage{epigraph}
\usepackage{mathrsfs}
\usepackage{relsize}
\usepackage{yfonts}
\usepackage[italian]{babel}
\usepackage{afterpage}
\usepackage{tikz}
%hyperref settings%
\hypersetup{
    colorlinks=true,
    linkcolor=black,
    filecolor=magenta,      
    urlcolor=cyan,
    pdftitle={Overleaf Example},
    pdfpagemode=FullScreen,
    }

\urlstyle{same}

%subfile settings%
\graphicspath{{IMG/}}

%page style%
\pagestyle{fancy}
\fancyhf{}
\rhead{\thepage}
\renewcommand{\headrulewidth}{1.5pt}
%\renewcommand{\figurename}{Figura}
%\renewcommand{\tablename}{Tabella} %non necessario dal momento che si cambia il dizionario
\definecolor{gray75}{gray}{0.75}
\newcommand{\hsp}{\hspace{20pt}}
\titleformat{\chapter}[hang]{\Huge\bfseries}{\thechapter\hsp\textcolor{gray75}{|}\hsp}{0pt}{\Huge\bfseries}

%caption style
\captionsetup[figure]{margin=25pt,labelfont=bf, font=small}
\captionsetup[table]{labelfont=bf, font=small}

%math style%
\renewcommand\qedsymbol{$\blacksquare$}
\numberwithin{equation}{section}
\mathcode`\*="8000
{\catcode`\*\active\gdef*{\cdot}}
\renewcommand{\CancelColor}{\color{red}}
\newcommand{\pbracket}[3]{\sum_{#3}\bigg(\pdv{#1}{q_{#3}}\pdv{#2}{p_{#3}} - \pdv{#1}{p_{#3}}\pdv{#2}{q_{#3}}\bigg)}
\newcommand{\uv}[1]{\vb{\hat{#1}}}
\renewcommand{\i}{\text{i}}
\newcommand{\field}[1]{\vb*{\mathcal{#1}}}

%code style%
\definecolor{codegreen}{rgb}{0,0.6,0}
\definecolor{codegray}{rgb}{0.5,0.5,0.5}
\definecolor{codepurple}{rgb}{0.58,0,0.82}
\definecolor{backcolour}{rgb}{0.95,0.95,0.92}

\lstdefinestyle{matlab}{
    backgroundcolor=\color{backcolour},   
    commentstyle=\color{codegreen},
    keywordstyle=\color{magenta},
    numberstyle=\tiny\color{codegray},
    stringstyle=\color{codepurple},
    basicstyle=\ttfamily\footnotesize,
    breakatwhitespace=false,         
    breaklines=true,                 
    captionpos=b,                    
    keepspaces=true,                 
    numbers=left,                    
    numbersep=5pt,                  
    showspaces=false,                
    showstringspaces=false,
    showtabs=false,                  
    tabsize=2
}
\lstset{style=matlab}


\fancyhf{} % Cancella le intestazioni e i piè di pagina predefiniti

% Intestazione con nome del capitolo allineato a destra sulle pagine dispari e a sinistra sulle pagine pari
\fancyhead[RO]{\textit{\nouppercase{\leftmark}}} % Intestazione a destra su pagine dispari
\fancyhead[LE]{\textit{\nuppercase{\leftmark}}} % Intestazione a sinistra su pagine pari

% Piè di pagina con numero di pagina centrato e linea sopra il numero
\fancyfoot[C]{\thepage}
\renewcommand{\footrulewidth}{0.4pt} % Aggiunge una linea sopra il numero di pagina



\begin{document}

%set a counter
\newcounter{articlecnt}
\setcounter{articlecnt}{1} %usare la combinazione \thearticlecnt per visualizzare il valore attuale e con \stepcounter{articleccnt} per far progredire tale valore

\begin{titlepage}
    \begin{center}
         \large
         \hfill \today
         \vspace{1 cm}
         \\
             \includegraphics[scale=0.8]{semito-v_logo.png} 
         \vspace*{1cm}
         \normalsize
      \\         
        \fontsize{18}{18}\selectfont
       \textbf{Regolamento SemiTO-V\\}
\fontsize{13}{13}\selectfont
\vspace{0.7 cm}
{Author:  Vincenzo Butera\\ }
{Contributors:  Tan Siret Akıncı, Maurizio Contu\\ }
\vspace{0.7 cm}


\vspace{0.7 cm}
Obiettivo:
Sviluppo di un regolamento interno per SemiTO-V, il team studentesco per sviluppare processori basati sull'architettura RISC-V, volto a garantire la crescita ordinata, solida e sostenibile del team.
Il focus sarà centrato sulla definizione di ruoli, regole operative e strutture organizzative, con particolare attenzione all'equilibrio tra creatività tecnica (HW e SW) e stabilità amministrativa (PR).

Il regolamento mira a favorire il buon funzionamento interno, promuovere responsabilità condivise, prevenire conflitti inutili e facilitare il passaggio generazionale.
Sarà uno strumento vivo: chiaro, essenziale, ma capace di evolvere nel tempo insieme al gruppo.

Il fine ultimo è rendere SemiTO-V autonomo e resiliente, capace di auto-organizzarsi, di attrarre nuovi membri e di mantenere relazioni di fiducia durature con partner, sponsor e istituzioni. Viva il RISC-V, Viva l'Open Source, Viva la Scienza e Viva i Giovani di buone intenzioni!
 \vspace{0.9 cm}
        
        \vspace{0.5 cm}
       \includegraphics[scale=1.5]{Logo_PoliTo_dal_2021_blu.png} 
       
   \end{center}
   \newcommand\blankpage{%
    \null
    \thispagestyle{empty}%
    \addtocounter{page}{-1}%
    \newpage}
\afterpage{\blankpage}
\end{titlepage}
\selectlanguage{italian}
\tableofcontents
\newpage

\section{Disposizioni generali}

   \subsection*{Articolo \thearticlecnt: Valori Fondamentali}
   \addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Valori Fondamentali}
   \stepcounter{articlecnt}

SemiTO-V si fonda su un insieme di valori condivisi, considerati imprescindibili per garantire un ambiente di lavoro sano, creativo e durevole. Ogni membro del team si impegna a rispettare questi principi:

\begin{itemize}
    \item \textbf{Responsabilità personale}: Ogni membro è responsabile del proprio operato e del rispetto degli impegni assunti verso il team e verso i progetti in corso.
    
    \item \textbf{Collaborazione}: La condivisione delle conoscenze, l'aiuto reciproco e il lavoro di squadra sono posti al centro dell’attività quotidiana.
    
    \item \textbf{Merito e impegno}: Il riconoscimento interno si basa sulla qualità e sulla costanza dei contributi, indipendentemente dall'anzianità, dal ruolo o da altri fattori estranei al merito.
    
    \item \textbf{Apertura mentale e rispetto reciproco}: SemiTO-V valorizza ogni contributo basandosi esclusivamente su motivazione, capacità e spirito di collaborazione, senza alcun interesse per caratteristiche personali o appartenenze di altra natura.
    
    \item \textbf{Resilienza e miglioramento continuo}: Gli errori sono considerati parte integrante del percorso di crescita. Ogni difficoltà è affrontata come occasione di apprendimento e sviluppo.
    
    \item \textbf{Etica e trasparenza}: Le attività del team sono condotte con integrità, correttezza, e totale rispetto delle persone, delle risorse utilizzate e delle norme condivise. Le attivita del team è tutto trasparente sia con i membri deal team che con il mondo.

    \item \textbf{Approccio Open Source}: SemiTO-V si impegna a sviluppare tecnologie, hardware e software orientati all'open source, contribuendo alla diffusione della conoscenza libera e favorendo l'accesso pubblico ai risultati del proprio lavoro. La condivisione responsabile dei progetti è considerata parte integrante della missione del team.
    
\end{itemize}

Il rispetto di questi valori costituisce la base per la partecipazione attiva e la continuità all'interno di SemiTO-V e ogni nuovo membro si impegna a far suoi e difendere questi valori.

     \subsection*{Articolo \thearticlecnt: Modalità di ingresso e onboarding}
     \addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Modalità di ingresso e onboarding}
     \stepcounter{articlecnt}

L'ingresso in SemiTO-V è regolato da un processo di selezione e inserimento progressivo, volto a garantire la qualità delle attività e a favorire l'integrazione responsabile dei nuovi membri.

\begin{itemize}
    \item \textbf{Selezione}: La candidatura di un nuovo membro viene valutata dai membri attivi dell'area di interesse (\textit{Hardware and Logic Dev}, \textit{Software and Instruction Dev} e/o \textit{Public Relations}). La selezione si basa sulla motivazione, sulla disponibilità effettiva a contribuire e sul potenziale di crescita.
    
    \item \textbf{Periodo di onboarding}: I nuovi membri accettati preliminarmente vengono inseriti in un periodo di onboarding della durata di un progetto o di 1 mese, durante il quale sono affiancati a un membro esperto dell'area.
    
    \item \textbf{Valutazione finale}: Al termine dell'onboarding, i membri dell'area interessata valutano l'integrazione definitiva del candidato, basandosi su criteri di partecipazione attiva, affidabilità, capacità di lavorare in gruppo e qualità dei contributi espressi.
    
    \item \textbf{Autonomia progressiva}: Durante l'onboarding, ai nuovi membri vengono assegnati compiti di difficoltà crescente, per permettere una valutazione realistica delle competenze e dell'impegno.
    
    \item \textbf{Esclusione}: Qualora un nuovo membro si dimostri inattivo, inaffidabile o incompatibile con i valori di SemiTO-V, l'area di appartenenza può decidere di interrompere il processo di integrazione.
\end{itemize}

Il processo di ingresso è finalizzato a costruire una squadra solida, coesa e orientata ai risultati, senza rinunciare all'accoglienza e all'investimento sui nuovi talenti.

     
     \subsection*{Articolo \thearticlecnt: Gestione delle divergenze}
     \addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Gestione delle divergenze}
     \stepcounter{articlecnt}

In un ambiente dinamico e creativo come SemiTO-V, il confronto di idee è naturale e positivo. Tuttavia, quando le divergenze rischiano di compromettere il clima o l'operatività del team, è importante gestirle in modo costruttivo.

\begin{itemize}
    \item \textbf{Responsabilità personale}: Ogni membro è incoraggiato a risolvere eventuali incomprensioni o contrasti attraverso un confronto diretto, rispettoso e privato con le persone coinvolte.
    
    \item \textbf{Facilitazione}: Se il conflitto persiste o coinvolge il lavoro comune, può essere richiesto l'intervento di un facilitatore, individuato tra i capiprogetto o i responsabili di area, con il solo compito di favorire il dialogo e il chiarimento reciproco.
    
    \item \textbf{Ruolo del facilitatore}: Il facilitatore non ha potere decisionale o disciplinare, ma agisce per aiutare le parti a ritrovare un terreno comune di collaborazione.
    
    \item \textbf{Tutela del team}: Se il conflitto dovesse continuare a compromettere il lavoro collettivo nonostante i tentativi di mediazione, può essere valutata, in via eccezionale, una riassegnazione di compiti, una diversa organizzazione interna, o una sospensione delle parti coinvolte fino a che non si giunga a risoluzione, sempre nell'ottica di preservare i progetti, i valori principali della liberta di hardware e software (Philosophy of the GNU Project), e il benessere del gruppo.
\end{itemize}

La capacità di affrontare e superare le divergenze con maturità e rispetto reciproco è considerata parte integrante dell’essere membri di SemiTO-V.

\subsection*{Articolo \thearticlecnt: Struttura dei Ruoli e Gerarchia Funzionale}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Struttura dei Ruoli e Gerarchia Funzionale}
\stepcounter{articlecnt}

SemiTO-V adotta una struttura organizzativa leggera ma funzionale, finalizzata a garantire chiarezza, efficienza e continuità operativa, senza compromettere l'orizzontalità e la libertà creativa dei membri.

\begin{figure}
    \centering
    \includegraphics[width=0.9\linewidth]{semitofive_hierarchy.png}
    \caption{La gerarchia semplificata del team}
    \label{fig:enter-label}
\end{figure}

\begin{itemize}
    \item \textbf{Aree operative}: Il team è suddiviso in tre aree principali: \textit{Hardware and Logic Dev (HW)}, \textit{Software and Instruction Dev (SW)} e \textit{Public Relations (PR)}, ognuna delle quali gestisce autonomamente i propri progetti e attività.
    
    \item \textbf{Ruoli di responsabilità}: Ogni area nomina i propri responsabili attraverso modalità interne (elezione o designazione). I responsabili hanno il compito di coordinare, facilitare il lavoro collettivo e rappresentare l'area nelle decisioni intersettoriali. 
    
    \item \textbf{Rotazione dei ruoli}: I ruoli di capo progetto nelle aree HW e SW hanno durata limitata (fino al completamento del progetto). I ruoli nell'area PR hanno durata più estesa (semestrale o annuale) per garantire continuità amministrativa.
    
    \item \textbf{Coordinamento generale}: I responsabili delle aree si incontrano periodicamente per assicurare l'allineamento strategico e operativo del team. Nessuna area è gerarchicamente superiore alle altre: la leadership è diffusa e collaborativa.

    \item \textbf{Codici Interni di Area}

Ogni area operativa di SemiTO-V (\textit{Hardware and Logic Dev}, \textit{Software and Instruction Dev}, \textit{Public Relations}) ha un proprio codice interno.  
Il codice interno ha lo scopo di disciplinare nel dettaglio l'organizzazione quotidiana dei lavori, facilitare il passaggio delle conoscenze tra i membri e garantire continuità anche nel cambio dei responsabili.

Il codice interno può includere, a titolo esemplificativo e non esaustivo:
\begin{itemize}
    \item \textbf{Metodi di lavoro}: descrizione delle pratiche operative standard (es. gestione delle repository, modalità di code review, procedure di documentazione tecnica, pipeline di rilascio ecc).
    
    \item \textbf{Procedure operative}: definizione di processi ricorrenti per task critici (es. gestione versioni, protocolli di test hardware, modalità di iscrizione a competizioni, gestione della comunicazione istituzionale).
    
    \item \textbf{Check list operative}: costruzione di elenchi di controllo da utilizzare per attività ricorrenti (es. checklist di rilascio di un progetto SW, checklist di audit di sicurezza HW, checklist di organizzazione e gestione del reparto PR).
    
    \item \textbf{Strumenti operativi}: indicazione degli strumenti adottati ufficialmente dall'area (es. sistemi di project management, piattaforme di versionamento, tool di documentazione, format di rendicontazione spese).
    
    \item \textbf{Criteri di elezione o nomina}: modalità interne di selezione dei capiprogetto e dei responsabili di area, inclusi criteri di rotazione, durata e modalità di revoca o sostituzione.
\end{itemize}

Il codice interno di ogni area deve essere coerente con i valori fondamentali e con il presente regolamento generale.  
Può essere aggiornato dall'area di appartenenza, previa consultazione e approvazione da parte dei membri attivi dell'area stessa. Maggiori dettagli sono disponibili nell'articolo 5 di questo documento.

La redazione accurata e l'aggiornamento costante dei codici interni è considerata parte integrante della professionalità e della maturità operativa del team.


\end{itemize}

La struttura dei ruoli esiste per favorire l'efficacia del lavoro e la crescita di ogni membro, non per creare gerarchie di status.

\subsection*{Articolo \thearticlecnt: Modifica del Regolamento}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Modifica del Regolamento}
\stepcounter{articlecnt}

Il regolamento di SemiTO-V è concepito come uno strumento vivo: deve garantire stabilità e coerenza, ma anche adattarsi all'evoluzione naturale del team e delle sue attività.

\begin{itemize}
    \item \textbf{Proposte di modifica}: Ogni membro attivo del team ha diritto di proporre modifiche o integrazioni al presente regolamento. Le proposte devono essere presentate in forma scritta e condivisa (documento breve, email o messaggio privato) ai responsabili di area o al coordinamento generale.
    
    \item \textbf{Discussione e confronto}: Le proposte vengono discusse in riunione plenaria aperta a tutti i membri attivi. È incoraggiata la massima chiarezza nel presentare le motivazioni e gli effetti attesi delle modifiche.
    
    \item \textbf{Approvazione}: Per l'approvazione definitiva di una modifica è richiesta una maggioranza qualificata pari ad almeno i due terzi (2/3) dei membri attivi presenti alla votazione. Le votazioni possono essere condotte in presenza o su piattaforme digitali ufficiali del team.
    
    \item \textbf{Entrata in vigore}: Una volta approvata, la modifica entra immediatamente in vigore, salvo diversa specificazione contenuta nella proposta stessa.
    
    \item \textbf{Limitazioni}: Nessuna modifica può annullare o contraddire i valori fondamentali espressi nel presente regolamento, pena la nullità automatica della modifica stessa.
\end{itemize}

Attraverso questo processo, SemiTO-V garantisce la propria capacità di evolversi senza perdere la propria identità e i propri principi fondanti.


\section{Area Hardware and Logic Dev (HW)}


\subsection*{Articolo \thearticlecnt: Organizzazione dell'Area Hardware and Logic Dev (HW)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Organizzazione dell'Area Hardware and Logic Dev (HW)}
\stepcounter{articlecnt}

L'Area \textit{Hardware and Logic Dev} di SemiTO-V è dedicata alla progettazione, allo sviluppo, alla validazione e alla documentazione di architetture basati su RISC-V e disegni circuitali, in linea con la missione open-source del team.

\begin{itemize}
    \item \textbf{Missione}: Contribuire allo sviluppo di disegno logica (implementazione delle architetture, core, CPU/MCU e moduli basati su RISC-V per i FPGA) e hardware intorno (progettazione degli circuiti e segnali, disegno degli PCB). Progettare disegni innovative, affidabili, aperte e documentate, valorizzando l'apprendimento pratico e il rigore tecnico.
    
    \item \textbf{Struttura}: L'area è organizzata per progetti. Ogni progetto è autonomo e coordinato da un capoprogetto HW, eletto tra i membri attivi dell'area. L'area può essere articolata nei seguenti ruoli:
    \begin{itemize}
        \item Ingegneri di sviluppo FPGA/descrizioni di logica
        \item Ingegneri elettronici delle schede
        \item Ingegneri di sviluppo embedded (hardware)
        \item Ingegneri di rete wireless
    \end{itemize}
    
    \item \textbf{Metodologia di lavoro}: Ogni progetto può adottare la metodologia operativa più adatta (es. milestones fisse, prototipazione rapida ecc.), da definire e documentare all'inizio del progetto stesso.
    
    \item \textbf{Standard tecnici}: I progetti HW devono seguire standard di buona pratica ingegneristica, tra cui: gestione della documentazione tecnica, versionamento dei file di progetto (tipo con git), testing funzionale e validazione dei prototipi.
    
    \item \textbf{Documentazione obbligatoria}: Ogni progetto deve avere almeno i seguenti: I file del progetto, un README utile (architettura, cos'è, come si gira ), licenza open-source.
    
    \item \textbf{Collaborazione inter-aree}: I membri HW collaborano attivamente con le aree SW e PR ove necessario (es. sviluppo firmware, presentazioni pubbliche, gestione logistica dei prototipi).
\end{itemize}

Il rispetto di questi principi è fondamentale per garantire la qualità, la tracciabilità e la crescita continua dell'Area \textit{Hardware and Logic Dev}.

\subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Capoprogetto Hardware and Logic Dev (HW)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Capoprogetto Hardware and Logic Dev (HW)}
\stepcounter{articlecnt}

Ogni Capoprogetto HW è responsabile del coordinamento operativo di un progetto specifico all'interno dell'Area HW di SemiTO-V.  
Il suo compito è garantire la coerenza tecnica, il rispetto delle tempistiche concordate e la valorizzazione del lavoro di tutti i membri coinvolti.

\begin{itemize}
    \item \textbf{Nomina}: Il Capoprogetto HW viene eletto a maggioranza semplice dai membri attivi dell'Area HW, all'avvio di ciascun nuovo progetto.
    
    \item \textbf{Durata}: Il mandato del Capoprogetto dura per tutta la durata del progetto a cui è assegnato. Al termine del progetto, il ruolo decade automaticamente.
    
    \item \textbf{Compiti principali}:
    \begin{itemize}
        \item Coordinare la definizione degli obiettivi tecnici e delle milestone.
        \item Favorire la distribuzione equilibrata delle attività tra i membri.
        \item Monitorare l'avanzamento del progetto e intervenire in caso di criticità operative.
        \item Facilitare il rispetto delle procedure tecniche e di documentazione previste dal codice interno HW.
        \item Mantenere il collegamento con i responsabili delle aree SW e PR per le attività intersettoriali.
    \end{itemize}
    
    \item \textbf{Stile di leadership}: Il Capoprogetto non esercita autorità gerarchica, ma svolge un ruolo di facilitatore e coordinatore, promuovendo l'autonomia e la crescita dei membri del team.
    
    \item \textbf{Revoca o sostituzione}: In caso di inattività prolungata, gravi inadempienze o dimissioni volontarie, il Capoprogetto può essere sostituito su decisione della maggioranza dei membri attivi dell'Area HW.
\end{itemize}

Il ruolo di Capoprogetto rappresenta un'opportunità di crescita tecnica, organizzativa e personale, ed è centrale per il buon esito dei progetti hardware di SemiTO-V.

\section{Area Software and Instruction Dev (SW)}

\subsection*{Articolo \thearticlecnt: Organizzazione dell'Area Software and Instruction Dev (SW)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Organizzazione dell'Area Software and Instruction Dev (SW)}
\stepcounter{articlecnt}

L'Area \textit{Software and Instruction Dev} di SemiTO-V è dedicata alla progettazione, allo sviluppo, al testing e alla documentazione di software a basso livello, firmware, sistemi operativi (sia quelli real time che Linux) e istruzioni RISC-V personalizzati, in coerenza con l'approccio open-source adottato dal team.

\begin{itemize}
    \item \textbf{Missione}: Contribuire allo sviluppo di soluzioni software e istruzioni per i processori RISC-V sia disegnato dentro club che già progettato in modo innovativo, robuste, accessibili e documentate, favorendo l'apprendimento, la sperimentazione e la diffusione della conoscenza tecnica.
    
    \item \textbf{Struttura}: L'area è organizzata su base progettuale. Ogni progetto software e di istruzioni personalizzati è coordinato da un Capoprogetto SW, eletto tra i membri attivi dell'area. L'area puo essere articolata in seguenti ruoli:
    \begin{itemize}
        \item Programmatori low-level di RISC-V assembly (RV32/RV64)
        \item Programmatori di sistemi operativi per RISC-V (Linux per RV64, RTOS per RV32)
        \item Ingegneri di firmware
        \item Ingegneri di sviluppo embedded (software)
        \item Architetti di calcolatori
    \end{itemize}
    
    \item \textbf{Metodologia di lavoro}: Ogni progetto definisce all'inizio per quale sistema (core/processore/microcontrollore) sviluppare i propri codici.
    
    \item \textbf{Standard tecnici}: I progetti SW devono rispettare buone pratiche di ingegneristica, tra qui: gestione del versionamento, adozione di strumenti di code review, testing con il proprio dispositivo e documentazione continua.
    
    \item \textbf{Documentazione obbligatoria}: Ogni progetto deve produrre una documentazione comprensiva di: specifiche funzionali, architettura basata, manuali d'uso, guide per sviluppatori, licenza open-source.
    
    \item \textbf{Collaborazione inter-aree}: I membri SW collaborano strettamente con l'Area HW (per lo sviluppo firmware, istruzioni personalizzati e interfacce) e con l'Area PR (per la promozione e la disseminazione dei risultati).
\end{itemize}

L'Area \textit{Software and Instruction Dev} di SemiTO-V si impegna a coniugare creatività, rigore tecnico e apertura, promuovendo progetti che possano avere un impatto reale e duraturo nell'ambito dei processori.

    \subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Capoprogetto Software (SW)}
    \addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Capoprogetto Software (SW)}
    \stepcounter{articlecnt}

Il Capoprogetto Software è responsabile del coordinamento operativo di un progetto specifico all'interno dell'Area SW di SemiTO-V.  
Il suo ruolo è facilitare la realizzazione tecnica, organizzativa e documentale del progetto, promuovendo collaborazione, qualità e crescita condivisa.

\begin{itemize}
    \item \textbf{Nomina}: Il Capoprogetto SW viene eletto a maggioranza semplice dai membri attivi dell'Area SW, in occasione dell'avvio di ciascun nuovo progetto.
    
    \item \textbf{Durata}: Il mandato del Capoprogetto ha durata limitata alla durata del progetto assegnato. Alla conclusione del progetto, il ruolo decade automaticamente.
    
    \item \textbf{Compiti principali}:
    \begin{itemize}
        \item Coordinare la definizione dei requisiti tecnici, delle priorità e delle milestones del progetto.
        \item Facilitare la suddivisione dei task e promuovere la responsabilizzazione autonoma dei membri.
        \item Monitorare il progresso tecnico, la qualità del codice, la documentazione e il rispetto delle buone pratiche.
        \item Favorire l'adozione di strumenti collaborativi (versionamento, issue tracker, piattaforme di gestione agile).
        \item Coordinare il dialogo con l'Area HW e l'Area PR per le attività interconnesse.
    \end{itemize}
    
    \item \textbf{Stile di leadership}: Il Capoprogetto esercita una leadership di servizio, basata sull'esempio, sul supporto e sulla facilitazione delle dinamiche di squadra, senza imposizioni gerarchiche.
    
    \item \textbf{Revoca o sostituzione}: In caso di inattività grave, abbandono del progetto o altre circostanze straordinarie, il Capoprogetto può essere sostituito tramite decisione della maggioranza semplice dei membri attivi dell'Area SW.
\end{itemize}

Essere Capoprogetto rappresenta un'opportunità formativa unica e un riconoscimento di competenze tecniche, relazionali e organizzative.


\section{Area Public Relations (PR) e Team Lead}

\subsection*{Articolo \thearticlecnt: Organizzazione dell'Area Public Relations (PR)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Organizzazione dell'Area Public Relations (PR)}
\stepcounter{articlecnt}

L'Area Public Relations (PR) di SemiTO-V è responsabile della gestione amministrativa, finanziaria, promozionale e relazionale del team, supportando la crescita interna ed esterna delle attività.

\begin{itemize}
    \item \textbf{Missione}: Curare i rapporti istituzionali, assicurare il supporto burocratico e logistico alle attività tecniche, promuovere l'immagine del team e garantirne la sostenibilità economica nel tempo.
    
    \item \textbf{Struttura}: L'area è articolata in quattro ruoli principali:
    \begin{itemize}
        \item Responsabile Amministrativo
        \item Responsabile Fundraising e Sponsorship
        \item Responsabile Eventi e Competizioni
        \item Responsabile Comunicazione
    \end{itemize}
    
    \item \textbf{Nomina}: I responsabili sono eletti dai membri attivi dell'Area PR a maggioranza semplice, con mandato iniziale di 6 mesi.
    
    \item \textbf{Estensione del mandato}: Dopo i primi 6 mesi, può essere proposta una votazione di conferma per estendere il mandato fino a un massimo di 12 mesi complessivi.
    
    \item \textbf{Rieleggibilità}: I responsabili possono essere rieletti senza limiti di mandato, salvo diversa disposizione deliberata dal team.
    
    \item \textbf{Obblighi di rendicontazione}: Ogni responsabile PR deve redigere report periodici (almeno uno ogni 3 mesi), documentando lo stato delle attività di competenza, i progressi ottenuti, le criticità emerse e le procedure burocratiche consolidate.
    
    \item \textbf{Coerenza operativa}: I responsabili PR devono collaborare attivamente con le Aree HW e SW, assicurando supporto amministrativo, logistico e comunicativo secondo le necessità dei progetti.
\end{itemize}

L'Area PR rappresenta il motore invisibile che sostiene l'esistenza, la crescita e la visibilità di SemiTO-V. Per questo motivo, la sua organizzazione richiede rigore, continuità e spirito di servizio.

\subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Amministrativo (Area PR)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Amministrativo (Area PR)}
\stepcounter{articlecnt}

Il Responsabile Amministrativo ha il compito di garantire la corretta gestione burocratica, documentale e amministrativa delle attività di SemiTO-V, assicurando la piena conformità alle normative interne ed esterne.

\begin{itemize}
    \item \textbf{Nomina}: Il Responsabile Amministrativo è eletto a maggioranza semplice dai membri attivi dell'Area PR, con mandato iniziale di 6 mesi, estendibile fino a 12 mesi previa votazione di conferma.
    
    \item \textbf{Compiti principali}:
    \begin{itemize}
        \item Gestire la documentazione ufficiale del team (domande di riconoscimento, dichiarazioni, richieste di spazi, richieste di fondi, assicurazioni).
        \item Redigere e aggiornare tutti i documenti formali richiesti dal Politecnico di Torino e dagli eventuali partner esterni.
        \item Assicurare il corretto archivio delle pratiche amministrative, sia in formato digitale sia, ove richiesto, in formato cartaceo.
        \item Collaborare con i responsabili dei progetti per garantire la conformità procedurale alle attività svolte (es. autorizzazioni per trasferte, utilizzo attrezzature, gestione spazi).
        \item Codificare e mantenere aggiornate le procedure amministrative interne in appositi documenti di riferimento.
    \end{itemize}
    
    \item \textbf{Rendicontazione}: Il Responsabile Amministrativo deve redigere report sintetici trimestrali sulle attività svolte, da condividere con l'intero team.
    
    \item \textbf{Stile di lavoro}: Il ruolo richiede precisione, affidabilità, capacità di gestire comunicazioni formali e interfacciarsi efficacemente con le istituzioni.
    
    \item \textbf{Revoca o sostituzione}: In caso di inattività prolungata o gravi inadempienze, il Responsabile può essere sostituito con decisione della maggioranza semplice dell'Area PR.
\end{itemize}

Il Responsabile Amministrativo è il garante della solidità istituzionale e operativa di SemiTO-V, nonché il custode della memoria formale delle sue attività.

\subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Fundraising e Sponsorship (Area PR)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Fundraising e Sponsorship (Area PR)}
\stepcounter{articlecnt}

Il Responsabile Fundraising e Sponsorship è incaricato di assicurare la sostenibilità economica di SemiTO-V, sviluppando strategie di raccolta fondi, costruendo relazioni con partner esterni e promuovendo accordi di supporto tecnico o finanziario.

\begin{itemize}
    \item \textbf{Nomina}: Il Responsabile Fundraising è eletto a maggioranza semplice dai membri attivi dell'Area PR, con mandato iniziale di 6 mesi, estendibile fino a 12 mesi previa votazione di conferma.
    
    \item \textbf{Compiti principali}:
    \begin{itemize}
        \item Individuare opportunità di sponsorizzazione, bandi di finanziamento, grant e altre forme di supporto esterno.
        \item Gestire i rapporti formali con sponsor, aziende, enti pubblici e privati, curando la comunicazione istituzionale.
        \item Redigere proposte di collaborazione, lettere ufficiali e materiali informativi destinati ai potenziali partner.
        \item Supportare l'elaborazione di budget preventivi e piani di spesa associati a progetti specifici o a esigenze operative generali.
        \item Monitorare l'andamento delle sponsorizzazioni attive, garantendo il rispetto degli obblighi reciproci.
    \end{itemize}
    
    \item \textbf{Rendicontazione}: Il Responsabile Fundraising deve redigere report trimestrali sulle attività di fundraising e sponsorship, illustrando contatti avviati, risultati raggiunti e azioni future.
    
    \item \textbf{Stile di lavoro}: Il ruolo richiede capacità di negoziazione, chiarezza comunicativa, attenzione alle dinamiche contrattuali e sensibilità strategica.
    
    \item \textbf{Revoca o sostituzione}: In caso di inattività prolungata o gravi inadempienze, il Responsabile può essere sostituito con decisione della maggioranza semplice dell'Area PR.
\end{itemize}

Il Responsabile Fundraising e Sponsorship rappresenta il collegamento tra SemiTO-V e il mondo esterno, assicurando risorse, visibilità e credibilità per sostenere la crescita del team.

\subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Eventi e Competizioni (Area PR)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Eventi e Competizioni (Area PR)}
\stepcounter{articlecnt}

Il Responsabile Eventi e Competizioni si occupa dell'organizzazione logistica e amministrativa delle partecipazioni del team a eventi esterni, fiere, hackathon, conferenze, e di tutte le attività pubbliche di SemiTO-V.

\begin{itemize}
    \item \textbf{Nomina}: Il Responsabile Eventi è eletto a maggioranza semplice dai membri attivi dell'Area PR, con mandato iniziale di 6 mesi, estendibile fino a 12 mesi previa votazione di conferma.
    
    \item \textbf{Compiti principali}:
    \begin{itemize}
        \item Monitorare opportunità di partecipazione a eventi nazionali e internazionali pertinenti alle attività del team (eventi su RISC-V, open-source, elettronica embedded, circuiti integrati).
        \item Coordinare le iscrizioni, la gestione delle candidature, la logistica di viaggio e la registrazione delle presenze.
        \item Gestire la documentazione necessaria per autorizzazioni interne (PoliTO, assicurazioni, utilizzo fondi, richieste di supporto logistico).
        \item Organizzare eventi interni o pubblici promossi da SemiTO-V (es. workshop, presentazioni, open day).
        \item Assicurare che ogni partecipazione esterna sia documentata a fini di reportistica e promozione.
    \end{itemize}
    
    \item \textbf{Rendicontazione}: Il Responsabile Eventi deve redigere un report sintetico al termine di ogni evento significativo, includendo attività svolte, esiti principali e proposte di miglioramento.
    
    \item \textbf{Stile di lavoro}: Il ruolo richiede capacità organizzative, attenzione ai dettagli, gestione efficiente delle tempistiche e delle risorse.
    
    \item \textbf{Revoca o sostituzione}: In caso di inattività o gravi inefficienze organizzative, il Responsabile può essere sostituito con decisione della maggioranza semplice dell'Area PR.
\end{itemize}

Il Responsabile Eventi e Competizioni contribuisce in modo essenziale alla visibilità e al riconoscimento esterno di SemiTO-V, curando con professionalità ogni momento di rappresentanza del team.

\subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Comunicazione (Area PR)}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Responsabile Comunicazione (Area PR)}
\stepcounter{articlecnt}

Il Responsabile Comunicazione ha il compito di curare l'immagine pubblica di SemiTO-V, gestire la presenza online del team e supportare la diffusione dei progetti e delle iniziative, in linea con la missione open-source e i valori del gruppo.

\begin{itemize}
    \item \textbf{Nomina}: Il Responsabile Comunicazione è eletto a maggioranza semplice dai membri attivi dell'Area PR, con mandato iniziale di 6 mesi, estendibile fino a 12 mesi previa votazione di conferma.
    
    \item \textbf{Compiti principali}:
    \begin{itemize}
        \item Curare la gestione e l'aggiornamento dei canali ufficiali del team (sito web, social media, piattaforme di community).
        \item Redigere comunicati, articoli, post e materiali promozionali destinati sia all'interno che all'esterno del Politecnico.
        \item Supportare la visibilità dei progetti tecnici, raccontandone l'evoluzione in modo accessibile e coinvolgente.
        \item Coordinare la coerenza dell'immagine grafica del team (logo, palette colori, template di presentazione, documentazione pubblica).
        \item Collaborare con i Responsabili Fundraising e Eventi per promuovere iniziative specifiche o campagne di raccolta fondi.
    \end{itemize}
    
    \item \textbf{Rendicontazione}: Il Responsabile Comunicazione deve fornire un report sintetico trimestrale sulle attività svolte, i canali attivati, l'engagement generato e le proposte di miglioramento della presenza online.
    
    \item \textbf{Stile di lavoro}: Il ruolo richiede creatività, precisione espositiva, capacità di storytelling tecnico e attenzione alla reputazione pubblica del team.
    
    \item \textbf{Revoca o sostituzione}: In caso di inattività o gestione inadeguata della comunicazione istituzionale, il Responsabile può essere sostituito con decisione della maggioranza semplice dell'Area PR.
\end{itemize}

Il Responsabile Comunicazione traduce il lavoro di SemiTO-V in narrazioni accessibili e coinvolgenti, alimentando l'identità e la presenza pubblica del team.



\subsection*{Articolo \thearticlecnt: Ruolo e Nomina del Team Lead}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Ruolo e Nomina del Team Lead}
\stepcounter{articlecnt}

Il Team Lead ha il compito di facilitare la coesione strategica tra le aree del team, promuovere la visione di lungo periodo del progetto SemiTO-V e rappresentare il gruppo verso l’esterno quando richiesto.  
Non esercita autorità gerarchica, ma agisce come figura di riferimento trasversale per la visione, il supporto organizzativo e la continuità del progetto.

\subsection*{Nomina e durata}
Il Team Lead è eletto a maggioranza semplice dai membri attivi del team, con mandato della durata di 12 mesi. Una persona puo fare il Team Lead al massimo per 1 anno. Il ruolo decade automaticamente in caso di abbandono volontario o uscita dal circuito accademico.

All'avvio del team, per finalità burocratiche e di registrazione, viene designato un Team Lead fittizio. Tale figura decade automaticamente entro 2 mesi dalla fondazione del team, salvo rielezione, e dovrà essere sostituita attraverso una votazione democratica aperta a tutti i membri attivi.

\subsection*{Compiti principali}
\begin{itemize}
  \item Coordinare le riunioni plenarie e stimolare il confronto strategico.
  \item Supportare Capiprogetto/Responsabili d’area nella gestione di situazioni complesse.
  \item Monitorare il benessere del team e promuovere la prevenzione dei conflitti.
  \item Curare la documentazione strategica del team (roadmap, visione evolutiva, relazioni istituzionali).
  \item Facilitare il passaggio generazionale e la trasmissione della cultura interna.
\end{itemize}

\subsection*{Rimozione anticipata}
La rimozione del Team Lead può essere proposta da almeno tre membri attivi del team, con una motivazione scritta anche informale.  
La proposta viene discussa in riunione plenaria e sottoposta a votazione: è richiesta una maggioranza semplice dei membri attivi presenti.  
In caso di approvazione, si procede a una nuova elezione entro due settimane.

\subsection*{Stile di leadership}
Il Team Lead esercita una leadership di servizio e visione, promuovendo l’autonomia delle aree e la coesione del gruppo.


\section{Attestazione risultati e consolidamento del know-how}

\subsection*{Articolo \thearticlecnt: Produzione di progetti dimostrativi}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Produzione di progetti dimostrativi}
\stepcounter{articlecnt}

SemiTO-V si impegna a promuovere la realizzazione periodica di progetti dimostrativi, utili al trasferimento del know-how interno, alla valorizzazione delle competenze maturate e alla presentazione delle attività del team verso l’esterno.\\
Le aree sono incoraggiate a contribuire ogni anno ad almeno un progetto dimostrativo, compatibilmente con le risorse disponibili e l’andamento delle attività.\\
I progetti possono essere manufatti o software dimostrativi, articoli di ricerca e/o presentazioni o report del lavoro svolto durante tutta la vita dell'attività del team.

\subsection*{Articolo \thearticlecnt: Pianificazione e collaborazione nei progetti dimostrativi}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Pianificazione dei progetti}
\stepcounter{articlecnt}

I progetti dimostrativi dovrebbero essere pianificati con cadenza annuale, anche in forma preliminare.\\
È fortemente incoraggiata la collaborazione tra le Aree Hardware e Software, in modo da valorizzare l’integrazione tra sviluppo logico, elettronico e sistemistico.\\
L’Area Public Relations supporta i progetti dimostrativi nella fase presentazione pubblica ed eventuale candidatura a eventi, fiere o workshop.

\subsection*{Articolo \thearticlecnt: Finalità dei progetti}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Finalità dei progetti}
\stepcounter{articlecnt}

I progetti dimostrativi hanno lo scopo di consolidare e trasmettere il know-how acquisito, documentare le competenze sviluppate nel tempo e rafforzare l’identità tecnica e pubblica del team.\\
Possono essere impiegati, a titolo esemplificativo ma non esaustivo, per la partecipazione a eventi di presentazione (workshop, fiere, summit, open day), per attività di disseminazione scientifica, come materiale o dispositivi da utilizzare in competizioni di settore, oppure come riferimento per la formazione interna.


\subsection*{Articolo \thearticlecnt: Standardizzazione operativa e cultura documentale}
\addcontentsline{toc}{subsection}{Articolo \thearticlecnt: Standardizzazione operativa e cultura documentale}
\stepcounter{articlecnt}


Per garantire qualità, continuità e tracciabilità del lavoro, SemiTO-V promuove l'adozione sistematica di strumenti di standardizzazione operativa.

\subsection*{Principi generali}
Ogni attività significativa, sia tecnica che organizzativa, deve essere codificata in forma di:
\begin{itemize}
  \item \textbf{Procedure operative}: descrizione dettagliata dei passaggi da seguire per lo svolgimento di task ricorrenti o critici.
  \item \textbf{Checklist di controllo}: elenchi di verifica da utilizzare prima, durante o dopo lo svolgimento di attività, per garantire qualità, sicurezza e coerenza.
  \item \textbf{Strumenti collaborativi}: utilizzo di piattaforme condivise (repository, documentazione, versionamento) per assicurare trasparenza e accessibilità.
\end{itemize}

\subsection*{Ambiti di applicazione}
Le procedure e le checklist devono essere sviluppate in ogni area del team, con particolare attenzione a:
\begin{itemize}
  \item Sviluppo hardware e software (rilasci, test, revisioni, compilazione)
  \item Partecipazione a eventi (logistica, iscrizioni, preparazione materiale)
  \item Fundraising e rapporti istituzionali (template, contatti, invii, tracciamento)
  \item Onboarding e formazione dei nuovi membri
\end{itemize}

\subsection*{Obbligo minimo per i progetti attivi}
Ogni progetto attivo di SemiTO-V, in qualsiasi area, deve essere accompagnato da almeno una checklist o una procedura documentata.  
Questa documentazione va redatta nella fase iniziale del progetto, mantenuta aggiornata durante lo sviluppo e archiviata al termine delle attività.

\subsection*{Gestione e condivisione}
Ogni codice interno di area (vedi Articolo 4 di questo documento) è responsabile della redazione, aggiornamento e revisione periodica della propria documentazione operativa.  
Il Team Lead e i Responsabili d’area collaborano per promuovere una cultura documentale coerente, accessibile e migliorabile nel tempo.

Tutta la documentazione operativa deve essere salvata in formato digitale e resa accessibile a tutti i membri attivi del team.  
È consigliato l’uso di piattaforme collaborative come \textbf{GitHub}, \textbf{GitLab}, \textbf{Google Drive}, \textbf{Notion} o simili, che garantiscano versionamento, accesso controllato e tracciabilità delle modifiche.



\newpage

\section{Glossario}

\begin{description}

    \item[ISA] Instruction Set Architecture che definisce architettura di un processore tipo il RISC-V (RV32, RV64), ARM (arm64) e X86 (x64 usato da solo Intel/AMD)

    \item[Istruzione personalizzato] Istruzione implementato per un ISA dagli sviluppatori oltre quelli definiti originalmente.

    \item[Checklist Operativa] Elenco strutturato di azioni da completare durante l'esecuzione di un processo o di una procedura, utilizzato per garantire la qualità, la sicurezza e la conformità agli standard previsti.
    
    \item[Code Review] Revisione sistematica del codice sorgente da parte di uno o più membri del team, con l'obiettivo di individuare errori, migliorare la qualità tecnica e garantire la coerenza stilistica dei progetti software.
    
    \item[Facilitatore] Figura che aiuta a gestire discussioni, mediare divergenze e favorire la collaborazione all'interno del team, senza esercitare autorità gerarchica o decisionale.
    
    \item[Issue Tracker] Strumento digitale utilizzato per registrare, assegnare e monitorare attività, problemi o richieste all'interno di un progetto, facilitando l'organizzazione e la trasparenza del lavoro di squadra.
    
    \item[Milestone] Obiettivo intermedio importante all'interno di un progetto, che segna il completamento di una fase significativa del lavoro e funge da punto di controllo per la valutazione dell'avanzamento.
    
    \item[Onboarding] Processo di integrazione dei nuovi membri all'interno del team, che comprende l'affiancamento, l'apprendimento delle procedure operative e la valutazione della compatibilità con i valori e il metodo di lavoro di SemiTO-V.
    
    \item[Open Source] Modello di sviluppo e distribuzione in cui il codice sorgente di un progetto viene reso pubblicamente accessibile, consentendo a chiunque di studiarlo, modificarlo e ridistribuirlo secondo licenze specifiche.
    
    \item[Repository (Repo)] Archivio centralizzato dove vengono conservati i file di progetto, gestiti attraverso un sistema di versionamento come Git, che consente di tracciare le modifiche e collaborare in modo ordinato.
    
\end{description}





\end{document}
