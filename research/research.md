<h3 class="masthead-title">
<!-- <a href="/" title="Home">{{ site.title }}</a> -->
<a href="/" title="Home">Home</a>


{% for page in site.pages_list %}
  &nbsp;&nbsp;&nbsp;
  <a href="{{ page[1]  }}">{{ page[0] }}</a>
{% endfor %}
</h3>

## Adaptive Autonomous Modification of Unstructured Environments

Proposed methods to perform autonomous construction in irregular terrain and designed a heterogeneous robotic system that allows effective evaluation of these methods at a physical implementation level. The heterogeneous robotic team is composed of two autonomous robots that are able to manipulate material of different physical properties (rigid and amorphous materials)

<iframe width="560" height="315" src="https://www.youtube.com/embed/PXaKOsIyeo8?start=11" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>

### Multi-Robot and Multi-Material (Rigid and Compliante)

<iframe width="560" height="315" src="https://www.youtube.com/embed/xAjEsM_ePN4?start=3" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>

### Single Robot and Amorphous/Compliate Material
<br/>
We use the notion of  _navigability_ to enable a robot to modify its environment and provide access to areas which were initially unreachable. In this model, the motion ability of a mobile platform over unstructured terrain is expressed in terms of three scalar parameters that can provide a conservative lower bound of the motion ability based on the stability and clearance constraints of an arbitrary mobile platform.  We used a _deposition_ _model_ that provides an upper bound of how much the environment changes in response to its actions. Together, the navigability and deposition model allow the robot to adaptively synthesize low-level motion and manipulation plans that are guaranteed to produce navigable structures as long as the environmental changes produced by the robots are consistent with the deposition model at each step. Navigability parameters induce lower bounds on both the allowable deposition models and sensing abilities of a robot. This abstract model for the construction process directly links the motion, sensing, and manipulation abilities of a robot. 
<br/>
<iframe width="560" height="315" src="https://www.youtube.com/embed/7tjbrfLna8A?start=11" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
