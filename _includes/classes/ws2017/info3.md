
<ul class="nav nav-tabs">
{% assign navitems = "Info3-/classes/ws2017/info3/,Schedule-/classes/ws2017/info3/schedule/,Labs-/classes/ws2017/info3/labs/" | split: "," %}
{% for navitem in navitems %}
  <li class="nav-item">
    {% assign n = navitem | split: "-" %}
    <a class="nav-link {% if page.url == n[1] %}active{% endif %}" href="{{ site.baseurl }}{{ n[1] }}">{{ n[0] }}</a>
  </li>
{% endfor %}


<li class="nav-item dropdown">
    <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">External Links</a>
    <div class="dropdown-menu">
      <a class="dropdown-item" href="https://moodle.htw-berlin.de/course/view.php?id=14389">Moodle</a>
      <a class="dropdown-item" href="https://lsf.htw-berlin.de/qisserver/rds?state=wsearchv&search=2&veranstaltung.veranstid=131704">LSF</a>
      <a class="dropdown-item" href="https://lsf.htw-berlin.de/qisserver/rds?state=wplan&act=stg&pool=stg&show=plan&P.vx=kurz&r_zuordabstgv.semvonint=3&r_zuordabstgv.sembisint=3&missing=allTerms&k_abstgv.abstgvnr=231">Semesterstundenplan im LSF</a>
      <a class="dropdown-item" href="https://github.com/htw-imi-info3">Github</a>
    </div>
  </li>
</ul>
