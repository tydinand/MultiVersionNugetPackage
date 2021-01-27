# MultiVersionNugetPackage
Nuget package support multi .net versions (Core)

<h2>Introduction</h2>

<p>Having your own Nuget package using on several projects means maintenance. But you like to follow the newest .net version. NuPkg can be downwards compatible with a few simple adjustments.</p>

<h3>Before you start</h3>

<p>This Article is only written for .net core and newer. &nbsp;</p>

<p>&nbsp;</p>

<h2>Let&#39;s Code</h2>

<p>Just code and see the result.</p>

<h4>Step 1&nbsp;</h4>

<p>Open your Nuget project in VS.</p>

<p>Set your project in the .net version you want to develop in.</p>

<p>Test it.</p>

<h4>Step 2</h4>

<p>Edit your Project file (Right-click on project and choose &quot;Edit project file&quot;)</p>

<p>&nbsp;</p>

<p>Find the &lt;TargetFramework&gt; tag and change both to &lt;TargetFrameworks&gt;.</p>

<p>Add your desired extra framework seperated by &quot;;&quot; as value to the existing value.&nbsp;</p>

<pre>
 &lt;TargetFrameworks&gt;net5.0;netcoreapp3.1&lt;/TargetFrameworks&gt;</pre>

<p>&nbsp;</p>

<h4>Step 3</h4>

<p>Save it all.</p>

<p>Reload all your projects. (project ,right-click, unload&nbsp;project, right-click, load project)</p>

<p>Test it.&nbsp; Add it to a&nbsp;project with the added .net version</p>

<p>&nbsp;</p>

<h4>Finished</h4>

<p>&nbsp;</p>

<h3>Notes</h3>

<ul>
	<li>The right&nbsp;SDK must be installed naturaly.</li>
	<li>This <a href="https://docs.microsoft.com/en-us/dotnet/standard/frameworks#how-to-specify-target-frameworks">LIST</a>&nbsp;gives you an overview of the frameworks supported and standarized.&nbsp;</li>
	<li>Remember that a big standard is netstandard 2.0 for net48 and onder versions.</li>
	<li>Be sure you reloaded your projects, it saves you a headache&nbsp;</li>
</ul>

<p>Good luke.</p>

<p>Dinand</p>

