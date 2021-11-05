---

layout: col-generic
title: Global Board and Staff
permalink: /corporate/

---

The OWASP Foundation Global Board is comprised of seven elected members who serve for two-year terms. Each Fall, membership votes to elect new leadership for the Foundation. Generally our Board meets monthly and meetings are open to the public. The Global Board sets the strategic direction of the Foundation, its policies, and sets governance and leadership roles. The [Global Board Home Page](/www-board/) has information about upcoming meetings, former meeting minutes, Board decisions, contact information, and other general information. 


<h2>Board of Directors</h2>

<section id="board" class="corporate">
<div>	
 {% for member in site.data.board %}
    <div class="member-container">
        <div class="member-img-container">	
            <div class="member-img" style="background-image: url(/assets/images{{ member.image }});">
            </div>
        </div>
        <div class="member-caption"><h2>{{ member.name }}</h2><hr><strong>{{ member.title }}</strong><br/>
        <div class="member-location">{{member.location}}</div></div><br/>
        <div class="member-info">{{ member.description }} Current Term Ends {{ member.term-ends}}.</div>	
    </div>
    <div style="height:18px;"></div>
{% endfor %}	
</div>
</section>

<h2>Staff</h2>
<p>
Under the direction of the Executive Director, staff implements programs and policies of the Foundation while collaborating with members on OWASP Projects, Chapters, Events, and initiatives.</p>
<p>
Each year the staff works with the Global Board to establish an <a href="https://owasp.org/www-staff/operating-plan/info">Operating Plan</a> and Budget. The work efforts of our staff are tracked publicly at the <a href="/www-staff/operating-plan/status-2021">Operating Plan Status</a>.
</p>

<section id="staff" class="corporate">
<div>	
 {% for member in site.data.staff %}
    <div class="member-container">
        <div class="member-img-container">	
            <div class="member-img" style="background-image: url(/assets/images{{ member.image }});">
            </div>
        </div>
        <div class="member-caption"><h2>{{ member.name }}</h2><hr><strong>{{ member.title }}</strong><br/><div class="member-location">{{member.location}}</div></div><br/>
        <div class="member-info">{{ member.description }}</div>	
    </div>
    <div style="height:18px;"></div>
{% endfor %}	
</div>
</section>


