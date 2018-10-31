---

copyright:

  years:  2016, 2018

lastupdated: "2018-10-03"

---

# Analyse et révision

Lorsque vous analysez des hôtes, des machines virtuelles et des dispositifs virtuels, vous les évaluez par rapport aux lignes de ligne et des groupes de lignes de base afin de déterminer leur niveau de conformité. Les objets d'inventaire sont analysés, et les résultats passés en revue pour déterminer leur conformité par rapport aux lignes de base et aux groupes de lignes de base. Les résultats d'analyse peuvent être filtrés avec une recherche de texte, une sélection de groupe ou de ligne de base et une sélection d'état de conformité. Vous pouvez initier les analyses suivantes :
*	**Lancement manuel d'une analyse d'hôtes vSphere ESXi** - Vous pouvez analyser des hôtes vSphere ESXi dans l'inventaire vSphere par rapport aux lignes de base et aux groupes de lignes de base associés.
*	**Lancement manuel d'une analyse de machines virtuelles et de dispositifs virtuels** - Vous pouvez analyser des machines virtuelles et des dispositifs virtuels dans l'inventaire vSphere par rapport aux lignes de base et aux groupes de lignes de base associés.
*	**Lancement manuel d'une analyse d'objet conteneur** - Lancez l'analyse simultanée des hôtes, des machines virtuelles et des dispositifs virtuels, en effectuant l'analyse d'un objet conteneur qui correspond à un centre de données ou un dossier de centre de données.
*	**Planification d'une analyse** - Vous pouvez configurer le client vSphere Web Client pour analyser des machines virtuelles, des dispositifs virtuels et des hôtes ESXi à des heures spécifiques ou aux intervalles qui vous conviennent.

##	Lancement manuel d'une analyse d'hôtes vSphere ESXi

1.	Cliquez sur le bouton **Scan for Updates** et sélectionnez **Patches and Extensions and Upgrades**, cliquez ensuite sur **OK**.
2.	Une fois l'analyse terminée, sélectionnez **Critical Host Patches** et dans le panneau inférieur, passez en revue les correctifs de chaque hôte
3.	En cliquant sur le numéro d'un correctif, une fenêtre s'affiche avec les détails du correctif.
4.	Passez-en revue et répétez ces étapes pour les correctifs non critiques (**Non-Critical Patches**).

Notez que les fichiers journaux de VUM peuvent se trouver dans _/var/log/vmware/vmware-updatemgr/vum-server/vmware-vum-server-log4cpp.log_

##	Lancement manuel d'une analyse de machines virtuelles et de dispositifs virtuels

Vous pouvez analyser des machines virtuelles et des dispositifs virtuels dans l'inventaire vSphere par rapport aux lignes de base et aux groupes de lignes de base associés. Les machines et dispositifs virtuels que vous sélectionnez sont analysés par rapport aux lignes de base associées, en fonction des options que vous avez choisies. Tous les objets enfant sont également analysés, de sorte que plus l'infrastructure virtuelle est importante et plus vous lancez l'analyse au niveau le plus haut dans la hiérarchie des objets, plus l'analyse prend du temps et plus la vue de conformité est précise.

1.	A l'aide du client vSphere Web Client, sélectionnez **Home** > **VMs and Templates**.
2.	Cliquez avec le bouton droit de la souris sur une _machine virtuelle_, un _dispositif virtuel_ ou un _dossier de machines virtuelles et de dispositifs virtuels_ et cliquez sur **Scan for Updates**.
3.	Sélectionnez les types de mises à jour à rechercher. Les options possibles sont : _Virtual Appliance upgrades, VM Hardware upgrades_ et _VMware Tools upgrades_.
4.	Cliquez sur **Scan**.

##	Lancement manuel d'une analyse d'objet conteneur

Lancez l'analyse simultanée des hôtes, des machines virtuelles et des dispositifs virtuels, en effectuant l'analyse d'un objet conteneur qui correspond à un centre de données ou un dossier de centre de données.
1.	A l'aide du client vSphere Web Client, sélectionnez **Home** > **VMs and Templates**.
2.	Cliquez avec le bouton droit de la souris sur un _centre de données_ ou un _dossier de centre de données_, puis cliquez sur **Scan for Updates**.
3.	Sélectionnez les types de mises à jour à rechercher. Les options possibles sont : _Virtual Appliance upgrades, VM Hardware upgrades_ et _VMware Tools upgrades_.
4.	Cliquez sur **Scan**.

##	Planification d'une analyse

Vous pouvez configurer le client vSphere Web Client pour analyser des machines virtuelles, des dispositifs virtuels et des hôtes vSphere ESXi à des heures spécifiques ou aux intervalles qui vous conviennent.

1.	A l'aide du client vSphere Web Client, sélectionnez un objet dans l'inventaire. Tous les objets enfant de l'objet que vous sélectionnez sont également analysés.
2.	Sélectionnez l'onglet **Monitor** et cliquez sur **Task & Events**.
3.	Sélectionnez **Scheduled Tasks** et cliquez sur **Schedule a New Task**.
4.	Sélectionnez **Scan for Updates** dans la liste déroulante qui s'affiche. L'assistant de recherche des mises à jour s'ouvre.
5.	Sur la page Edit Settings, sélectionnez les types de mises à jour à rechercher pour l'objet d'inventaire. Vous devez sélectionner au moins un type d'analyse. Sur la page des options de planification Scheduling, décrivez et planifiez la tâche d'analyse.
6.	Entrez un nom unique, et éventuellement, une description pour la tâche d'analyse. Cliquez sur **Change** pour définir la fréquence et l'heure de début de la tâche d'analyse. Cliquez sur **OK**.
7.	La tâche d'analyse est répertoriée dans la vue Scheduled Tasks de vSphere Web Client.

### Liens connexes

* [VMware HCX on IBM Cloud Solution](https://www.ibm.com/cloud/garage/files/HCX_Architecture_Design.pdf)
* [VMware Solutions on IBM Cloud Digital Technical Engagement](https://ibm-dte.mybluemix.net/ibm-vmware) (démonstrations)