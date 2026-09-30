---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# The Tree of Tales
{: .wide-block .center .pixel }

The Tree of Tales is a record of winners of the Dark Sphere Pauper League.
{: .middle-block }

<br />

<ol class="wide-block alt" >
{% for post in site.posts %}
    <li class="list-entry" >
        <img src="{{post.image}}" />
        <div>
            <p class="tiny green">{{post.shortdate}} – {{post.winner}} ({{post.points}} points)</p>
            <p class="small">This record marks the winner Dark Sphere Pauper League in 
            {{post.englishdate}}. For besting all their foes in friendly competition, {{post.winner}} won the right to inscribe the name of one card in the Tree of Tales.
            <br /><br />
            {{post.winner}} chose <span class="caps">{{post.cardname}}</span> to be inscribed. 
            <br /><br />
            Here may all visitors see its mark.</p>
        </div>
    </li>
    <br />
{% endfor %}
</ol>