<h3>King's Corporate Fonts</h3>
<p style="font-size: 14px, sans-serif;">For more information please consult the <a href="https://internal.kcl.ac.uk/erd/depts/brand/Visual-Identity/Fonts.aspx" target="_self"><u>King's Corporate Fonts</u></a> webpage and make sure that the most recent version of the corporate fonts is being used. The font package, including the .ttf, .oet and .woff files can be downloaded from that page. Since almost all browsers support <code>.ttf</code> and <code>.woff</code>, you may link or <code>@font-face</code> to those two primary file formats.</p>
<h4>Linking or <code>@font-face</code> to the King's Corporate fonts</h4>
<ol>
      <li><p style="font-size: 14px, sans-serif;"><b>If starting with new font files:</b> Download the font family package from the King's Corporate Fonts page, which is stored on the King's Digital Assets repository;</li>
<li>Upload to your GitHub or other repository and serve each individual font package/file <i>separately</i>, i.e. do not link to the entire font package directory or folder;</li>
<li>On your KEATS pages, reference each individual font separately in your HTML code. You may reference the font format using inline CSS, <code><style></code> tags and @-rules.</p></li>
      <li><b>If using the currently available font files in this repository:</b> The font files (archived and current as of 2018) are available in this repository, so you can serve each file using the current URL in KEATS, or if that's no longer practical, use a CDN of your choice, e.g. RawGit to serve the files again.</li>
</ol>

<strong>To use <code>@font-face</code>,</strong>
<blockquote>
<code>
@font-face { 
font-family: 'BureauGrotesqueThreeSeven';
src:  url(repository path for your .woff font file.woff) format('woff'),
      url(repository path for your .ttf font file.ttf) format('truetype');
}
</code>
</blockquote>

For reference, <code>.woff</code> is for Web Open Font Formats and <code>.ttf</code> is for TrueType font formats. Other font formats that are supported include <code>.eot</code> for Embedded OpenType fonts, which are a compact form of OpenType fonts designed and only supported by Microsoft IE. To ensure acceptable font use on IE, ensure you include the alternative fonts, i.e. Impact and Georgia.

<strong>To reference the font in your CSS stylesheet for a certain <code>p</code> element,</strong>
<br>
<code>p { font-family: 'BureauGrotesqueThreeSeven', Impact, sans-serif; }</code>

For HTML, <code><p style="font-family: BureauGrotesqueThreeSeven";></code>

<h4>Acceptable font alternatives for web browser compatibility</h4>
The acceptable alternative font for Bureau Grotesque 37 is Impact, for Kings Caslon Display (or Kings Caslon Text) it is Georgia regular. Reference the King's Corporate Fonts <a href="https://internal.kcl.ac.uk/erd/depts/brand/Documents/Branding-essentials.pdf" target="_self"><u>Branding Essentials</u></a> document for more information.
