---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# The Tree of Tales
{: .wide-block .center .pixel }

The Tree of Tales is a record of winners of the monthly Dark Sphere Pauper League. It began in September 2026. Across a calendar month, the results of weekly pauper tournaments are added up and a winner is decided.
{: .wide-block }

Winners of the league may select one card not already chosen by anyone else to inscribe into The Tree where it will remain for all to see.
{: .wide-block }

## --- --- ---
{: .wide-block .center .pixel .connect-above }

<ol class="middle-block alt" >
{% for post in site.posts %}
    <li class="list-entry" >
        <img src="{{post.image}}" />
        <div>
            <p class="tiny green">{{post.shortdate}} – {{post.winner}} ({{post.points}} points)</p>
            <p class="small">This record marks the winner of the Dark Sphere Pauper League in 
            {{post.englishdate}}. For besting all {{post.possessive}} foes in friendly competition, {{post.winner}} 
            won the right to inscribe the name of one card in the Tree of Tales.
            <br /><br />
            {{post.winner}} chose <span class="caps">{{post.cardname}}</span> to be inscribed. 
            <br /><br />
            Here may all visitors see its mark.</p>
        </div>
    </li>
    <br />
{% endfor %}
<!-- Forever entry -->
    <li class="list-entry" >
        <img src="/assets/images/mrd-285-tree-of-tales.jpeg" />
        <div>
            <p class="tiny green">The lowest ring</p>
            <p class="small">
            This lowest mark on The Tree of Tales marks the beginning of its record.
            <br /><br />
            As it is wished, above this point may all visitors see the marks of those who won before them.
            </p>
        </div>
    </li>
</ol>