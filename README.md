### Team Workshop: LockBit

```
Groupe 2
```

## Agenda

##### 1. Présentation des membres du groupe de travail

- Claude-Olivier
- Sébastien Hals
- Michaël Batungwanayo
- Antoine Blairon

##### 2.Lockbit

- Qu'est-ce que c'est? ( présenté par Antoine)
- Vulnérabilité exploitée(présenté par Michaël)
- Impacts de cette attaque (présenté par Sébastien)
- Remédiation mise en œuvre(présenté par Claude-Olivier)
- Conséquencespour Lockbit(présenté par Sébastien)
- Conclusion (présentation par Antoine)


## 1. Présentation des membres du groupe

#### Claude-Olivier

- Senior Asset Manager à la STIB depuis 2016. Actif depuis 2005

#### essentiellement dans le contrôle-commande des réseaux Haute

#### Tension ainsi que la signalisation et automatismes ferroviaire.

- Ingénieur Civil en Informatique et Gestion (UMons - 2013) &

- Ingénieur Industriel en Électricité (ISIB - 2004)

- Technologies préférées: C#, C++, C, Python, CPLEX


## 1. Présentation des membres du groupe

#### Sébastien

- Bachelier en Informatique de Gestion et Certificat d'Aptitude Pédagogique

- Enseignant à l'INRACI en 4ème/5ème année en informatique industrielle

- Technologies préférées: C#, Javascript (React), Python


## 1. Présentation des membres du groupe

#### Michaël

- 2 Bachelors : Informatique de gestion & Gestion Marketing
- J'ai travaillé dans le commerce, puis comme développeur Fullstack d'applications web(Framework PHP Laravel,VueJS,
 ReactJS).
- Bonnes connaissances en Java, Python, C#, C/C++, Angular.
- Linuxien (mon principal système d'exploitation depuis 10 ans). À l'aise avec le terminal :-).


## 1. Présentation des membres du groupe

#### Antoine

- Analyste programmeur de formation
- Depuis 20 ans dans le domaine de l'informatique
- Spécialisation dans l'Infrastructure IT & sécurité
- Connaissances en audit IT sécurité (ISO27001 & NIS2)
- Actuellement IT Infra Manager & CISO dans une PME (150 FTE)
- Motivé par l'apprentissage de connaissances techniques


## 2. Lockbit

**Qu'est-ce que c'est Lockbit?**

Lockbitest un ransomware connu depuis 2019. Ce logiciel malveillant extorquait et/ou chiffrait les données pour les rendre
inaccessibles par l'utilisateur qui les détenait. Une rançon était alors négociée publiquement.
Les systèmes d'exploitation visés étaient Windows et Linux. Une version à destination de l'OS MAC a été élaborée à partir
d'avril 2023.
En 2022, le code a été rendu public sur GitHub et réutilisé par de nombreux groupes. Il existerait désormais plus de 400
variantes!
De grandes entreprises nationales et mondiales telles que Thales, Continental, La Poste ou des hôpitaux ont été victimes de ce
ransomware. Nous avons connaissance de minimum 1700 attaques dans le monde depuis 2020!

Ce nom représente également le groupe de hackersrusse qui l'exploite. Ils n'attaquent pas les entités Russes ainsi que leurs
alliés.
Ils sont structurés comme une startup et beaucoup plus organisés que d'autres groupes. Par exemple, ils ont un processus de
recrutement élaboré pour évaluer les compétences de leurs membres. Ils proposent également un modèle de partenariat.

Comme beaucoup de groupes de pirates, ils demandent à être payés en Bitcoins.


## 2. Lockbit

**Vulnérabilités exploitées?**

- Exploitation des accès RDP (RemoteDesktop Protocol), protocole réseau d'accès à distance
de Microsoft, mal configurées.
- Grâce auxinformations d'identification volées, les pirates peuvent escaladerdes privilèges
(devenir le root) pour contrôler complètement le système et infecter d'avantage de machines).
- Failles de sécurité dans des logiciels tiers (VPN mal configuré, outils de gestion à distance,...)
- Failles dans l'Active Directory (Gestionnaire des utilisateurs, des machines et des ressources
réseaux sur les environnementsWindows) exploitées dans le but d'escalader ou d'étendre ses
privilèges.
- Failles zéro-dayc’est-à-dire des vulnérabilités encore inconnues.


## 2. Lockbit

###### Impacts des attaques

- Leak: Informations confidentielles
- Systèmes internes compromis
- Impact sur les entreprises


## 2. Lockbit -

**Mesures préventives (avant l’attaque):**

- **Sauvegarde régulières et complètes des données critiques**. Sauvegarde à conserver sur
    des supports non connectés. Sauvegarde à tester régulièrement.
- **Segmentation du réseau** pour limiter le mouvement latéral de l’attaquant une fois qu’il a
    compromis une partie du réseau (e.g: Isoler les serveurs de DB des Workstation ordinaire)
- Appliquer rapidement les **patchs de sécurité** pour éviter de trainer longtemps avec les
    failles que LockBitpourrait exploiter

**Incident Management (pendant l’attaque):**

- **Déconnecter immédiatement les machines infectées** : Déconnexion LAN, Wi-Fi et
    d’internet.
- **Mettre hors ligne** les serveurs critiques.
- **Bien identifier** la variante de Lockbit.


## 2. Lockbit -

**Mesures correctives et reprise (après l’attaque):**

- **Restaurer les systèmes** à partir de versions antérieures à l’attaque. Les systèmes restaurés
    soient **complétement patchés et à jour.**
- **Mettre en place d’une surveillance accrue** pour détecter toute tentative de réinfection.
    Des outils de surveillance des journaux, des IDS/IPS (Systèmes de détection et des SIEM
    (Security Information and Event Management) peuvent être utilisés pour surveiller
    l’infrastructure**.**
- **Former et sensibiliser l’ensemble du personnel,** en particulier en ce qui concerne les
    emails de phishing.


# 3. Conséquence pour

# Lockbit

- L'opération Cronosa porté un coup à Lockbit(site
    web fermés, clés de déchiffrement)
- Plusieurs personnes impliquées dans le
    développement de Lockbitont été ajoutés à la base
    de données du FBI, une rançon est toujours
    disponible.
- Plusieurs internautes ont révélé des informations sur
    ces mêmes personnes (@fs0c131y sur Twitterpar
    exemple)


## 4. Conclusion

Les ransomwares font parties des pires attaques qu'une entreprise peut subir.

En plus de l'impact sur les opérations de l'entreprise, elle peut également avoir des conséquences
financières importantes et également sur l'image de l'entreprise.

C'est pour cette raison que plusieurs nouvelles législations ont vu le jour telles que:

- DORA
- PCI DSS
- GDPR
- NIS

Celles-ci visent à accroitre sensiblement les niveaux en matière:

- D'identification (des menaces, des actifs informatiques)
- De protection (des actifs IT, sensibilisation)
- De réponse aux événements (incidents et crises)
- De mécanismes de restauration (backup & recovery)


#### Des questions?

#### Sébastien, Claude-Olivier, Michaël et Antoine

#### vous remercie pour votre attention :)

