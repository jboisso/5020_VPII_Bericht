# Read ME

## Packages für Latex in VSCode:

- LaTeX
- LaTeX Utilities
- LaTeX Workshop
- LTeX+ Grammar / spell checking
  - benötigt idr. Strawberry Perl [Download](https://strawberryperl.com/)
- Makefile Tools
- MKiKTex Console: Einstellungen > Paketinstallation > Pakete (on-the-fly) -> "immer"

## GIT Setup: (nur für Repo besitzer)

1. Ordner lokal erstellen
2. Ordner in Terminal öffnen und folgende Befehle ausführen:
3. git init
4. git remote add origin https://github.com/jboisso/5020_VPII_Bericht (oder https://github.com/jboisso/3030_3DA_Bericht.git)
5. git pull

## GIT Setup from local folder to Github Repo: (nur für Repo besitzer)

1. Lokaler Ordner in Terminal öffnen
2. Folgende Befehle ausführen:
   - git init
   - git remote add origin [link zum Repo]
   - git add .
   - git commit -m "your commit message"
   - git push --set-upstream origin master

## GIT Freigabe für Mitwirkende: (nur für Repo besitzer)

2. Als Entwickler (Contributors) hinzufügen (Settings > Collaborators > Add people)
3. GitHub Account mit Email einladen
4. Teilnehmende müssen ANGEMELDET auf den link klicken

## Öffnen in Vs Code:

Open Folder -> Hauptordner mit Main drin öffnen
in VS-Code: linker Balken -> TEX -> View LaTeX PDF

## Tipps & Tricks

- ctrl drücken und in PDF-Vorschau auf Text klicken -> öffnet Text in Code
- Doppelcklick auf Fehler in Problem springt zu Fehler in File

## GIT Ablauf bei Änderungen:

### Jedes mal vor Beginn der Arbeit machen!

1. LaTeX Ordner in Visual Studio Code mit Open Folder geöffnet
2. Terminal in Visual Studio Code öffnen, kontrollieren ob korrekter Pfad (Ordner mit LaTeX)
3. folgende Befehle im Terminal ausführen:
   a. git pull

### Jedes mal vor Beenden der Arbeit machen!

1. LaTeX Ordner in Visual Studio Code mit Open Folder geöffnet
2. Terminal in Visual Studio Code öffnen, kontrollieren ob korrekter Pfad (Ordner mit LaTeX)
3. folgende Befehle im Terminal ausführen:
4. git add .
5. git commit -m "Was wurde gemacht"
6. git push

## Referenzieren:

### Tabellen:

in Text:
Text~\ref{tab:Bildflugparameter}
in Tabelle:
\begin{table}[h!]
...
\label{tab:Bildflugparameter}

### Kapitel:

in Text:
Text~\ref{subsec:Instrumentarium}
Im Titel:
\subsection{Instrumentarium}
\label{subsec:Instrumentarium}

-> Analog für Sections, Bilder mit
ref{sec:...}
ref{fig:...}
