<h2>Project Description</h2>

Aim of this project is to extend the capability of JasperReports to support rendering of Indic scripts in PDF Export using OpenOffice library. JasperReports currently uses iText pdf engine to export reports into PDF, which does not support correct rendering of Indic Scripts. Indic-Jasper is able to correctly render Indic Scripts in PDF export by generating an intermediate ODT file which is converted to PDF using OpenOffice.org library.

<h3>Installation</h3>
<ul>
<blockquote><li>Download the zip from <a href='http://indic-jasper.googlecode.com/files/jasperreports-cdac-ilcg.zip'>http://indic-jasper.googlecode.com/files/jasperreports-cdac-ilcg.zip</a></li>
<li>Unzip the content</li>
<li>Copy the content to SRC folder of the JasperReports</li>
<li>Include required OpenOffice libraries in your class path</li>
<li>Required OpenOffice library files :</li>
<ul>
<blockquote><li>officebean.jar</li>
<li>juh.jar</li>
<li>jurt.jar</li>
<li>ridl.jar</li>
<li>unoil.jar</li>
</blockquote></ul>
<li>Ex: in Linux use the command  <b>export CLASSPATH=$CLASSPATH:/JarFolder/JarFile</b> to set up class path</li></blockquote>

<blockquote><li>Run the command "ant jar" from the root folder of your JasperReport project to re build</li></blockquote>

</ul>

<h3>Usage</h3>
<ul>
<blockquote><li>Setup OPENOFFICE_PATH variable to corresponding path on your machine ex: .../openoffice/program/</li>
<li>In your java application file replace your JRPdfExporter <br>statement <b>import net.sf.jasperreports.engine.export.JRPdfExporter;</b> </br> <br>with <b>import in.cdac.ilcg.jasperreports.pdfexporter.JRPdfExporter;</b> </br> statement in order to generate PDF reports in Indic scripts</li>
<li>Now run your application</li>
</ul></blockquote>

<h3>Links</h3>
<ul>
<blockquote><li><a href='http://jasperforge.org/projects/jasperreports'>JasperReports</a></li>
<li><a href='http://itextpdf.com/'>iText</a></li>
</ul></blockquote>
