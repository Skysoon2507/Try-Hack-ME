---


---

<h1 id="burp-suite-community">Burp Suite Community</h1>
<h2 id="onglets-et-utilité">Onglets et utilité</h2>
<ul>
<li>
<p><strong>Proxy :</strong> L’aspect le plus connu de Burp Suite , le Burp Proxy nous permet d’intercepter et de modifier les requêtes/réponses lors de l’interaction avec des applications Web.</p>
</li>
<li>
<p><strong>Répéteur :</strong> La deuxième fonctionnalité Burp la plus connue nous permet de capturer, modifier, puis renvoyer la même demande plusieurs fois. Cette fonctionnalité peut être absolument inestimable, en particulier lorsque nous devons créer une charge utile par essais et erreurs (par exemple dans une injection de langage <strong>SQLi</strong> - S tructured <strong>Query</strong> Language <strong>)</strong> ou lorsque nous testons la fonctionnalité d’un point de terminaison pour détecter des failles <strong>.</strong></p>
</li>
<li>
<p><strong>Intruder :</strong> Bien que le débit soit sévèrement limité dans Burp Community, nous permet de diffuser des requêtes sur un point final. Ceci est souvent utilisé pour les attaques par force brute ou pour fuzz les points de terminaison.</p>
</li>
<li>
<p><strong>Décodeur :</strong> bien que moins utilisé que les fonctionnalités mentionnées précédemment, Decodeur fournit toujours un service précieux lors de la transformation des données, soit en termes de décodage des informations capturées, soit en encodant une charge utile avant de l’envoyer à la cible. Bien qu’il existe d’autres services disponibles pour faire le même travail, le faire directement dans Burp Suite peut être très efficace.</p>
</li>
<li>
<p><strong>Comparer :</strong> Comme son nom l’indique, Comparer nous permet de comparer deux éléments de données au niveau du mot ou de l’octet. Encore une fois, ce n’est pas quelque chose d’unique à Burp Suite , mais le fait de pouvoir envoyer des données (potentiellement très volumineuses) directement dans un outil de comparaison avec un seul raccourci clavier peut accélérer considérablement les choses.</p>
</li>
<li>
<p><strong>Séquenceur :</strong> nous utilisons généralement Sequencer pour évaluer le caractère aléatoire des jetons tels que les valeurs des cookies de session ou d’autres données générées prétendument aléatoires. Si l’algorithme ne génère pas de valeurs aléatoires sécurisées, cela pourrait ouvrir des voies d’attaque dévastatrices.</p>
</li>
</ul>
<h3 id="exemple-utilisation-burp-suite-cross-scripting">Exemple utilisation burp suite cross scripting</h3>
<p><code>&lt;script&gt;alert("Succ3ssful XSS")&lt;/script&gt;</code>. Après avoir collé la charge utile, nous devons la sélectionner, puis l’encoder en URL avec le <code>Ctrl + U</code>raccourci pour sécuriser son envoi. Ce processus est illustré dans le GIF ci-dessous :</p>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>

