
<nav id="navbar" class="collapse navbar-collapse">
    <ul class="nav navbar-nav">
        {% assign links = site.data.navigation %}
        {% for link in links %}
            {% assign class = nil %}
            {% if page.url contains link.url %}
                {% assign class = 'active' %}
            {% endif %}
            {% if link.sublinks %}
                <li class="dropdown {{ class }}">
                    <a href="{{ site.url }}{{ site.baseurl }}{{ link.url }}" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">{{ link.title }} <span class="caret"></span></a>
                    <ul class="dropdown-menu">
                        {% for sublink in link.sublinks %}
                            {% if sublink.title == 'separator' %}
                                <li role="separator" class="divider"></li>
                            {% else %}
                                <li>
                                    <a href="{{ site.url }}{{ site.baseurl }}{{ sublink.url }}">{{ sublink.title }}</a>
                                </li>
                            {% endif %}
                        {% endfor %}
                    </ul>
                </li>
            {% else %}
                <li class="{{ class }}">
                    <a href="{{ site.url }}{{ site.baseurl }}{{ link.url }}">{{ link.title }}</a>
                </li>
            {% endif %}
        {% endfor %}
    </ul>
</nav>

<h1>Domeinspecifieke leerresultaten</h1>
  <p>1. De professionele bachelor TI analyseert een probleem, vertaalt dit naar een ITcontext en geeft de informatiebehoeften van een organisatie gestructureerd weer
    door gebruik te maken van analyse- en modelleringstechnieken.</p>
  <p>
2. De professionele bachelor TI verzamelt en verwerkt proces- en datagegevens,
slaat ze op en stelt ze ter beschikking, zodanig dat deze op een correcte en
efficiënte manier kunnen worden opgevraagd.
  </p>
    <p>
3. De professionele bachelor TI ontwerpt, bouwt, documenteert en test kwalitatieve
IT oplossingen.
  </p>
  <p>
4. De professionele bachelor TI installeert, configureert, beveiligt, onderhoudt en
ondersteunt IT-oplossingen en past ze indien nodig aan zodat ze blijven
beantwoorden aan de veranderende behoeften van een organisatie.
  </p>
  <p>
5. De professionele bachelor TI handelt deontologisch en maatschappelijk
verantwoord, conform bedrijfs- en organisatiecontext, regelgeving, best practices en
strategieën vanuit eigen inzicht en kennis.
  </p>
  <p>
6. De professionele bachelor TI onderzoekt en evalueert kritisch bestaande en
innovatieve IT-oplossingen.
  </p>
  <p>
7. De professionele bachelor TI geeft advies over IT-oplossingen, -producten, -
diensten en –technologieën voor verschillende domeinen en/of sectoren.
  </p>
  <p>
8. De professionele bachelor TI kan zelfstandig en in een multidisciplinair en/of
multicultureel team een opdracht op projectmatige wijze aanpakken. De
professionele bachelor TI kan eenvoudig leidinggevende taken uitvoeren en een
projectplan ontwerpen, interpreteren, uitvoeren, aanpassen en toelichten.
  </p>
  <p>
9. De professionele bachelor TI communiceert minstens in het Nederlands en het
Engels, mondeling en schriftelijk aangepast aan het doelpubliek.
  </p>
  <p>
10. De professionele bachelor TI houdt rekening met en handelt naar de internationale
context van het vakgebied.
  </p>
  <p>
11. De professionele bachelor TI is ondernemend, neemt initiatief en reageert op nieuwe
ontwikkelingen en toepassingsdomeinen.
  </p>
  <p>
12. De professionele bachelor TI ondersteunt veranderingsprocessen bij ingebruikname
van IT-oplossingen.
  </p>
  </p>
</body>
