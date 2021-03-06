<h5><a href="http://bensoft.de/projects/acis">Visit my webpage! (documentation, demo, etc.)</a></h5>
<h1>ACIS</h1>
						<h2>Contents</h2>
						<ul>
						<li><a href="#whatisacis">What is ACIS?</a></li>
						<li><a href="#whoisacisfor">Who is ACIS for?</a></li>
						<li><a href="#howdoesitwork">How does it work?</a></li>
						<li><a href="#whatdoesittake">What does it take?</a></li>
						<li><a href="#wherecanigetit">Where can I get it?</a></li>
						<li><a href="#getstarted">Get started</a></li>
						<li><a href="#samples">Samples and tutorials</a></li>
						<li><a href="#documentation">Documentation</a></li>
						</ul>
						<h2 id="whatisacis" >What is ACIS?</h2>
						<p>ACIS stands for <b>A</b>dvanced <b>C</b>ommunication and <b>I</b>nteraction <b>S</b>ystem and is a library written in Java which can be used for speech interaction. The design of the library allows interaction in a very natural way.<br>The ACIS library can be used to create a personal assistant like Google Home or Amazon Echo but it is on the programmers behalf how it behaves and what actions are provided.</p>
						<h2 id="whoisacisfor">Who is ACIS for?</h2>
						<p>The ACIS library is for people who want to do their own thing, who do not want to rely on the possibilities the other assitant manufacturers provide. Because the ACIS library handles everything locally, there are no security or privacy problems.<br>
						Of course a minimum knowledge in programming (Java) is required, but the library itself as well as the sample implementations should be easy to understand.</p>
						<h2 id="howdoesitwork">How does it work? (short version)</h2>
						<p>Basically any ACIS system consists of two main parts - a language-dependent and a language-independent part. Between these two parts is a standardized interface both can use. The language-dependent part is the language the system uses. It delivers language specific information e.g. about words and the sentence objects. The language-independent part uses this information to provide results, even while natural interaction. In fact, the ACIS library is applicable for any language. The only thing needed is a language interface.</p>
						<h2 id="whatdoesittake">What does it take?</h2>
						<p>Basically only a computer capable of running Java programs is required to create something using the ACIS library. To create your own actions, a Java IDE is recommended.<br>
						To create a personal assistant you have no limits - the reference implementation is on a Raspberry Pi3 running Android Things but you can run it on anything. Just add what is needed - a microphone, a speaker, a sound card if needed, a display if you want, a temperature sensor or whatever you can imagine.</p>
						<h2 id="wherecanigetit">Where can I get it?</h2>
						<p>The code of ACIS is publicly available on my <a href="https://github.com/bensoftde">GitHub</a>. It is published under MIT license. If you do not want to clone the repository, a pre-built .jar file is in the root of the master branch.</p>
						<h2 id="getstarted">Get started</h2>
						<p>
						<table class="bordered">
						<tr><td><a href="https://github.com/bensoftde/acis/tree/master/de/bensoft/acis/core">core</a></td><td>The core system.</td></tr>
						<tr><td><a href="https://github.com/bensoftde/acis/tree/master/de/bensoft/acis/server">server</a></td><td>A simple HTTP server which can be used to interact with a device.</td></tr>
						<tr><td><a href="https://github.com/bensoftde/acis/tree/master/de/bensoft/acis/utils">utils</a></td><td>Contains common utilities used by other packages.</td></tr>
						<tr><td><a href="https://github.com/bensoftde/acis/tree/master/de/bensoft/acis/languages">languages</a></td><td>Contains some language interfaces for ACIS. The <a href="https://github.com/bensoftde/acis/blob/master/de/bensoft/acis/languages/Unified.java"><i>Unified</i></a> language interface can be used with any language. Note: German and English are available in high-quality mode. Please <a href="mailto:code@bensoft.de">contact</a> me if you want to contribute a language interface.</td></tr>
						<tr><td><a href="https://github.com/bensoftde/acis/tree/master/samples">samples</a></td><td>Contains samples, code snippets and implementation examples. An Android client app which can be used to send requests to the default server interface provided by the <a href="https://github.com/bensoftde/acis/blob/master/de/bensoft/acis/server/contexts/SampleRequestHandler.java">SampleRequestHandler</a> can be found <a href="https://github.com/bensoftde/acis/tree/master/samples/client_app">here</a>.</td></tr>
						</table>
						<br>
						A pre-built .jar file is in the root of the master branch.
						</p>
						<h2 id="samples">Samples and tutorials</h2>
						<p><ul>
						<li><a href="https://github.com/bensoftde/acis/blob/master/samples/SampleImplementation.java">Sample implementation. Contains how to create/add ActionPackages/Actions with single/multiple trigger and/or context. Also how to set up a server. Best way of implementation for a personal assistant is probably through</a> <a href="https://developer.android.com/things">AndroidThings</a></li>
						<li><a href="https://github.com/bensoftde/acis/tree/master/de/bensoft/acis/server/contexts">Sample ServerContexts</a></li>
						<li><a href="https://github.com/bensoftde/acis/blob/master/de/bensoft/acis/languages/BensoftGermanWiktionary.java">Sample language interface for German:</a> See de.bensoft.acis.core.language <a href="http://bensoft.de/projects/acis/documentation#scrolled">documentation</a> too</li>
						<li><a href="https://github.com/bensoftde/acis/tree/master/samples/android_things">Sample implementation on the</a> <a href="https://developer.android.com/things">AndroidThings platform.</a></li>
						</ul>
						</p>
						<p>
						<h2 id="documentation"><a href="http://bensoft.de/projects/acis/documentation#scrolled">Whole library documentation</a></h2>
						</p>
