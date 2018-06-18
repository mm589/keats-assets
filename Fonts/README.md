<style>
.tooltip {
    position: relative;
    display: inline-block;
    border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
    visibility: hidden;
    width: 120px;
    background-color: #555;
    color: #fff;
    text-align: center;
    border-radius: 6px;
    padding: 5px 0;
    position: absolute;
    z-index: 1;
    bottom: 125%;
    left: 50%;
    margin-left: -60px;
    opacity: 0;
    transition: opacity 0.3s;
}

.tooltip .tooltiptext::after {
    content: "";
    position: absolute;
    top: 100%;
    left: 50%;
    margin-left: -5px;
    border-width: 5px;
    border-style: solid;
    border-color: #555 transparent transparent transparent;
}

.tooltip:hover .tooltiptext {
    visibility: visible;
    opacity: 1;
}
</style>
<h3>King's Corporate Fonts</h3>
<p style="font-size: 14px, sans-serif;">For more information please consult the <a href="https://internal.kcl.ac.uk/erd/depts/brand/Visual-Identity/Fonts.aspx" target="_self"><u>King's Corporate Fonts</u></a> webpage and make sure that the most recent version of the corporate fonts is being used. The font package, including the .ttf, .oet and .woff files can be downloaded from that page. <div class="tooltip">Since almost all browsers support <span class="tooltiptext"><code>.ttf</code> and <code>.woff</code></span>, you may link or <code>@font-face</code> to those two primary file formats.</p></div>
<h4>Linking or <code>@font-face</code> to the King's Corporate fonts</h4>
<ol>
<li><p style="font-size: 14px, sans-serif;">Download the font family package from the King's Corporate Fonts page;</li>
<li>Upload to your GitHub or other repository and serve each individual font package/file <i>separately</i>, i.e. do not link to the entire font package directory or folder;</li>
<li>On your KEATS pages, reference each individual font separately in your HTML code. You may reference the font format using inline CSS and <code><style></code> tags or use @-rules.</p></li>
</ol>

<strong>For <code>@font-face</code>,</strong>
<blockquote>
<code>
@font-face { 
font-family: 'BureauGrotesqueThreeSeven'
src:  url(repository path for your .woff font file) format('woff'),
      url(repository path for your .ttf font file) format('truetype');
}
</code>
</blockquote>

<strong>To link to your font formats in the head of your HTML code,</strong>
<blockquote>
<code>
link rel="stylesheet" href="repository path to your woff font format.woff">
</code>
</blockquote>

For reference, <code>.woff</code> is for Web Open Font Formats and <code>.ttf</code> is for TrueType font formats. Other font formats that are supported include <code>.eot</code> for Embedded OpenType fonts, which are a compact form of OpenType fonts designed and only supported by Microsoft IE.
