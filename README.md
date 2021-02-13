## Internet_Security_Gr24

# Detyra e tretë: “Zhvillimi i aplikacionit i cili përdorë librarinë Python Nmap për simulimin e kontrolleve me NMAP.”

Hyrje

Në projektin e tretë në kuadër të lëndës “Siguria në Internetë’shtë dhënë detyra si vijon:
Aplikacioni duhet të përmbajë një meny për përzgjedhjen e opcioneve/funksionaliteteve të veta. Menyja duhet të jetë e punuar si GUI (graphical user interface) duke përdorur vetëm modulin tkinter të Python.
Aplikacionet duhet të shmangin përdorimin e moduleve të gatshme përvec në rastin kur një gjë e tillë është e pashmangshme.
Zhvillimi i aplikacioni i cili perdor librarine Python Nmap per simulimin e kontrolleve me NMAP.”

Projekti është zhvilluar me python dhe është publik në platformën “github” në linkun: https://github.com/tonikrasniqi/Internet_Security_Gr24


Përshkrimi i projektit

Fillimisht do të njoftohemi me disa terma të cilët do ti përdorim në vijim.
Çfarë është Nmap?
Nmap (Rrjetuesi i Rrjetit) është një skanues sigurie, i shkruar fillimisht nga Gordon Lyon (i njohur gjithashtu me pseudonimin e tij Fyodor Vaskovich), dhe përdoret për të zbuluar host dhe shërbime në një rrjet kompjuterik, duke ndërtuar kështu një hartë të rrjetit. Për të përmbushur qëllimin e tij, Nmap dërgon pako të punuara posaçërisht tek host (et) e synuar dhe më pas analizon përgjigjet e tyre.
Disa nga tiparet e dobishme të Nmap përfshijnë:
Zbulimi i hostit : Kjo mundëson identifikimin e hostëve në çdo rrjet. Për shembull, renditja e hostëve që i përgjigjen kërkesave të TCP dhe / ose ICMP ose kanë një port të veçantë të hapur.
Skanimi i Portit : Renditja (numërimi dhe renditja një nga një) e të gjitha portave të hapura në hostet e synuara.
Zbulimi i Versionit : Marrja në pyetje e shërbimeve të rrjetit në pajisjet e largëta për të përcaktuar emrin e aplikacionit dhe numrin e versionit.
Zbulimi i OS : Përcaktimi i sistemit operativ dhe karakteristikave të pajisjeve të pajisjeve të rrjetit.
Ndërveprimi i Shkrueshëm me synimin : Duke përdorur Nmap Scripting Engine (NSE) dhe gjuhën e programimit Lua, ne mund të shkruajmë lehtësisht skripte për të kryer operacione në pajisjet e rrjetit.




Pjesa e Kodit

Në këtë pjesë kemi importuar socketen ku kemi përdorur modulin “tkinter”.
![Screenshot_4](https://user-images.githubusercontent.com/53190272/107861783-594f4500-6e48-11eb-9707-a9e96073eb8e.png)


Në këtë pjesë të kodit  kemi krijuar klasën “Port Scanner” me hostin “google.com” dhe fillimin e portit 70 dhe mbarimin 85
![Screenshot_5](https://user-images.githubusercontent.com/53190272/107861821-ac28fc80-6e48-11eb-99c8-2757ba3d3e2d.png)

Në këtë pjesë të kodit fillon skanimi  porteve.
![Screenshot_1](https://user-images.githubusercontent.com/51675513/107861879-1641a180-6e49-11eb-896b-de96ff043eaa.png)

Në ketë pjesë të kodit kemi krijuar “gui” për  butonat kemi përcaktuar ngjyren e backgroundit dhe shkronjave. 
![Screenshot_2](https://user-images.githubusercontent.com/51675513/107861914-4b4df400-6e49-11eb-9836-5643238a8bf2.png)


Testimi

Ekzekutimi I fajllit portscan.py
Hapi I parë: Ne folderin perkates ‘Skanimi’  hapim cmd(Command Prompt) dhe shkruajmë emrin e fajllit në këtë rast portscan.py

![Screenshot 2021-02-13 221638](https://user-images.githubusercontent.com/57811400/107861945-8d773580-6e49-11eb-9be6-4631d01cd114.png)

 Ekzekutimi I fajllit portscan bëhet pasi te klikojm Enter  shfaqet pamja në vijim

![Screenshot 2021-02-13 221703](https://user-images.githubusercontent.com/57811400/107861991-e1821a00-6e49-11eb-87dc-7c98f62a2ca9.png)

Pastaj  pas klikimit scan skanohet portat prej 70-85 ku në këtë rast 80 e shfaq si opended(sit e hapur) pasi që Hosti esht google.com dhe numri I portes se http është 80 .
