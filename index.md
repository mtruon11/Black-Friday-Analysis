<html>
<head><meta charset="utf-8" />
<title>Black-Friday-Analysis</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>

<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    color: #000 !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.2.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.2.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.2.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.2.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.2.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.2.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=1);
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2);
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1);
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1);
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
@media (max-width: 991px) {
  #ipython_notebook {
    margin-left: 10px;
  }
}
[dir="rtl"] #ipython_notebook {
  float: right !important;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#login_widget {
  float: right;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  text-align: center;
  vertical-align: middle;
  display: inline;
  opacity: 0;
  z-index: 2;
  width: 12ex;
  margin-right: -12ex;
}
.alternate_upload .btn-upload {
  height: 22px;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
[dir="rtl"] #tabs li {
  float: right;
}
ul#tabs {
  margin-bottom: 4px;
}
[dir="rtl"] ul#tabs {
  margin-right: 0px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons {
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-right {
  padding-top: 1px;
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-left {
  float: right !important;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: baseline;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
#tree-selector {
  padding-right: 0px;
}
[dir="rtl"] #tree-selector a {
  float: right;
}
#button-select-all {
  min-width: 50px;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
[dir="rtl"] #new-menu {
  text-align: right;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
[dir="rtl"] #running .col-sm-8 {
  float: right !important;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI colors. */
.ansibold {
  font-weight: bold;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  border-left-width: 1px;
  padding-left: 5px;
  background: linear-gradient(to right, transparent -40px, transparent 1px, transparent 1px, transparent 100%);
}
div.cell.jupyter-soft-selected {
  border-left-color: #90CAF9;
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected {
  border-color: #ababab;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 5px, transparent 5px, transparent 100%);
}
@media print {
  div.cell.selected {
    border-color: transparent;
  }
}
div.cell.selected.jupyter-soft-selected {
  border-left-width: 0;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 7px, #E3F2FD 7px, #E3F2FD 100%);
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #66BB6A -40px, #66BB6A 5px, transparent 5px, transparent 100%);
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  padding: 0.4em;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. We need the 0 value because of how we size */
  /* .CodeMirror-lines */
  padding: 0;
  border: 0;
  border-radius: 0;
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul {
  list-style: disc;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ul ul {
  list-style: square;
  margin: 0em 2em;
}
.rendered_html ul ul ul {
  list-style: circle;
  margin: 0em 2em;
}
.rendered_html ol {
  list-style: decimal;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
  margin: 0em 2em;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  background-color: #fff;
  color: #000;
  font-size: 100%;
  padding: 0px;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: 1px solid black;
  border-collapse: collapse;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  border: 1px solid black;
  border-collapse: collapse;
  margin: 1em 2em;
}
.rendered_html td,
.rendered_html th {
  text-align: left;
  vertical-align: middle;
  padding: 4px;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget {
  float: right !important;
  float: right;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  margin-top: 6px;
}
span.save_widget span.filename {
  height: 1em;
  line-height: 1em;
  padding: 3px;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  display: none;
}
.command-shortcut:before {
  content: "(command)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>
<style type="text/css">
    
/* Temporary definitions which will become obsolete with Notebook release 5.0 */
.ansi-black-fg { color: #3E424D; }
.ansi-black-bg { background-color: #3E424D; }
.ansi-black-intense-fg { color: #282C36; }
.ansi-black-intense-bg { background-color: #282C36; }
.ansi-red-fg { color: #E75C58; }
.ansi-red-bg { background-color: #E75C58; }
.ansi-red-intense-fg { color: #B22B31; }
.ansi-red-intense-bg { background-color: #B22B31; }
.ansi-green-fg { color: #00A250; }
.ansi-green-bg { background-color: #00A250; }
.ansi-green-intense-fg { color: #007427; }
.ansi-green-intense-bg { background-color: #007427; }
.ansi-yellow-fg { color: #DDB62B; }
.ansi-yellow-bg { background-color: #DDB62B; }
.ansi-yellow-intense-fg { color: #B27D12; }
.ansi-yellow-intense-bg { background-color: #B27D12; }
.ansi-blue-fg { color: #208FFB; }
.ansi-blue-bg { background-color: #208FFB; }
.ansi-blue-intense-fg { color: #0065CA; }
.ansi-blue-intense-bg { background-color: #0065CA; }
.ansi-magenta-fg { color: #D160C4; }
.ansi-magenta-bg { background-color: #D160C4; }
.ansi-magenta-intense-fg { color: #A03196; }
.ansi-magenta-intense-bg { background-color: #A03196; }
.ansi-cyan-fg { color: #60C6C8; }
.ansi-cyan-bg { background-color: #60C6C8; }
.ansi-cyan-intense-fg { color: #258F8F; }
.ansi-cyan-intense-bg { background-color: #258F8F; }
.ansi-white-fg { color: #C5C1B4; }
.ansi-white-bg { background-color: #C5C1B4; }
.ansi-white-intense-fg { color: #A1A6B2; }
.ansi-white-intense-bg { background-color: #A1A6B2; }

.ansi-bold { font-weight: bold; }

    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><img src="blackfriday.png" alt="title"></p>
<h1 id="Advertisements-On-Black-Friday">Advertisements On Black Friday<a class="anchor-link" href="#Advertisements-On-Black-Friday">&#182;</a></h1><h5 id="Minh-Truong,-Yunhan-Bai,-David-Hood">Minh Truong, Yunhan Bai, David Hood<a class="anchor-link" href="#Minh-Truong,-Yunhan-Bai,-David-Hood">&#182;</a></h5><h3 id="-----------------------------------------------------------------------------------------------------------------------------------------------------------------">-----------------------------------------------------------------------------------------------------------------------------------------------------------------<a class="anchor-link" href="#-----------------------------------------------------------------------------------------------------------------------------------------------------------------">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Table-Of-Contents:">Table Of Contents:<a class="anchor-link" href="#Table-Of-Contents:">&#182;</a></h1><ul>
    <li><a href="#intro">Introduction</a></li>
    <li><a href="#1">Get Started With Data</a>
        <ul>
            <li> <a href="#library">Libraries</a></li>
            <li><a href="#source">Data Source</a></li>
            <li><a href="#reading">Reading Data</a></li>
        </ul>
    </li>
    <li><a href="#2">Tidying and Modifying Data</a>
        <ul>
            <li> <a href="#missingdata">Handle Missing Data</a></li>
            <li><a href="#melting">Melting Data</a></li>
        </ul>
    </li>
    <li><a href="#3">Exploratory Data Analysis (EDA)</a>
        <ul>
            <li><a href="#4">Gender</a></li>
            <li><a href="#5">Age</a></li>
            <li><a href="#sum">Sum Purchases</a></li>
            <li><a href="#6">Frequency Purchase</a></li>
            <li><a href="#citycategory">City Category</a></li>
            <li><a href="#7">Top 5 Selling</a></li>
            <li><a href="#8">Product Category</a></li>
        </ul>
    </li>
    <li><a href="#hypothesis">Hypothesis Testing</a></li>
    <li><a href="#ANOVA">Analysis of Variance</a></li>
    <li><a href="#9">Linear Regression</a></li>
    <li><a href="#10">Logistic Regression</a></li>
    <li><a href="#conclusion">Conclusion</a></li>
</ul>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Introduction"><section id="intro">Introduction</section><a class="anchor-link" href="#Introduction">&#182;</a></h1><p><br>
The <mark>first recorded use</mark> of the term “Black Friday” was applied not to holiday shopping but to <a href="https://www.history.com/news/whats-the-real-history-of-black-friday">financial crisis</a>: specifically, the crash of the U.S. gold market on September 24, 1869. Two notoriously ruthless Wall Street financiers, Jay Gould and Jim Fisk, worked together to buy up as much as they could of the nation’s gold, hoping to drive the price sky-high and sell it for astonishing profits. On that Friday in September, the conspiracy finally unraveled, sending the stock market into free-fall and bankrupting everyone from Wall Street barons to farmers.
<br><br>
<mark>In recent years</mark>, another myth has surfaced that gives a particularly ugly twist to the tradition, claiming that back in the 1800s Southern plantation owners could buy slaves at a discount on the day after Thanksgiving. Though this version of Black Friday’s roots has understandably led some to call for a boycott of the retail holiday, it has no basis in fact.
<br><br>
The <strong>"Black Friday"</strong> we know today is a much happier occasion then the two above... <br></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><img src="Crazybf2.png" width="600" height="300"/></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><br>though, maybe just as violent. After the pumpkin pie, families all over America make there way to their local retailers to spend absurd amounts of money for the upcoming holiday season.
<br><br>
In this tutorial, our <mark>goal</mark> is to advertise the right products to the right people. As an advertising agency, our strategy is to learn different behaviors of customers on Black Friday to see what they really like and what they would like to buy on Black Friday. Also, we want to learn from the past purchases to recognize the pattern and likelihood in a certain group of people in order to increase the profit on Black Friday. Moreover, we would like to know which product categories are purchased the most and by which groups of people has bought the most for that particular product category.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="-Getting-Started-with-the-Data"><section id="1"> Getting Started with the Data</section><a class="anchor-link" href="#-Getting-Started-with-the-Data">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Importing-Libraries"><section id="library">Importing Libraries</section><a class="anchor-link" href="#Importing-Libraries">&#182;</a></h2><p>We make use of Python 3 along with a few imported libraries: <a href="http://pandas.pydata.org/pandas-docs/stable/">pandas</a>, <a href="http://www.numpy.org/">numpy</a>, <a href="https://matplotlib.org/tutorials/index.html">matplotlib</a>, <a href="https://scikit-learn.org/stable/">scikit-learn</a>, <a href="https://seaborn.pydata.org/">seaborn</a>, and more.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Suppress FutureWarning</span>
<span class="kn">import</span> <span class="nn">warnings</span>
<span class="n">warnings</span><span class="o">.</span><span class="n">simplefilter</span><span class="p">(</span><span class="n">action</span><span class="o">=</span><span class="s1">&#39;ignore&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="ne">FutureWarning</span><span class="p">)</span>
<span class="c1"># Necessary libraries and imports to complete this tutorial</span>
<span class="kn">import</span> <span class="nn">re</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span>
<span class="kn">import</span> <span class="nn">statsmodels.api</span> <span class="k">as</span> <span class="nn">sm</span>
<span class="kn">from</span> <span class="nn">scipy</span> <span class="k">import</span> <span class="n">stats</span>
<span class="kn">from</span> <span class="nn">scipy.stats</span> <span class="k">import</span> <span class="n">f</span>
<span class="kn">from</span> <span class="nn">statsmodels.formula.api</span> <span class="k">import</span> <span class="n">ols</span>
<span class="kn">from</span> <span class="nn">sklearn</span> <span class="k">import</span> <span class="n">linear_model</span><span class="p">,</span> <span class="n">preprocessing</span><span class="p">,</span> <span class="n">model_selection</span>
<span class="kn">from</span> <span class="nn">sklearn.cross_validation</span> <span class="k">import</span> <span class="n">train_test_split</span>
<span class="kn">from</span> <span class="nn">sklearn.metrics</span> <span class="k">import</span> <span class="n">classification_report</span><span class="p">,</span> <span class="n">accuracy_score</span><span class="p">,</span> <span class="n">mean_squared_error</span><span class="p">,</span> <span class="n">r2_score</span>
<span class="kn">from</span> <span class="nn">sklearn.model_selection</span> <span class="k">import</span> <span class="n">KFold</span>
<span class="kn">from</span> <span class="nn">mpl_toolkits.mplot3d</span> <span class="k">import</span> <span class="n">Axes3D</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stderr output_text">
<pre>C:\Users\truon\Anaconda3\lib\site-packages\sklearn\cross_validation.py:41: DeprecationWarning: This module was deprecated in version 0.18 in favor of the model_selection module into which all the refactored classes and functions are moved. Also note that the interface of the new CV iterators are different from that of this module. This module will be removed in 0.20.
  &#34;This module will be removed in 0.20.&#34;, DeprecationWarning)
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Data-Source"><section id="source">Data Source</section><a class="anchor-link" href="#Data-Source">&#182;</a></h2><p>Dataset of 550 000 observations about the black Friday in a retail store, it contains different kinds of variables either numerical or categorical. It contains missing values.
<br><br> Kaggle dataset <a href="https://www.kaggle.com/mehdidag/black-friday">here</a></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Reading-the-data"><section id="reading">Reading the data</section><a class="anchor-link" href="#Reading-the-data">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">blackfriday</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="s2">&quot;blackfriday.csv&quot;</span><span class="p">)</span>
<span class="c1">#Making Mean_age so for graphing in later sections</span>
<span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Mean_age&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">map</span><span class="p">({</span><span class="s1">&#39;0-17&#39;</span><span class="p">:</span> <span class="mf">8.5</span><span class="p">,</span> <span class="s1">&#39;18-25&#39;</span><span class="p">:</span> <span class="mf">21.5</span><span class="p">,</span><span class="s1">&#39;26-35&#39;</span><span class="p">:</span> <span class="mf">30.5</span><span class="p">,</span> <span class="s1">&#39;36-45&#39;</span><span class="p">:</span> <span class="mf">40.5</span><span class="p">,</span><span class="s1">&#39;46-50&#39;</span><span class="p">:</span> <span class="mi">48</span><span class="p">,</span> <span class="s1">&#39;51-55&#39;</span><span class="p">:</span> <span class="mi">53</span><span class="p">,</span> <span class="s1">&#39;55+&#39;</span><span class="p">:</span> <span class="mf">67.5</span><span class="p">})</span>
<span class="c1">#Modify the &quot;Stay_In_Current_City_Years&quot; column, so assume that anyone that live more than 4 years is just 4 years.</span>
<span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Stay_In_Current_City_Years&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Stay_In_Current_City_Years&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">map</span><span class="p">({</span><span class="s1">&#39;0&#39;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s1">&#39;1&#39;</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="s1">&#39;2&#39;</span><span class="p">:</span> <span class="mi">2</span><span class="p">,</span> <span class="s1">&#39;3&#39;</span><span class="p">:</span> <span class="mi">3</span><span class="p">,</span><span class="s1">&#39;4+&#39;</span><span class="p">:</span> <span class="mi">4</span><span class="p">})</span>
<span class="n">blackfriday</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[2]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Product_ID</th>
      <th>Gender</th>
      <th>Age</th>
      <th>Occupation</th>
      <th>City_Category</th>
      <th>Stay_In_Current_City_Years</th>
      <th>Marital_Status</th>
      <th>Product_Category_1</th>
      <th>Product_Category_2</th>
      <th>Product_Category_3</th>
      <th>Purchase</th>
      <th>Mean_age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1000001</td>
      <td>P00069042</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>8370</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1000001</td>
      <td>P00248942</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>6.0</td>
      <td>14.0</td>
      <td>15200</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1000001</td>
      <td>P00087842</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>12</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1422</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1000001</td>
      <td>P00085442</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>12</td>
      <td>14.0</td>
      <td>NaN</td>
      <td>1057</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1000002</td>
      <td>P00285442</td>
      <td>M</td>
      <td>55+</td>
      <td>16</td>
      <td>C</td>
      <td>4</td>
      <td>0</td>
      <td>8</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>7969</td>
      <td>67.5</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>In the above dataset, there are 12 columns in total. We have: <br>
Column 1: User_ID <br>
Column 2: Product_ID  <br>
Column 3: Gender (Male and Female) <br>
Column 4: Age (Age in bins) <br>
Column 5: Occupation <br>
Column 6: City_Category (A, B, C) <br>
Column 7: Stay_In_Current_City_Years (Number of years stay in current city) <br>
Column 8: Marital_Status (0 for single, 1 for married) <br>
Column 9: Product_Category_1 <br>
Column 10: Product_Category_2 <br>
Column 11: Product_Category_3 <br>
Column 12: Purchase (Purchase amount in Dollars) <br>
Column 13: Mean_Age (mean of the age bins)<br>
<br>
A product can belong to many different categories.<br></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Display some basic statistic about the dataset. Since summary statistics are used in the pandas describe() method, only the columns with quantitative data are displayed. There are 537577 purchases made in the dataset.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">blackfriday</span><span class="o">.</span><span class="n">describe</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[3]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Occupation</th>
      <th>Stay_In_Current_City_Years</th>
      <th>Marital_Status</th>
      <th>Product_Category_1</th>
      <th>Product_Category_2</th>
      <th>Product_Category_3</th>
      <th>Purchase</th>
      <th>Mean_age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>5.375770e+05</td>
      <td>537577.00000</td>
      <td>537577.000000</td>
      <td>537577.000000</td>
      <td>537577.000000</td>
      <td>370591.000000</td>
      <td>164278.000000</td>
      <td>537577.000000</td>
      <td>537577.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>1.002992e+06</td>
      <td>8.08271</td>
      <td>1.859458</td>
      <td>0.408797</td>
      <td>5.295546</td>
      <td>9.842144</td>
      <td>12.669840</td>
      <td>9333.859853</td>
      <td>34.725908</td>
    </tr>
    <tr>
      <th>std</th>
      <td>1.714393e+03</td>
      <td>6.52412</td>
      <td>1.289828</td>
      <td>0.491612</td>
      <td>3.750701</td>
      <td>5.087259</td>
      <td>4.124341</td>
      <td>4981.022133</td>
      <td>12.004781</td>
    </tr>
    <tr>
      <th>min</th>
      <td>1.000001e+06</td>
      <td>0.00000</td>
      <td>0.000000</td>
      <td>0.000000</td>
      <td>1.000000</td>
      <td>2.000000</td>
      <td>3.000000</td>
      <td>185.000000</td>
      <td>8.500000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>1.001495e+06</td>
      <td>2.00000</td>
      <td>1.000000</td>
      <td>0.000000</td>
      <td>1.000000</td>
      <td>5.000000</td>
      <td>9.000000</td>
      <td>5866.000000</td>
      <td>30.500000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>1.003031e+06</td>
      <td>7.00000</td>
      <td>2.000000</td>
      <td>0.000000</td>
      <td>5.000000</td>
      <td>9.000000</td>
      <td>14.000000</td>
      <td>8062.000000</td>
      <td>30.500000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>1.004417e+06</td>
      <td>14.00000</td>
      <td>3.000000</td>
      <td>1.000000</td>
      <td>8.000000</td>
      <td>15.000000</td>
      <td>16.000000</td>
      <td>12073.000000</td>
      <td>40.500000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>1.006040e+06</td>
      <td>20.00000</td>
      <td>4.000000</td>
      <td>1.000000</td>
      <td>18.000000</td>
      <td>18.000000</td>
      <td>18.000000</td>
      <td>23961.000000</td>
      <td>67.500000</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Tidying-and-modifying-the-data"><section id="2">Tidying and modifying the data</section><a class="anchor-link" href="#Tidying-and-modifying-the-data">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="-In-tidy-data:-"><b> In tidy data: </b><a class="anchor-link" href="#-In-tidy-data:-">&#182;</a></h2><p><br> 1. Each variable forms a column.
<br> 2. Each observation forms a row.
<br> 3. Each type of observational unit forms a table.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Handling-missing-data"><section id="missingdata">Handling missing data</section><a class="anchor-link" href="#Handling-missing-data">&#182;</a></h2><p>In our dataset the three columns Product_Category_1,Product_Category_2, and Product_Category_3 represent all the  categories that the puchesed product belongs to. Most products belong to three categories, but some belong to two or less. These columns will have NaN as the value. This will make things difficult when we try to make a category table in the next step. Therefore, we are going to replace NaN with 0 to let to convey that product does not belong to any more categories.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">blackfriday</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">fillna</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
<span class="n">blackfriday</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[4]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Product_ID</th>
      <th>Gender</th>
      <th>Age</th>
      <th>Occupation</th>
      <th>City_Category</th>
      <th>Stay_In_Current_City_Years</th>
      <th>Marital_Status</th>
      <th>Product_Category_1</th>
      <th>Product_Category_2</th>
      <th>Product_Category_3</th>
      <th>Purchase</th>
      <th>Mean_age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1000001</td>
      <td>P00069042</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>3</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>8370</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1000001</td>
      <td>P00248942</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>6.0</td>
      <td>14.0</td>
      <td>15200</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1000001</td>
      <td>P00087842</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>12</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1422</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1000001</td>
      <td>P00085442</td>
      <td>F</td>
      <td>0-17</td>
      <td>10</td>
      <td>A</td>
      <td>2</td>
      <td>0</td>
      <td>12</td>
      <td>14.0</td>
      <td>0.0</td>
      <td>1057</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1000002</td>
      <td>P00285442</td>
      <td>M</td>
      <td>55+</td>
      <td>16</td>
      <td>C</td>
      <td>4</td>
      <td>0</td>
      <td>8</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>7969</td>
      <td>67.5</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Melting-Product-Category-Table"><section id="melting">Melting Product Category Table</section><a class="anchor-link" href="#Melting-Product-Category-Table">&#182;</a></h2><p>Another step in tidying data is to remove variables from column names. <br>For our dataframe, Product_Category_1, Product_Category_2, and Product_Category_3 should be melted into one column.<br>To keep the original dataframe clear and have fewer repeated information, we will create a new dataframe to store Product_Category seperately. <br>The Category of a product can be looked up with its Product_ID in the new dataframe. <br> Several columns are retained for lookups in future analysis.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Create a seperate dataframe to store category infomation</span>
<span class="n">category_table</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="p">[[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="s1">&#39;Age&#39;</span><span class="p">,</span> <span class="s1">&#39;Product_Category_1&#39;</span><span class="p">,</span> <span class="s1">&#39;Product_Category_2&#39;</span><span class="p">,</span> <span class="s1">&#39;Product_Category_3&#39;</span><span class="p">]]</span>
<span class="c1"># Drop Product_Category columns from the original dataframe for neatness</span>
<span class="n">blackfriday</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">drop</span><span class="p">([</span><span class="s1">&#39;Product_Category_1&#39;</span><span class="p">,</span><span class="s1">&#39;Product_Category_2&#39;</span><span class="p">,</span> <span class="s1">&#39;Product_Category_3&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>

<span class="c1"># Melt Product_Category columns in to one</span>
<span class="n">category_table</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">melt</span><span class="p">(</span><span class="n">category_table</span><span class="p">,</span> <span class="n">id_vars</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="s1">&#39;Age&#39;</span><span class="p">],</span> <span class="n">value_vars</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_Category_1&#39;</span><span class="p">,</span> <span class="s1">&#39;Product_Category_2&#39;</span><span class="p">,</span> <span class="s1">&#39;Product_Category_3&#39;</span><span class="p">])</span>
<span class="c1"># Drop any row with value equals to 0 (no category)</span>
<span class="n">category_table</span> <span class="o">=</span> <span class="n">category_table</span><span class="p">[</span><span class="n">category_table</span><span class="o">.</span><span class="n">value</span> <span class="o">!=</span> <span class="mi">0</span><span class="p">]</span>   
<span class="c1"># Drop variable column</span>
<span class="n">category_table</span> <span class="o">=</span> <span class="n">category_table</span><span class="o">.</span><span class="n">drop</span><span class="p">([</span><span class="s1">&#39;variable&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="c1"># Rename value column to Product_Category</span>
<span class="n">category_table</span> <span class="o">=</span> <span class="n">category_table</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">index</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;value&quot;</span><span class="p">:</span> <span class="s2">&quot;Product_Category&quot;</span><span class="p">})</span>
<span class="n">category_table</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[5]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Product_ID</th>
      <th>Age</th>
      <th>Product_Category</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>P00069042</td>
      <td>0-17</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>P00248942</td>
      <td>0-17</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>P00087842</td>
      <td>0-17</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>P00085442</td>
      <td>0-17</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>P00285442</td>
      <td>55+</td>
      <td>8.0</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>For More information about tidying data, you can click this <a href="http://vita.had.co.nz/papers/tidy-data.html">link</a></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Exploratory-Data-Analysis-(EDA)"><section id="3">Exploratory Data Analysis (EDA)</section><a class="anchor-link" href="#Exploratory-Data-Analysis-(EDA)">&#182;</a></h1><h4 id="Four-types-of-EDA">Four types of EDA<a class="anchor-link" href="#Four-types-of-EDA">&#182;</a></h4><ul>
<li>Univariate non-graphical</li>
<li>Multivariate non-graphical</li>
<li>Univariate graphical</li>
<li>Multivariate graphical</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Advantages-of-EDA:">Advantages of EDA:<a class="anchor-link" href="#Advantages-of-EDA:">&#182;</a></h4><ul>
<li>Detection of mistakes</li>
<li>Checking of assumptions</li>
<li>Preliminary selection of appropriate models</li>
<li>Determining relationships among the explanatory variables</li>
<li>Assessing the direction and rough size of relationships between explanatory and outcome variables</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Gender"><section id="4">Gender</section><a class="anchor-link" href="#Gender">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">purchase_by_user</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;User_ID&#39;</span><span class="p">,</span> <span class="s1">&#39;Gender&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span>
<span class="n">purchase_by_user</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">purchase_by_user</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[6]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Gender</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1000001</td>
      <td>F</td>
      <td>333481</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1000002</td>
      <td>M</td>
      <td>810353</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1000003</td>
      <td>M</td>
      <td>341635</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1000004</td>
      <td>M</td>
      <td>205987</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1000005</td>
      <td>M</td>
      <td>821001</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>It is often believed that women spend more than men on Black Friday. To test this myth we made the graph below to observe the total spending of both genders. As the following graph shows, we can see a large difference between male and female spending. However the results are the opposite of what we were lead to expect. The graph below shows that women spend about a third of the amount men do on Black Friday. Myth busted!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">ax</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">purchase_by_user</span><span class="p">[</span><span class="s1">&#39;Gender&#39;</span><span class="p">])</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This gender split is really helpful for retailers and advertising agencies. With this information, retailers could modify their store layout, and product selection to appeal to their larger male consumer base. Advertising agency might want to choose different strategies to advertise products and the whole Black Friday shopping experience based on the gender proportion of their shoppers. They could further appeal to men bye marketing the Black Friday experience in ways that solicit to them. For example, Walmart could hire <a href="https://en.wikipedia.org/wiki/Shaquille_O%27Neal"> Shaquille O'Neal</a> to appear in an ad, boxing out other customers while he gets the products he wants.
<br><br>
However this is just the count of shoppers based on gender. For further investigation, we should look at the average amount, in dollars, spent by each gender.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">male_spending</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="p">[</span><span class="n">purchase_by_user</span><span class="o">.</span><span class="n">Gender</span><span class="o">==</span><span class="s1">&#39;M&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">mean</span><span class="p">()</span>

<span class="n">female_spending</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="p">[</span><span class="n">purchase_by_user</span><span class="o">.</span><span class="n">Gender</span><span class="o">==</span><span class="s1">&#39;F&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">mean</span><span class="p">()</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The average of spending money by male on Black Friday is $&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">male_spending</span><span class="o">.</span><span class="n">Purchase</span><span class="p">))</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The average of spending money by female on Black Friday is $&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">female_spending</span><span class="o">.</span><span class="n">Purchase</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>The average of spending money by male on Black Friday is $911963.1614201183
The average of spending money by female on Black Friday is $699054.0342136854
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, let's visualize the result:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">data</span> <span class="o">=</span> <span class="p">{</span><span class="s1">&#39;Gender&#39;</span><span class="p">:[</span><span class="s2">&quot;Male&quot;</span><span class="p">,</span> <span class="s2">&quot;Female&quot;</span><span class="p">],</span> <span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="p">[</span><span class="n">male_spending</span><span class="o">.</span><span class="n">Purchase</span><span class="p">,</span> <span class="n">female_spending</span><span class="o">.</span><span class="n">Purchase</span><span class="p">]}</span>
<span class="n">avg_spend_by_gender</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">data</span><span class="o">=</span><span class="n">data</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">avg_spend_by_gender</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Gender&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase By Different Gender&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Gender&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase in U.S Dollar&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA5EAAAHwCAYAAAA/5etpAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMS4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvNQv5yAAAIABJREFUeJzs3Xm0ZVV5L+zfS4GCSqOIXhUFkmBUWhUEY2wiuYBGxfaK10RQE9TPqImJicZ8ipjcmNxEoyZBRVA0KnYJwRaNXT6bKIVig6ggoJSgFq3EBkHe74+9jh4qp1lVxT61i3qeMfY4e80111rv3uecUedXc665q7sDAAAAY2y1qQsAAABg8yFEAgAAMJoQCQAAwGhCJAAAAKMJkQAAAIwmRAIAADCaEAkwI6rq2Kr6501dx+amqp5RVd+rqv+qqp03YR0XVtVvbqrrbwpV9Zqq+n/nbd/ge1FV96uqc4ftR27KWmdBVT2oqtZs6joANpYQCbBChj+k5x7XV9WP520/cUrXPLaquqruM43zb6yq2n2ob+sNPH6bJC9Pcmh336q7L1vk/HPv84VV9fwbo/ZZs8Br/V5V/dPwHm3I+S4cfkavrqorq+rTVfX0qvr53w7d/fTufunQf6HvxXFJ/mHYPvXGeJ3rUf/RVfXJEf3+Z1V9bHidl1XVWVX1p1W17UrUCbA5EiIBVsjwh/StuvtWSb6d5OHz2t5yY1+vqirJ7yS5PMlRN/b5Z8Ttk2yb5Oxl+u00vO9PSPKiqjp8fS+0oUF3E5h7rfskuW+SZ27EuR7e3dsn2S3Jy5L8aZITF+m70Pdityz/vVnQSrzfVfW4JO9K8tYku3X3zkken2TXJHee9vXXx2b08wdsAYRIgNlys6p60zAqcnZVHTC3o6ruWFXvrqq1VXVBVT17mXPdP8kdkzwnyZFVdbN55zq6qj5VVa8YRpnOr6pfG9ovqqrvV9VR8/rvONS1tqq+VVV/Pjcite403HVHF6vq41X10uF6V1fVh6rqtkP3/xi+XjmMnt133RdRVTevqr+vqouHx98PbXdN8vV5x390uTe3uz+TSajZe6FR0KHW313gPbo8ybFD++9V1TnDa/lqVd1r3iX2r6ovVdVVVfX2udGsqrp1Vb13eP+uGJ7vus734/zhnBfMH5muqqcM17uiqk6vqt2We53Da/1+kg8nucdwnudV1bvXeW9fXVV/P+JcV3X3aZkErKOqau/h+DdW1V8s9L2oqm8m+aUk7xm+tzcffo5OrKpLquo7w7Grlnm/F339w/fv6TWZMntFVf1jTdw9yWuS3He49pXrvqbhP1lenuS47j6huy8fXuvXu/tZ3X3u0G+rqnp+VX2zJiOV76iq2wz75n6Gjqqqb1fVpVX1wnnX2G54j66oqq8mOXCdGhb9nR5+r95VVf9cVT9IcvRy3yeAlSJEAsyWRyQ5JclOSU5L8g/J5A/ZJO9J8sUkd0pySJI/qKrDljjXUcMxbx+2H7bO/oOSfCnJzpmMxJySyR+5v5Lkt5P8Q1Xdauj76iQ7ZhIKHpjkSUmevB6v638P/W+X5GZJ/nhof8DwdadhRPYzCxz7wiQHJ9k/yX5J7pPkz7v7G0n2mnf8g5cqYAgX9xuO+cLIug9Kcv5Q91/WZOTq2Exe/w6ZfL/mT6H9X0kOT7JHkn3ziz/8t0ryhkxG5u6S5Mf5xff2lkleleQhw6jfryU5a9j3yCR/luTRSXZJ8v8leduYwqvqjkkOS/KfQ9M/Jzm8qnYa9m+dSSh887i3IunuzyVZk8l/UMxv/2/fi+7+5dxwxP2aJCcnuS6Tn7F7Jjk0ye/OO9W67/eY1/+wTH5u98vk/T+su89J8vQknxmuvdMCL+dXMxlxfPcC++Z7dpJHZvJzf8ckVyT5x3X6/PpwvkMyGem++9D+4iS/PDwOy7wZASN/p4/IZKR0pyQ3+mwFgA0lRALMlk929/u7+2eZ/HG/39B+YJJduvu47v5pd5+f5IQkRy50kqq6RZLHJXlrd1+byR+i605pvaC73zBc6+2ZTN87rruv6e4PJflpkl8ZRooen+QF3X11d1+Y5O8ymSo71hu6+xvd/eMk78gkEI71xKGu73f32iQvWc9rJ8mlmUzrfX2S53f3R0Yed3F3v7q7rxtq/90kf9PdZ/TEed39rXn9X9XdFw+jWu/J8Dq7+7Lufnd3/6i7r07yl5mEkjnXZzI6ul13X9Ldc1NAn5bkr7r7nO6+Lsn/yWS0c6nRyEuHkbfvJPlhJt/7dPclmYz8Pm7od3iSS7v7zJHvxc/fkyS3Wc9jUlW3T/KQJH/Q3T8cRkpfkRv+DK/7fo95/S/r7iu7+9tJPpbxP1tzo+HfnVfjKTUZmf9RVc39jD0tyQu7e80QhI9N8ti64fTSl3T3j7v7i5mEwrnf2/+V5C+7+/LuviiT/yyYM+Z3+jPdfWp3Xz+8HwAzQYgEmC3fnff8R0m2Hf5Y3S3JHYc/cK8cQsKfZXIf2kIelcmIz/uH7bckeUhV7TKvz/fmPf9xknT3um23yuSP7ZslmR+WvpXJ6MmGvq5bLdZxAXdc4Np3XI/jk+S23X3r7r57d79q+e4/d9E623dO8s0l+i/4OqvqFlX12ppMBf5BJmFup6pa1d0/zCSkPz3JJVX1vqq623CO3ZK8ct73/PIklaXf+9sOI2+3SPKpJB+ct+/kTEaZM3wdPQo5z52GOtbXbkm2yeQ1zr2e12Yy6jhn3fd7zOvf0J+tuRHkO8w1dPeRw3v3+SSr5tXwr/NqOCfJz3LD373FarjjOq9p/s/xmN/pdd8PgJkgRAJsHi7KZORwp3mP7bv7oYv0PyqTP2S/XVXfTfLOTP6Af8IGXPvSJNdm8kfvnLtkMtKVTEa7bjFv3/9Yj3P3iD4XL3Dti9fjGov54fB1qdrXre+iTKYmrq8/ymS640HdvUN+MY23kqS7T+/u/5lJoPlaJiNSc9d72jrf9+26+9PLXXAYuXpjJvcFzo26nZpk3+GexodlPadIVtWBmQS4ZVc9XcBFSa7JEHKHxw7dvde8Pgu93xv0+hc417q+lsnP8KNH1P2QdWrYtru/s8xxSXJJbrhAz13WOe9yv9Njfj8AVpwQCbB5+FySH9Tkowe2q6pVVbX38Ef9DVTV3P1VD8tkat/cvYR/nQ1YpXWY7vqOTO5R236YSvjcTO6xSyb37z2gqu5SVTsmecF6nH5tJlM5f2mJPm9L8udVtcsQhl4079obbJga+50kvz28n0/J8gHx9Un+uKruPdxj+SvLTC2ds30mI7tXDouyvHhuR1XdvqoeMdwbeU2S/8pkpCuZLA7zgqraa+i743Bf5rKq6uaZTPv9boZRt+7+SX6xGunnhimgY861Q1U9LJP7Zv+5u7885rj5hum0H0ryd8P5tqqqX66qBy5x2Aa//kxG2neteQtKrVNPZxLuX1yTxZJuPXxP98wNRwNfk8nP/m5DDbtU1REja3jHUP+ta7KQ0rPm7Rv9Ow0wa4RIgM3AEOQenkkgvCCT0cHXZ7LYzbp+J8lZ3f2h7v7u3COT+7HmRqHW17MyGbk7P5NRqLcmOWmo7cOZ3FP5pSRnJnnveryuH2Vyf+Cnhil9By/Q7S+SrB7O/+VMphr+xQa8hoX8XpLnZRKy9kqy5AhXd79zqPetSa7OZGRvzP2Bf59ku0y+b/+ZG04x3SqTMHNxJtM1H5jk/xmu96+ZhP9ThmmwX8nkvsKlXFlV/5VJiLpvkkcMgWnOyZl8/MeYqazvqaqrMxk1e2Emq5muz4JK63pSJlOjv5rJAjXvyrzppOvawNc/56OZrMT73aq6dJHzvz2T+xZ/O5PXeGkmwe91mYzeJ8krM1nk6kPDe/GfmSwANMZLMpnCekEmAfrn7/l6/k4DzJS64b8rAMBNWVXdJZOpnP+ju3+wqesBYPNjJBIAthDDx0o8N8kpAiQAG2rr5bsAAJu74Z7L72UyvfLwTVwOAJsx01kBAAAYzXRWAAAARhMiAQAAGM09kYPb3va2vfvuu2/qMgAAADaJM88889Lu3mW5fkLkYPfdd8/q1as3dRkAAACbRFV9a0w/01kBAAAYTYgEAABgNCESAACA0dwTCQAAbDauvfbarFmzJj/5yU82dSmbrW233Ta77rprttlmmw06XogEAAA2G2vWrMn222+f3XffPVW1qcvZ7HR3LrvssqxZsyZ77LHHBp3DdFYAAGCz8ZOf/CQ777yzALmBqio777zzRo3kCpEAAMBmRYDcOBv7/gmRAAAA62HVqlXZf//9s/fee+dxj3tcfvSjH230OS+88MLsvffeN0J10+eeSAAAYLO1+/Pfd6Oe78KX/dayfbbbbrucddZZSZInPvGJec1rXpPnPve5o85/3XXXZeutN+8YZiQSAABgA93//vfPeeed999GEv/2b/82xx57bJLkQQ96UP7sz/4sD3zgA/PKV74y3/ve9/KoRz0q++23X/bbb798+tOfTpL87Gc/y+/93u9lr732yqGHHpof//jHSZITTjghBx54YPbbb7885jGP+fnI5zvf+c7svffe2W+//fKABzzg5+d43vOelwMPPDD77rtvXvva197or1mIBAAA2ADXXXddPvCBD2SfffZZtu+VV16ZT3ziE/mjP/qjPPvZz84DH/jAfPGLX8znP//57LXXXkmSc889N8985jNz9tlnZ6eddsq73/3uJMmjH/3onHHGGfniF7+Yu9/97jnxxBOTJMcdd1xOP/30fPGLX8xpp52WJDnxxBOz44475owzzsgZZ5yRE044IRdccMGN+rqFSAAAgPXw4x//OPvvv38OOOCA3OUud8lTn/rUZY95/OMf//PnH/3oR/OMZzwjyeT+yh133DFJsscee2T//fdPktz73vfOhRdemCT5yle+kvvf//7ZZ5998pa3vCVnn312kuR+97tfjj766Jxwwgn52c9+liT50Ic+lDe96U3Zf//9c9BBB+Wyyy7Lueeee6O99sQ9kQAAAOtl/j2Rc7beeutcf/31P99e9yM0bnnLWy573pvf/OY/f75q1aqfT2c9+uijc+qpp2a//fbLG9/4xnz84x9PkrzmNa/JZz/72bzvfe/L/vvvn7POOivdnVe/+tU57LDDNvTlLctIJAAAwEa6/e1vn+9///u57LLLcs011+S9733von0POeSQHH/88Ukm9zD+4Ac/WPLcV199de5whzvk2muvzVve8paft3/zm9/MQQcdlOOOOy63ve1tc9FFF+Wwww7L8ccfn2uvvTZJ8o1vfCM//OEPb4RX+AtGIgEAADbSNttskxe96EU56KCDsscee+Rud7vbon1f+cpX5phjjsmJJ56YVatW5fjjj88d7nCHRfu/9KUvzUEHHZTddtst++yzT66++uokyfOe97yce+656e4ccsgh2W+//bLvvvvmwgsvzL3uda90d3bZZZeceuqpN+prre6+UU+4uTrggAN69erVm7oMAABgCeecc07ufve7b+oyNnsLvY9VdWZ3H7DcsaazAgAAMJoQCQAAwGhCJAAAAKNZWIfNwu7Pf9+mLgE2exe+7Lc2dQkAcKPo7lTVpi5js7Wx6+IYiQQAADYb2267bS677LKNDkJbqu7OZZddlm233XaDz2EkEgAA2GzsuuuuWbNmTdauXbupS9lsbbvtttl11103+HghEgAA2Gxss8022WOPPTZ1GVs001kBAAAYTYgEAABgNCESAACA0YRIAAAARhMiAQAAGE2IBAAAYDQhEgAAgNGESAAAAEYTIgEAABhNiAQAAGA0IRIAAIDRhEgAAABGEyIBAAAYTYgEAABgNCESAACA0YRIAAAARhMiAQAAGE2IBAAAYDQhEgAAgNGESAAAAEYTIgEAABhNiAQAAGA0IRIAAIDRhEgAAABGEyIBAAAYTYgEAABgNCESAACA0YRIAAAARhMiAQAAGE2IBAAAYDQhEgAAgNGESAAAAEYTIgEA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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This is a very interesting observation. It seems women are spending almost as much, on average, as male shoppers even though there are far less of them making purchases. From this observation, we note that the number of males and females play an important role here. Women are only spending about $250,000 less than men even though there are far less of them shopping. From these two graphs we can conclude there are much more men buying on Black Friday than women. However on average women spend much more.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Age"><section id="5">Age</section><a class="anchor-link" href="#Age">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Creating an ad to appeal to a certain age group is very important. One reason is that different age groups consume different media. If I had a product that sold well to people over 55 but not well at all to younger ages, it would be a very bad idea to create ads on <a href="https://help.instagram.com/424737657584573Instagram">Instagram</a> for it. We don't want customers to see ads for a product that they are not interested in. If we advertise the wrong products to a group, it could also be other problems. There might be a critic from people who are not supposed to see it. Retailers could also be upset that they spent money on a non profitable group. In conclusion, it is very important that we analyze the data by age group.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, let's view how a customer in different groups of age spend money on Black Friday.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[10]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">groups</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;User_ID&#39;</span><span class="p">,</span> <span class="s1">&#39;Age&#39;</span><span class="p">,</span> <span class="s1">&#39;Mean_age&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>
<span class="c1">#0-17</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 0-17 total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mf">8.5</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="c1">#18-25</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 18-25 total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mf">21.5</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="c1">#26-35</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 26-35 total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mf">30.5</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="c1">#36-45</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 36-45 total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mf">40.5</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="c1">#46-50</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 46-50 total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mi">48</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="c1">#51-55</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 51-55 total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mi">53</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="c1">#55+</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;group 55+ total purchase&#39;</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="n">groups</span><span class="p">[</span><span class="n">groups</span><span class="o">.</span><span class="n">Mean_age</span> <span class="o">==</span> <span class="mf">67.5</span><span class="p">]</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 0-17 total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1000001</td>
      <td>0-17</td>
      <td>8.5</td>
      <td>333481</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1000019</td>
      <td>0-17</td>
      <td>8.5</td>
      <td>1457938</td>
    </tr>
    <tr>
      <th>48</th>
      <td>1000051</td>
      <td>0-17</td>
      <td>8.5</td>
      <td>200772</td>
    </tr>
    <tr>
      <th>72</th>
      <td>1000075</td>
      <td>0-17</td>
      <td>8.5</td>
      <td>1035228</td>
    </tr>
    <tr>
      <th>83</th>
      <td>1000086</td>
      <td>0-17</td>
      <td>8.5</td>
      <td>294050</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 18-25 total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>17</th>
      <td>1000018</td>
      <td>18-25</td>
      <td>21.5</td>
      <td>1978675</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1000021</td>
      <td>18-25</td>
      <td>21.5</td>
      <td>126744</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1000022</td>
      <td>18-25</td>
      <td>21.5</td>
      <td>1279678</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1000025</td>
      <td>18-25</td>
      <td>21.5</td>
      <td>534215</td>
    </tr>
    <tr>
      <th>33</th>
      <td>1000034</td>
      <td>18-25</td>
      <td>21.5</td>
      <td>807747</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 26-35 total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2</th>
      <td>1000003</td>
      <td>26-35</td>
      <td>30.5</td>
      <td>341635</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1000005</td>
      <td>26-35</td>
      <td>30.5</td>
      <td>821001</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1000008</td>
      <td>26-35</td>
      <td>30.5</td>
      <td>796545</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1000009</td>
      <td>26-35</td>
      <td>30.5</td>
      <td>593960</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1000011</td>
      <td>26-35</td>
      <td>30.5</td>
      <td>556902</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 36-45 total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>6</th>
      <td>1000007</td>
      <td>36-45</td>
      <td>40.5</td>
      <td>234427</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1000010</td>
      <td>36-45</td>
      <td>40.5</td>
      <td>2169486</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1000014</td>
      <td>36-45</td>
      <td>40.5</td>
      <td>127629</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1000016</td>
      <td>36-45</td>
      <td>40.5</td>
      <td>150428</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1000023</td>
      <td>36-45</td>
      <td>40.5</td>
      <td>1670998</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 46-50 total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>3</th>
      <td>1000004</td>
      <td>46-50</td>
      <td>48.0</td>
      <td>205987</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1000013</td>
      <td>46-50</td>
      <td>48.0</td>
      <td>713927</td>
    </tr>
    <tr>
      <th>32</th>
      <td>1000033</td>
      <td>46-50</td>
      <td>48.0</td>
      <td>1940043</td>
    </tr>
    <tr>
      <th>34</th>
      <td>1000035</td>
      <td>46-50</td>
      <td>48.0</td>
      <td>821303</td>
    </tr>
    <tr>
      <th>41</th>
      <td>1000044</td>
      <td>46-50</td>
      <td>48.0</td>
      <td>1180380</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 51-55 total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>5</th>
      <td>1000006</td>
      <td>51-55</td>
      <td>53.0</td>
      <td>379450</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1000017</td>
      <td>51-55</td>
      <td>53.0</td>
      <td>1425501</td>
    </tr>
    <tr>
      <th>51</th>
      <td>1000054</td>
      <td>51-55</td>
      <td>53.0</td>
      <td>187201</td>
    </tr>
    <tr>
      <th>56</th>
      <td>1000059</td>
      <td>51-55</td>
      <td>53.0</td>
      <td>980068</td>
    </tr>
    <tr>
      <th>57</th>
      <td>1000060</td>
      <td>51-55</td>
      <td>53.0</td>
      <td>279980</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>group 55+ total purchase
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Age</th>
      <th>Mean_age</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>1000002</td>
      <td>55+</td>
      <td>67.5</td>
      <td>810353</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1000031</td>
      <td>55+</td>
      <td>67.5</td>
      <td>496154</td>
    </tr>
    <tr>
      <th>77</th>
      <td>1000080</td>
      <td>55+</td>
      <td>67.5</td>
      <td>339119</td>
    </tr>
    <tr>
      <th>86</th>
      <td>1000089</td>
      <td>55+</td>
      <td>67.5</td>
      <td>112226</td>
    </tr>
    <tr>
      <th>87</th>
      <td>1000090</td>
      <td>55+</td>
      <td>67.5</td>
      <td>1310621</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Graphing-the-amount-of-purchase-by-different-groups-of-age">Graphing the amount of purchase by different groups of age<a class="anchor-link" href="#Graphing-the-amount-of-purchase-by-different-groups-of-age">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[11]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">groups</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Age&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">groups</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Age&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase By Different Groups of Age&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Groups of Age&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase in U.S Dollar&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[11]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;The Amount of Purchase in U.S Dollar&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA4IAAAHwCAYAAADzfNGCAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMS4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvNQv5yAAAIABJREFUeJzs3Xm4XWV99//3xxCNA5MQLRICaYsVGRI1GC0qWiugVanTA9QBnKj+cKqWVtQHETtYH6t1qggSQYtgnWhEFGidanEgWEYRQQaJQQlhVAYJfH9/rHVwczzDTjjrHHLW+3Vd+zp7zd+19z7J/pz7XvdKVSFJkiRJ6o/7zXQBkiRJkqTpZRCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgpN5KckSSf5vpOjY2SV6b5JdJfpVkqxms44okfzpTx58JSY5K8n8Hpu/xXiTZI8kl7fSfz2StfZLGJ5Ncn+QHM12PJA3DIChp1mq/DI887kpy68D0izs65hFJKsnju9j/vZVkh7a+TTZw+7nA+4G9quohVbV2nP2PvM5XJHnrVNR+XzPGuf4yyb+2r9GG7O+K9jN6c5IbkpyZ5DVJ7v6/uqpeU1Xvbtcf6704EvhIO33yVJznetR/UJLvDLHeM5J8oz3PtUnOSfK3SeZNR50deRLwDGBBVY37u5/kqe1n5m+mrzRJGptBUNKs1X4ZfkhVPQT4GfCcgXknTPXxkgR4KXAdcOBU7/8+4uHAPODCSdbbon3dDwAOT7LP+h5oQ8PqDBg5112BJwKH3It9PaeqNgW2B94D/C1w7DjrjvVebM/k782YpuP1TvIi4PPAZ4Dtq2orYD9gAbDdTNU1BbYHrqiqX0+y3oHM7n8fJG1EDIKS+u7+ST7Vtk5cmGTpyIIkj0jyhSRrklye5A2T7OvJwCOANwL7J7n/wL4OSvI/ST7QtvZcluSP2/lXJbkmyYED62/e1rUmyZVJ3jHSMjS6S+voVr4k30zy7vZ4Nyc5PcnW7erfbn/e0LZiPXH0SSR5QJJ/SbK6ffxLO++RwMUD2399she3qr5LE0x2Gas1sq31VWO8RtcBR7TzX53kovZcfpTksQOHWJLkvCQ3JvnsSKtSki2TnNK+fte3zxeMej8ua/d5+WALcZJXtMe7PslpSbaf7Dzbc70GOAN4dLufQ5N8YdRr++Ek/zLEvm6sqhU0IenAJLu02x+X5O/Gei+S/BT4feDL7Xv7gPZzdGySq5P8vN12ziSv97jn375/r0nT/fT6JB9NYyfgKOCJ7bFvGH1O7R9K3g8cWVXHVNV17bleXFWvr6pL2vWOSPL5JP+W5CbgoPE+kwPn8Z1Rx6okfzjwmh2V5Iz2/f7WyDm1tX8gze/fje1naZex3pM0/x6sSHJdkkuTvLqd/0rgEwPn/q5xtn8Q8EKaPxTsmIF/a9rlL0vzu742yf/NQNfnJPdL8tYkP22X/3uSh451HEkalkFQUt89FzgJ2AJYAXwEmi9ewJeBc4FtgacDb0qy9wT7OrDd5rPt9LNHLV8GnAdsRdMichKwO/CHwEuAjyR5SLvuh4HNab7Y7wm8DHj5epzXX7TrPwy4P/DX7fyntD+3aFtGvzvGtm8HngAsARYDjwfeUVU/AXYe2P5PJiqg/ZK9R7vN/w5Z9zLgsrbuv0/TgnQEzflvRvN+DXZH/T/APsAiYDfgoHb+/YBP0rTULARu5bfv7YOBDwHPbFvf/hg4p13258DbgOcD84H/Bk4cpvAkjwD2Br7Xzvo3YJ8kW7TLN6EJdp8e7qWAqvoBsIrmjwyD83/nvaiqP+CeLd+3A8cD62g+Y48B9gJeNbCr0a/3MOf/bJrP7WKa13/vqroIeA3w3fbYW4xxOn9E0/L3hTGWjbYvTcvhFsAJjPOZHGI/I14MvBvYmua9HukRsBfN78Qj22Ptxz0/X4NOpHkvHkET6P4hydOr6ljuee7vHGf7FwC/Aj4HnEbzmQYgyaOBf23r3Ibmd3/bgW3fAPw5zb8FjwCuBz465LlL0phmXRBMsrz9y94FQ6y7fZL/av8C+M0M/LVYUm98p6pOrao7ab6gL27n7w7Mr6ojq+o3VXUZcAyw/1g7af/a/yLgM1V1B82X2NHdvy6vqk+2x/osTVe4I6vq9qo6HfgN8Idti81+wGFVdXNVXQH8M02302F9sqp+UlW3Av9O8wV6WC9u67qmqtYA71rPYwNcS9MF7hPAW6vqv4bcbnVVfbiq1rW1vwp4b1WdVY1Lq+rKgfU/VFWr29alL9OeZ1WtraovVNUtVXUz8Pc0X6JH3EXTSvnAqrq6qka6U/4l8I9VdVFVrQP+gabVcaJWwWvbFrCfA7+mee+pqqtpWmBf1K63D3BtVZ095Gtx92sCrHfrT5KHA88E3lRVv25bLD/APT/Do1/vYc7/PVV1Q1X9DPgGw3+2RlqlfzFQ40lpWshvSTL4GftuVZ1cVXe1dd3bz+RXqurbbTh+O03r3XbAHcCmwKOAtOd99eiN23WfBPxtVd1WVefQfLbXp4YDgc+2v/+fAQ7Ib68nfSHw5ar6TlX9BjgcqIFt/xJ4e1Wtas/hCOCF2Ti6zUq6j5p1QRA4juY/22G8D/hUVe1Gc4H9P3ZVlKT7rF8MPL8FmNd+udoeeET7JfWG9ov+22iuyxrL82haXk5tp08Anplk/sA6vxx4fitAVY2e9xCaL8z3BwYDz5Xcs4Vgfc/rIeOtOIZHjHHsR6zH9gBbV9WWVbVTVX1oPba7atT0dsBPJ1h/zPNM8qAkH2+72t1EE8i2SDKnvY5rP5pWnKuTfCXJo9p9bA98cOA9vw4IE7/2W7ctYA8C/gf42sCy42lae2l/Dt0aOGDbto71tT0wl+YcR87n4zStfyNGv97DnP+GfrZGWtq2GZlRVfu3r90PgTkT1HVvP5N376+qfkVzXo+oqq/TtBR/FPhlkqOTbDbG9o8Armv/qDBYw1C/k22QfBq/bYn8D5rrO/9sYP+DNd7CPVsmtwe+NPC+XATcyfj/HknSpGZdEKyqbzPqP8wkf5Dka0nOTvLfA//hPxoY+Sv1N2i6okgSNF/KLq+qLQYem1bVs8ZZ/0CaL8Q/S/ILmu5fc2kGS1lf19K0VAy2wiykaXGCptXpQQPLfm899l2Tr8LqMY69ej2OMZ6RgTQmqn10fVcBf7ABx3oLTVfEZVW1Gb/tEhuAqjqtqp5BE0p+TNPaO3K8vxz1vj+wqs6c7IBty9VxNK1NI61fJwO7tdedPZvfBoGhJNmdJmxMOhrnGK4CbqcNqu1js6raeWCdsV7vDTr/MfY12o9pPsPP34B9TfSZvMfvQ5Kxfh+2G1j+EJoW1tUAVfWhqnocTVfbRwKHjrH9auChSTYdVcPPx1h3LC+l+c715fbfh8toguBI99CrabrNjtT4QJou5COuounKPPi+zKuqYY8vSb9j1gXBcRwNvL79h/6vafrhQ3Ptzwva588DNs0M3hNL0n3KD4Cb0gxr/8Akc5Ls0n4xv4ckI9cQPpumm9zIdUz/xAaMDth2Hft3mmu2Nm275b2Z5pozaK5xekqShUk2Bw5bj92voekW+fsTrHMi8I4k89tAc/jAsTdY26Xv58BL2tfzFUwe8j4B/HWSx7XXHP7hJN00R2xK08J6Qzuoxt3XbSV5eJLnttcK3k5z3dad7eKjgMOS7Nyuu3l7neKk0gxe8lKaFrO17Tnfxm9HyfxB251ymH1tluTZNNeR/ltVnT/MdoPaLo6nA//c7u9+7R9G95xgsw0+f5oW7wUZGCRpVD1FE9DfmWYAoC3b93RHJm/ZmugzeS6wc5IlaQYLOmKM7Z+V5Eltbe8Gvl9VVyXZPcmytovmr4Hb+O1nYbD2q4AzgX9MMi/JbsArGT7Yv4ymO+uSgccLgD9rv3d8HnhOmgGk7t+um4Htj6L592BkkJv5SfzjtaR7ZdYHwfYvf38MfC7JOTTdYka6pfw1sGeS/6W5duTnNF27JPVcG8aeQ/OF7XKaVrpP0AziMNpLgXOq6vSq+sXIg2ZAkpHWoPX1epovppfRtAZ9Blje1nYGzTWG5wFnA6esx3ndQnO93P+03cyeMMZqfwesbPd/Pk23vb/bgHMYy6tpWlzW0rTATNjSVFWfa+v9DHAzTQvbMNfL/QvwQJr37Xvcs7vm/WgCyWqaHiR7Av9fe7wv0QT4k9oupRfQXGc3kRuS/IomCD0ReG4bekYcT3NriWG6hX45yc00LUBvpxllc30GCRrtZTTdjH9EM8DI5xnomjnaBp7/iK/TjBD7iyTXjrP/z9IMMPMSmnO8luaPHkfTtKKPZ9zPZDUD5xwJ/CdwCWO3nn6G5o8B1wGPo7nmEJoBiI6heW2upPlcvm+cGg4AdqD53HwJeGf7uzih9ndsB+Cjg/8+VDMq7KXAAe01qq+nCf5X03zWr6H5QwXAB2kGszq9/Xx8j2agH0naYLnn/1WzQ5IdgFOqape2r//FVTXuf3ztNg8BflxVDhgjSZoySRbSdIv8vaq6aabr6ZskxwGrqmp9RhmdUe13khuAHavq8pmuR9LsNOtbBNv/dC8f6drSdkNZ3D7fOu19uWi6Vi2foTIlSbNQ+3/Mm4GTDIGaSJLntIMcPZimVfJ84IqZrUrSbDbrgmCSE4HvAn+UZFWaG72+GHhlknNpuq2M9Kt/KnBxkp/QXJ/w9zNQsiRpFmq/0N8EPIOBaxSlcexL0+10NbAjsH/Nxm5bku4zZmXXUEmSJEnS+GZdi6AkSZIkaWIGQUmSJEnqmU1muoCptPXWW9cOO+ww02VIkiRJ0ow4++yzr62q+ZOtN6uC4A477MDKlStnugxJkiRJmhFJrhxmPbuGSpIkSVLPGAQlSZIkqWcMgpIkSZLUM7PqGkFJkiRJ93133HEHq1at4rbbbpvpUjZa8+bNY8GCBcydO3eDtjcISpIkSZpWq1atYtNNN2WHHXYgyUyXs9GpKtauXcuqVatYtGjRBu3DrqGSJEmSptVtt93GVlttZQjcQEnYaqut7lWLqkFQkiRJ0rQzBN479/b1MwhKkiRJ6p05c+awZMkSdtllF170ohdxyy233Ot9XnHFFeyyyy5TUF33vEZQkiRJ0oza4a1fmdL9XfGeP5t0nQc+8IGcc845ALz4xS/mqKOO4s1vfvNQ+1+3bh2bbLJxRylbBCVJkiT12pOf/GQuvfTS32nRe9/73scRRxwBwFOf+lTe9ra3seeee/LBD36QX/7ylzzvec9j8eLFLF68mDPPPBOAO++8k1e/+tXsvPPO7LXXXtx6660AHHPMMey+++4sXryYF7zgBXe3QH7uc59jl112YfHixTzlKU+5ex+HHnoou+++O7vtthsf//jHp/ycDYKSJEmSemvdunV89atfZdddd5103RtuuIFvfetbvOUtb+ENb3gDe+65J+eeey4//OEP2XnnnQG45JJLOOSQQ7jwwgvZYost+MIXvgDA85//fM466yzOPfdcdtppJ4499lgAjjzySE477TTOPfdcVqxYAcCxxx7L5ptvzllnncVZZ53FMcccw+WXXz6l520QlCRJktQ7t956K0uWLGHp0qUsXLiQV77ylZNus99++939/Otf/zqvfe1rgeZ6w8033xyARYsWsWTJEgAe97jHccUVVwBwwQUX8OQnP5ldd92VE044gQsvvBCAPfbYg4MOOohjjjmGO++8E4DTTz+dT33qUyxZsoRly5axdu1aLrnkkik7d/AaQUmSJEk9NHiN4IhNNtmEu+666+7p0bdnePCDHzzpfh/wgAfc/XzOnDl3dw096KCDOPnkk1m8eDHHHXcc3/zmNwE46qij+P73v89XvvIVlixZwjnnnENV8eEPf5i99957Q09vUrYISpIkSRLw8Ic/nGuuuYa1a9dy++23c8opp4y77tOf/nQ+9rGPAc01fTfddNOE+7755pvZZpttuOOOOzjhhBPunv/Tn/6UZcuWceSRR7L11ltz1VVXsffee/Oxj32MO+64A4Cf/OQn/PrXv56CM/wtWwQlSZIkCZg7dy6HH344y5YtY9GiRTzqUY8ad90PfvCDHHzwwRx77LHMmTOHj33sY2yzzTbjrv/ud7+bZcuWsf3227Prrrty8803A3DooYdyySWXUFU8/elPZ/Hixey2225cccUVPPaxj6WqmD9/PieffPKUnmuqakp3ePeOk+2ATwG/B9wFHF1VHxy1ToAPAs8CbgEOqqoftssOBN7Rrvp3VXX8ZMdcunRprVy5cupOQpIkSdKUu+iii9hpp51muoyN3livY5Kzq2rpZNt22SK4DnhLVf0wyabA2UnOqKofDazzTGDH9rEM+BiwLMlDgXcCS4Fqt11RVdd3WK8kSZIk9UJn1whW1dUjrXtVdTNwEbDtqNX2BT5Vje8BWyTZBtgbOKOqrmvD3xnAPl3VKkmSJEl9Mi2DxSTZAXgM8P1Ri7YFrhqYXtXOG2++JEmSJOle6nywmCQPAb4AvKmqRg+lkzE2qQnmj7X/g4GDARYuXHgvKpXUN7seP/mNY2eL8w88f6ZLkCTpHqqKZsgQbYh7O9ZLpy2CSebShMATquqLY6yyCthuYHoBsHqC+b+jqo6uqqVVtXT+/PlTU7gkSZKkzsybN4+1a9fe6zDTV1XF2rVrmTdv3gbvo7MWwXZE0GOBi6rq/eOstgJ4XZKTaAaLubGqrk5yGvAPSbZs19sLOKyrWiVJkiRNnwULFrBq1SrWrFkz06VstObNm8eCBQs2ePsuu4buAbwUOD/JOe28twELAarqKOBUmltHXEpz+4iXt8uuS/Ju4Kx2uyOr6roOa5UkSZI0TebOncuiRYtmuoxe6ywIVtV3GPtav8F1CjhknGXLgeUdlCZJkiRJvTYto4ZKkiRJku47DIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqmU262nGS5cCzgWuqapcxlh8KvHigjp2A+VV1XZIrgJuBO4F1VbW0qzolSZIkqW+6bBE8DthnvIVV9f+qaklVLQEOA75VVdcNrPK0drkhUJIkSZKmUGdBsKq+DVw36YqNA4ATu6pFkiRJkvRbM36NYJIH0bQcfmFgdgGnJzk7ycGTbH9wkpVJVq5Zs6bLUiVJkiRpVpjxIAg8B/ifUd1C96iqxwLPBA5J8pTxNq6qo6tqaVUtnT9/fte1SpIkSdJG774QBPdnVLfQqlrd/rwG+BLw+BmoS5IkSZJmpRkNgkk2B/YE/mNg3oOTbDryHNgLuGBmKpQkSZKk2afL20ecCDwV2DrJKuCdwFyAqjqqXe15wOlV9euBTR8OfCnJSH2fqaqvdVWnJEmSJPVNZ0Gwqg4YYp3jaG4zMTjvMmBxN1VJkiRJku4L1whKkiRJkqaRQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSeqazIJhkeZJrklwwzvKnJrkxyTnt4/CBZfskuTjJpUne2lWNkiRJktRHXbYIHgfsM8k6/11VS9rHkQBJ5gAfBZ4JPBo4IMmjO6xTkiRJknqlsyBYVd8GrtuATR8PXFpVl1XVb4CTgH2ntDhJkiRJ6rGZvkbwiUnOTfLVJDu387YFrhpYZ1U7T5IkSZI0BTaZwWP/ENi+qn6V5FnAycCOQMZYt8bbSZKDgYMBFi5c2EWdkiRJkjSrTNgimGROkn/r4sBVdVNV/ap9fiowN8nWNC2A2w2sugBYPcF+jq6qpVW1dP78+V2UKkmSJEmzyoRBsKruBOYnuf9UHzjJ7yVJ+/zxbS1rgbOAHZMsao+7P7Biqo8vSZIkSX01TNfQK4D/SbIC+PXIzKp6/0QbJTkReCqwdZJVwDuBue22RwEvBF6bZB1wK7B/VRWwLsnrgNOAOcDyqrpwPc9LkiRJkjSOYYLg6vZxP2DTYXdcVQdMsvwjwEfGWXYqcOqwx5IkSZIkDW/SIFhV75qOQiRJkiRJ02PSIJhkPvA3wM7AvJH5VfUnHdYlSZIkSerIMPcRPAH4MbAIeBfNNYNndViTJEmSJKlDwwTBrarqWOCOqvpWVb0CeELHdUmSJEmSOjLMYDF3tD+vTvJnNAPHLOiuJEmSJElSl4YJgn+XZHPgLcCHgc2Av+q0KkmSJElSZ4YZNfSU9umNwNO6LUeSJEmS1LVxg2CSDwM13vKqekMnFUmSJEmSOjVRi+DKaatCkiRJkjRtxg2CVXX8dBYiSZIkSZoeE3UN/TITdw19bicVSZIkSZI6NVHX0PdNWxWSJEmSpGkzUdfQb408T3J/4JHt5MVVdcfYW0mSJEmS7usmvX1EkqcCxwNXAAG2S3JgVX2729IkSZIkSV0Y5oby/wzsVVUXAyR5JHAi8LguC5MkSZIkdeN+Q6wzdyQEAlTVT4C53ZUkSZIkSerSMC2CK5McC3y6nX4xcHZ3JUmSJEmSujRMEHwtcAjwBpprBL8N/GuXRUmSJEmSujNpEKyq25N8Gvh0Va2ZhpokSZIkSR0a9xrBNI5Ici3wY+DiJGuSHD595UmSJEmSptpEg8W8CdgD2L2qtqqqhwLLgD2S/NW0VCdJkiRJmnITBcGXAQdU1eUjM6rqMuAl7TJJkiRJ0kZooiA4t6quHT2zvU7Q20dIkiRJ0kZqoiD4mw1cJkmSJEm6D5to1NDFSW4aY36AeR3VI0mSJEnq2LhBsKrmTGchkiRJkqTpMVHXUEmSJEnSLGQQlCRJkqSeMQhKkiRJUs8MHQSTbJXkeUke12VBkiRJkqRujRsEk5ySZJf2+TbABcArgE8nedM01SdJkiRJmmITtQguqqoL2ucvB86oqucAy2gCoSRJkiRpIzRRELxj4PnTgVMBqupm4K4ui5IkSZIkdWeiG8pfleT1wCrgscDXAJI8EJg7DbVJkiRJkjowUYvgK4GdgYOA/arqhnb+E4BPdlyXJEmSJKkj47YIVtU1wGvGmP8N4BtdFiVJkiRJ6s4G3UcwycFTXYgkSZIkaXps6A3lM6VVSJIkSZKmzQYFwar6+FQXIkmSJEmaHuNeI5jkzaNmFXAt8J2qurzTqiRJkiRJnZmoRXDTUY/NgKXAV5PsPw21SZIkSZI6MNGooe8aa36ShwL/CZzUVVGSJEmSpO6s9zWCVXUdDhYjSZIkSRut9Q6CSf4EuH6I9ZYnuSbJBeMsf3GS89rHmUkWDyy7Isn5Sc5JsnJ9a5QkSZIkjW+iwWLOpxkgZtBDgdXAy4bY93HAR4BPjbP8cmDPqro+yTOBo4FlA8ufVlXXDnEcSZIkSdJ6GDcIAs8eNV3A2qr69TA7rqpvJ9lhguVnDkx+D1gwzH4lSZIkSffORIPFXDmNdbwS+Org4YHTkxTw8ao6ehprkSRJkqRZbaIWwWmR5Gk0QfBJA7P3qKrVSR4GnJHkx1X17XG2Pxg4GGDhwoWd1ytJkiRJG7v1HixmKiXZDfgEsG9VrR2ZX1Wr25/XAF8CHj/ePqrq6KpaWlVL58+f33XJkiRJkrTRm7EgmGQh8EXgpVX1k4H5D06y6chzYC9gzJFHJUmSJEnrb9KuoUmeD/wT8DCa+wcGqKrabJLtTgSeCmydZBXwTmAuzcZHAYcDWwH/mgRgXVUtBR4OfKmdtwnwmar62oacnCRJkiTpdw1zjeB7gedU1UXrs+OqOmCS5a8CXjXG/MuAxb+7hSRJkiRpKgzTNfSX6xsCJUmSJEn3XcO0CK5M8lngZOD2kZlV9cXOqpIkSZIkdWaYILgZcAvNoC0jimagF0mSJEnSRmbSIFhVL5+OQiRJkiRJ02PcIJjkb6rqvUk+TNMCeA9V9YZOK5MkSZIkdWKiFsGRAWJWTkchkiRJkqTpMW4QrKovtz+Pn75yJEmSJEldG+b2EZIkSZKkWcQgKEmSJEk9YxCUJEmSpJ6ZNAgmeWSS/0pyQTu9W5J3dF+aJEmSJKkLw7QIHgMcBtwBUFXnAft3WZQkSZIkqTvDBMEHVdUPRs1b10UxkiRJkqTuDRMEr03yB7Q3lU/yQuDqTquSJEmSJHVmohvKjzgEOBp4VJKfA5cDL+m0KkmSJElSZyYNglV1GfCnSR4M3K+qbu6+LEmSJElSV4YZNfSNSTYDbgE+kOSHSfbqvjRJkiRJUheGuUbwFVV1E7AX8DDg5cB7Oq1KkiRJktSZYYJg2p/PAj5ZVecOzJMkSZIkbWSGCYJnJzmdJgielmRT4K5uy5IkSZIkdWWYUUNfCSwBLquqW5JsRdM9VJIkSZK0ERpm1NC7klwOPDLJvGmoSZIkSZLUoUmDYJJXAW8EFgDnAE8Avgv8SbelSZIkSZK6MMw1gm9uKg46AAAen0lEQVQEdgeurKqnAY8B1nRalSRJkiSpM8MEwduq6jaAJA+oqh8Df9RtWZIkSZKkrgwzWMyqJFsAJwNnJLkeWN1tWZIkSZKkrgwzWMzz2qdHJPkGsDnwtU6rkiRJkiR1ZpgWQZLMAR4OXN7O+j3gZ10VJUmSJEnqzjCjhr4eeCfwS357I/kCduuwLkmSJElSR4ZpEXwj8EdVtbbrYiRJkiRJ3Rtm1NCrgBu7LkSSJEmSND3GbRFM8ub26WXAN5N8Bbh9ZHlVvb/j2iRJkiRJHZioa+im7c+ftY/7tw9JkiRJ0kZs3CBYVe+azkIkSZIkSdNj0msEk5zR3lB+ZHrLJKd1W5YkSZIkqSvDDBYzv6puGJmoquuBh3VXkiRJkiSpS8MEwTuTLByZSLI9zX0EJUmSJEkboWHuI/h24DtJvtVOPwU4uLuSJEmSJEldmjAIJglwIfBY4AlAgL+qqmunoTZJkiRJUgcmDIJVVUlOrqrHAadMU02SJEmSpA4Nc43g95Ls3nklkiRJkqRpMcw1gk8D/jLJlcCvabqHVlXt1mllkiRJkqRODBMEn9l5FZIkSZKkaTNM19Aa5zGpJMuTXJPkgnGWJ8mHklya5Lwkjx1YdmCSS9rHgcMcT5IkSZI0uWFaBL9CE/wCzAMWARcDOw+x7XHAR4BPjbP8mcCO7WMZ8DFgWZKHAu8ElrbHPjvJivZm9pIkTeiiR+000yVMq51+fNFMlyBJ2shMGgSratfB6bbV7i+H2XlVfTvJDhOssi/wqaoqmkFptkiyDfBU4Iyquq495hnAPsCJwxxXkiRJkjS+YbqG3kNV/RCYqlFEtwWuGphe1c4bb74kSZIk6V6atEUwyZsHJu9Hc3P5NVN0/IwxryaY/7s7SA4GDgZYuHDhFJUlSZIkSbPXMC2Cmw48HkBzzeC+U3T8VcB2A9MLgNUTzP8dVXV0VS2tqqXz58+forIkSZIkafaasEUwyXya4HdpVd3QwfFXAK9LchLNYDE3VtXVSU4D/iHJlu16ewGHdXB8SZIkSeqdcYNgklcB/wD8FFiU5OCqWrE+O09yIs3AL1snWUUzEuhcgKo6CjgVeBZwKXAL8PJ22XVJ3g2c1e7qyJGBYyRJkiRJ985ELYJvAnauqjVJfh84gaYFb2hVdcAkyws4ZJxly4Hl63M8SZIkSdLkJrpG8DdVtQagqi6juT5QkiRJkrSRm6hFcEGSD403XVVv6K4sSZIkSVJXJgqCh46aPrvLQiRJkiRJ02PcIFhVx09nIZIkSZKk6THMfQQlSZIkSbOIQVCSJEmSembcIJjkn9qfL5q+ciRJkiRJXZuoRfBZSeYCh01XMZIkSZKk7k00aujXgGuBBye5CQhQIz+rarNpqE+SJEmSNMXGbRGsqkOranPgK1W1WVVtOvhzGmuUJEmSJE2hiVoEAaiqfZM8HNi9nfX9qlrTbVmSJEmSpK5MOmpoO1jMD4AXAf8H+EGSF3ZdmCRJkiSpG5O2CALvAHavqmsAkswH/hP4fJeFSZIkSZK6Mcx9BO83EgJba4fcTpIkSZJ0HzRMi+DXkpwGnNhO7wec2l1JkiRJkqQuDTNYzKFJng88iebWEUdX1Zc6r0y6Lzhi85muYHodceNMVyBJkqRpMEyLIFX1ReCLHdciSZIkSZoGXusnSZIkST1jEJQkSZKknhnmPoJvHGaeJEmSJGnjMEyL4IFjzDtoiuuQJEmSJE2TcQeLSXIA8BfAoiQrBhZtSnMvQUmSJEnSRmiiUUPPBK4Gtgb+eWD+zcB5XRYlSZIkSerOuEGwqq4ErgSeOH3lSJIkSZK6NsxgMc9PckmSG5PclOTmJDdNR3GSJEmSpKk3zA3l3ws8p6ou6roYSZIkSVL3hhk19JeGQEmSJEmaPYZpEVyZ5LPAycDtIzOr6oudVSVJkiRJ6swwQXAz4BZgr4F5BRgEJUmSJGkjNGkQrKqXT0chkiRJkqTpMWkQTPJJmhbAe6iqV3RSkSRJkiSpU8N0DT1l4Pk84HnA6m7KkSRJkiR1bZiuoV8YnE5yIvCfnVUkSZIkSerUMLePGG1HYOFUFyJJkiRJmh7DXCN4M801gml//gL4247rkiRJkiR1ZJiuoZtORyGSJEmSpOkxzGAxJHku8JR28ptVdcpE60uSJEmS7rsmvUYwyXuANwI/ah9vTPKPXRcmSZIkSerGMC2CzwKWVNVdAEmOB/4XOKzLwiRJkiRJ3Rh21NAtBp5v3kUhkiRJkqTpMUyL4D8C/5vkGzQjhz4FWwMlSZIkaaM1zKihJyb5JrA7TRD826r6RdeFSZIkSZK6MWzX0PntzznAHyd5fkf1SJIkSZI6NswN5ZcDuwEXAne1swv44hDb7gN8kCZAfqKq3jNq+QeAp7WTDwIeVlVbtMvuBM5vl/2sqp476dlIkiRJkiY1zDWCT6iqR6/vjpPMAT4KPANYBZyVZEVV/Whknar6q4H1Xw88ZmAXt1bVkvU9riRJkiRpYsN0Df1ukvUOgsDjgUur6rKq+g1wErDvBOsfAJy4AceRJEmSJK2HYYLg8TRh8OIk5yU5P8l5Q2y3LXDVwPSqdt7vSLI9sAj4+sDseUlWJvlekj8f7yBJDm7XW7lmzZohypIkSZKkfhuma+hy4KU01+vdNcm6gzLGvBpn3f2Bz1fVnQPzFlbV6iS/D3w9yflV9dPf2WHV0cDRAEuXLh1v/5IkSZKk1jBB8GdVtWID9r0K2G5gegGwepx19wcOGZxRVavbn5e1t694DPA7QVCSJEmStH6GCYI/TvIZ4MvA7SMzq2qyUUPPAnZMsgj4OU3Y+4vRKyX5I2BL4LsD87YEbqmq25NsDewBvHeIWiVJkiRJkxgmCD6QJgDuNTBv0ttHVNW6JK8DTqO5fcTyqrowyZHAyoFWxgOAk6pqsFvnTsDHk9xFcx3jewZHG5UkSZIkbbhJg2BVvXz0vCS7D7PzqjoVOHXUvMNHTR8xxnZnArsOcwxJkiRJ0voZpkUQgPYWEvvTtODdCCztqihJkiRJUncmDILtbR0OaB/rgO2BpVV1RfelSZIkSZK6MO59BJOcSdOtcy7wwqp6HHCzIVCSJEmSNm4T3VB+DbAp8HBgfjvP+/RJkiRJ0kZu3CBYVfvSDNjyQ+BdSS4Htkzy+OkqTpIkSZI09Sa8RrCqbgSWA8uTPAzYD/iXJNtV1XYTbStJkiRJum+aqGvoPVTVNVX14ar6Y+BJHdYkSZIkSerQ0EFwUFVdOdWFSJIkSZKmxwYFQUmSJEnSxssgKEmSJEk9M2kQTPLIJP+V5IJ2erck7+i+NEmSJElSF4ZpETwGOAy4A6CqzgP277IoSZIkSVJ3hgmCD6qqH4yat66LYiRJkiRJ3RsmCF6b5A+AAkjyQuDqTquSJEmSJHVmwhvKtw4BjgYeleTnwOXASzqtSpIkSZLUmUmDYFVdBvxpkgcD96uqm7svS5IkSZLUlUmDYJIHAC8AdgA2SQJAVR3ZaWWSJEmSpE4M0zX0P4AbgbOB27stR5IkSZLUtWGC4IKq2qfzSiRJkiRJ02KYUUPPTLJr55VIkiRJkqbFuC2CSS4A7mrXeXmSy2i6hgaoqtptekqUJEmSJE2libqGbgssma5CJEmSJEnTY6IgeHlVXTltlUiSJEmSpsVEQfBhSd483sKqen8H9UiSJEmSOjZREJwDPITmmkBJkiRJ0iwxURC82pvGS5IkSdLsM9HtI2wJlCRJkqRZaKIg+PRpq0KSJEmSNG3GDYJVdd10FiJJkiRJmh4TtQhKkiRJkmYhg6AkSZIk9YxBUJIkSZJ6xiAoSZIkST1jEJQkSZKknjEISpIkSVLPGAQlSZIkqWcMgpIkSZLUMwZBSZIkSeoZg6AkSZIk9YxBUJIkSZJ6xiAoSZIkST1jEJQkSZKknjEISpIkSVLPdBoEk+yT5OIklyZ56xjLD0qyJsk57eNVA8sOTHJJ+ziwyzolSZIkqU826WrHSeYAHwWeAawCzkqyoqp+NGrVz1bV60Zt+1DgncBSoICz222v76peSZIkSeqLLlsEHw9cWlWXVdVvgJOAfYfcdm/gjKq6rg1/ZwD7dFSnJEmSJPVKl0FwW+CqgelV7bzRXpDkvCSfT7Ldem5LkoOTrEyycs2aNVNRtyRJkiTNal0GwYwxr0ZNfxnYoap2A/4TOH49tm1mVh1dVUuraun8+fM3uFhJkiRJ6osug+AqYLuB6QXA6sEVqmptVd3eTh4DPG7YbSVJkiRJG6bLIHgWsGOSRUnuD+wPrBhcIck2A5PPBS5qn58G7JVkyyRbAnu18yRJkiRJ91Jno4ZW1bokr6MJcHOA5VV1YZIjgZVVtQJ4Q5LnAuuA64CD2m2vS/JumjAJcGRVXddVrZIkSZLUJ50FQYCqOhU4ddS8wweeHwYcNs62y4HlXdYnSZIkSX3U6Q3lJUmSJEn3PQZBSZIkSeoZg6AkSZIk9YxBUJIkSZJ6xiAoSZIkST1jEJQkSZKknjEISpIkSVLPGAQlSZIkqWcMgpIkSZLUMwZBSZIkSeoZg6AkSZIk9YxBUJIkSZJ6ZpOZLkCSJGl9fPQ1X5/pEqbVIUf9yUyXIGkWskVQkiRJknrGIChJkiRJPWMQlCRJkqSeMQhKkiRJUs8YBCVJkiSpZwyCkiRJktQzBkFJkiRJ6hmDoCRJkiT1jEFQkiRJknrGIChJkiRJPbPJTBcgSZIkAfzzfs+e6RKm1Vs+e8pMl6Aes0VQkiRJknrGIChJkiRJPWMQlCRJkqSeMQhKkiRJUs8YBCVJkiSpZwyCkiRJktQzBkFJkiRJ6hmDoCRJkiT1jEFQkiRJknrGIChJkiRJPWMQlCRJkqSeMQhKkiRJUs8YBCVJkiSpZwyCkiRJktQzBkFJkiRJ6hmDoCRJkiT1jEFQkiRJknrGIChJkiRJPdNpEEyyT5KLk1ya5K1jLH9zkh8lOS/JfyXZfmDZnUnOaR8ruqxTkiRJkvpkk652nGQO8FHgGcAq4KwkK6rqRwOr/S+wtKpuSfJa4L3Afu2yW6tqSVf1SZIkSVJfddki+Hjg0qq6rKp+A5wE7Du4QlV9o6puaSe/ByzosB5JkiRJEt0GwW2BqwamV7XzxvNK4KsD0/OSrEzyvSR/3kWBkiRJktRHnXUNBTLGvBpzxeQlwFJgz4HZC6tqdZLfB76e5Pyq+ukY2x4MHAywcOHCe1+1JEmSJM1yXbYIrgK2G5heAKwevVKSPwXeDjy3qm4fmV9Vq9uflwHfBB4z1kGq6uiqWlpVS+fPnz911UuSJEnSLNVlEDwL2DHJoiT3B/YH7jH6Z5LHAB+nCYHXDMzfMskD2udbA3sAg4PMSJIkSZI2UGddQ6tqXZLXAacBc4DlVXVhkiOBlVW1Avh/wEOAzyUB+FlVPRfYCfh4krtowup7Ro02KkmSJEnaQF1eI0hVnQqcOmre4QPP/3Sc7c4Edu2yNkmSJEnqq05vKC9JkiRJuu8xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPVMp7ePkCRJkiSAVW/975kuYVoteM+TZ7qECdkiKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnNpnpAjZ2O7z1KzNdwrS64j1/NtMlSJIkSbqXbBGUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSesYgKEmSJEk9YxCUJEmSpJ4xCEqSJElSzxgEJUmSJKlnDIKSJEmS1DMGQUmSJEnqGYOgJEmSJPWMQVCSJEmSeqbTIJhknyQXJ7k0yVvHWP6AJJ9tl38/yQ4Dyw5r51+cZO8u65QkSZKkPuksCCaZA3wUeCbwaOCAJI8etdorgeur6g+BDwD/1G77aGB/YGdgH+Bf2/1JkiRJku6lLlsEHw9cWlWXVdVvgJOAfUetsy9wfPv888DTk6Sdf1JV3V5VlwOXtvuTJEmSJN1LXQbBbYGrBqZXtfPGXKeq1gE3AlsNua0kSZIkaQNs0uG+M8a8GnKdYbZtdpAcDBzcTv4qycVDV7hx2xq4droPmn+a7iP21oy8v7xrrF89dWDa398c5Hs7TWbmdze+v9NkRt7f1318uo/YSzPy3v71v/u7O01m5t/mmfvevP0wK3UZBFcB2w1MLwBWj7POqiSbAJsD1w25LQBVdTRw9BTVvNFIsrKqls50HeqG7+/s5vs7e/nezm6+v7OX7+3s5vs7ti67hp4F7JhkUZL70wz+smLUOiuAA9vnLwS+XlXVzt+/HVV0EbAj8IMOa5UkSZKk3uisRbCq1iV5HXAaMAdYXlUXJjkSWFlVK4BjgU8nuZSmJXD/dtsLk/w78CNgHXBIVd3ZVa2SJEmS1Cdddg2lqk4FTh017/CB57cBLxpn278H/r7L+jZyvesO2zO+v7Ob7+/s5Xs7u/n+zl6+t7Ob7+8Y0vTElCRJkiT1RZfXCEqSJEmS7oMMgvdBSfZJcnGSS5O8dZx1vpbkhiSnjJr/30nOaR+rk5w8PVVrPEmWJ7kmyQUD85b8/+3dffBcVX3H8ffHgFCgCDURlaBBiWK1GECCDEIxKvjABBGZJC3VaLHCiAo64NDWKHQYkaiIoOLYIliTII8angSKLQ+dEGKQp4giQhhRJIIjGIUwIR//OGfNzbr7y+Zhfw/u5zXzm9w9955zz+Z77+49e849V9KtNU4/kDS1S9559Vi4p5azZU0/SNITjVjP6ZQ/+kvSLpL+V9K9kpZJ+mhj3Ydr7JZJOqNL/v+QdFeN4XWSXlzTE98RJmlrSbdJurPG8JSaLkmnSbqvxv0j6ynnbEkrG69nS/p1I7ZH9/u9RHeSxkn6Yeu7tNf4Sjpf0oONOE5p5P9S/f6+S9Jew/l+opC0XNLdre/YmnZkPZfXSOo6e6SkT0v6RSO2b6/pkyQ91Ug/d7jeTwytS7w7xjHW1dd7BGPDSRoHfBl4C+UxGkskLbT9o7ZN5wLbAB9sJto+oFHWpcB3+1vj6MH5wDnANxtpZwCn2L6mfjidARzUIe884Ki6PB84GvhqfX2z7UP7UeHo2Wrg47Zvl/TXwFJJ1wM7AYcBe9heJekFXfLPtf1JgHrBOQc4pq5LfEfWKmCa7ZX1B5hbJF0DvIryeKPdba8ZIrbUi80dOqz6tu3j+lLr2FAfBe4Ftq+vZ9NjfIETbV/SlvY2ykznk4F9KZ/X+27WGkev3mi7+dy4e4B3Ab08lfFM25/rkP4z21M2S+1ic2uPN3SPI1Aai8By2+f3s2KjWXoER5+pwP22H7D9DHAh5YJyHbZvAH7XrZB6UToNSI/gCLN9E2VW3HWSWXvh8Ty6PyfzaleUR6hM7FtFY4PZfsT27XX5d5QLyp2BY4HTba+q61Z0yf9k4+W2lOMiRoF62rV68rasf6bE9lTba+p2HWNbf9SbC5w0DNWNjSBpIvAO4D8byT3FdwiHAd+sx8+twA6SXrRZKhybxPa9tn8y0vWIGE3SEBx9dgZ+3nj9cE3bUIcDN7RdaMbocTwwV9LPgc8BJw+1ce2R+Cfge43k/eqwtWskvbp/VY1eSJoE7AksBl4BHCBpsaQbJe0zRL7T6nHwj5QewZbEd4TVYYN3ACuA620vBl4OzFAZ0n2NpMldsh8HLLT9SId1R9Rhg5dI2qVP1Y/1+yKlob6mkdZrfAFOq3E8U9JWNW1zfYfHpjFwnaSlkv5lI/IfV2N7nqQdG+m71qHEN0o6oGvuGG7d4t0tjlGlITj6qEPaxvQSzAIWbGJdon+OBU6wvQtwAuWZmkP5CnCT7Zvr69uBl9p+LXA26fkdUZK2Ay4Fjq8/vmwB7Ai8HjgRuEhSp3Mb2/9Wj4N5lMYDJL6jgu1n6zCwicBUSa8BtgKetv064OvAee35VO71PJISu3ZXAJNs7wH8D3BBv+of3Uk6FFhhe2nbqvXGtzoZ2B3YB/gb4BOtojtsm57+4be/7b0oQ3U/JOnADcj7VcoPAlOAR4DP1/RHgJfY3hP4GDBf0vadi4hh1ineHeMo6e9a9w1SbsU4tXEf4fNHqP4jJg3B0edhyv0JLROBxxoH6fT1FVAP5KnAVX2qY2y69wKX1eWLKfFC0rU1zn8aqiTpU8AEyhcPUIYUtoat1ed1bilp/HBVPtaqvbWXAvNst2L6MHBZHR52G6XHYbykb9T4Xt2hqPnAEZD4jja2fwv8H/BWSmwvrasuB/aAPzt39wR2A+6XtBzYRtL9tazHW0OGKQ2NvYfrfcQ69gem1/hcCEyT9C16i29rWLhrLL9B/Qyn83d4x6H/0T+2f1n/XUGJY8cJ2QDaP5dtP1p/BFpDOUen1vRVth+vy0uBn1FGf8QI6xTvIeJ4t+0p9Ue+c4E5rdet+A6SNARHnyXAZEm7SnouMBO4pHGQLuyhjCOBK20/3deaxqb4JfD3dXka8FMA24fUOB8NoDKj4CHArNY9KzX9ha0eJpUZR58DDNwH2EirMfgv4F7bX2is+g4lrkh6BfBc4DHb76vxbc1C1xx2Nh34cU1PfEeYpAmSdqjLfwW8mRKfP8WWcg7fB+ueu7avsv1C25NsTwL+YHu3WlbzfrHplPtKY5jZPtn2xBqfmcD3bR9FD/GFtXGs5+k7KRORACwE3qPi9cATXYYHR59I2rbOk4CkbYGDWRufP9Phc7l5jh7eyls/E8bV5ZdRJgR6oD/vInrVLd7d4hjryqyho4zt1ZKOA64FxgHn2V7Wvp2kmynDUraT9DDwz7avratnAqcPV51jaJIWUGYEHV9j9SngA8BZkrYAnga63cNwLvAQsKi2Cy6zfSrwbuBYSauBp4CZdUKZGF77U+7dvLsOMwH4V8pwsvNUHhnyDPDeLvE5XdIrKT2GD7F2xtDEd+S9CLigXvg9B7jI9pWSbgHmSToBWEmZyXdDfKSO7FhNmURq9masc2y60+ktvvMkTaAMBW0NMQO4Gng7cD/wB+B9/a1udLATcHn9ztwCmG/7e5IOpwzXngBcJekO24d0yH+GyuNADCxn7ezsB1KGEa4GngWOsd0+EVwMv27x/u8ucYwG5doiIiIiIiJisGRoaERERERExIBJQzAiIiIiImLApCEYERERERExYNIQjIiIiIiIGDBpCEZERERERAyYNAQjImLMk7STpPmSHpC0VNKiOl38qCVprqRlkuZ2Wf9dSYuGu14RETEY8hzBiIgY0+pDvb8DXGD7H2raSykPbG/fdgvbq4e5it18EJhge1X7ivow+72AlZJ2tf3gsNcuIiL+oqVHMCIixrppwDO2z20l2H7I9tkAkmZLuljSFcB1KuZKukfS3ZJm1O0OknRlqwxJ50iaXZeXS/qspNvq3241/chazp2Sbmqv2BD7WghsCyxupbU5ArgCuBCY2Sjv5ZJulbRE0qmSVjbWnVjT75J0ykb/b0ZExEBIj2BERIx1rwZuX882+wF72P6NpCOAKcBrgfHAkk6NuA6etD1V0nuALwKHAnOAQ2z/ovbitXtXp33Zni5ppe0pXfY1CzgFeBS4BPhMTT8LOMv2AknHtDaWdDAwGZgKCFgo6UDbvbyviIgYQOkRjIiIvyiSvlx76JY0kq+3/Zu6/AZgge1nbT8K3Ajs00PRCxr/7leX/x84X9IHgHEd8mzwviTtBOwG3GL7PmC1pNfU1fsBF9fl+Y1sB9e/H1IaxbtTGoYREREdpUcwIiLGumWUoZQA2P6QpPHADxrb/L6xrC7lrGbdH0i3blvv9mXbx0jaF3gHcIekKbYf72FfQ5kB7Ag8WG5/ZHvK8NB/HyKPgM/Y/tpG7C8iIgZQegQjImKs+z6wtaRjG2nbDLH9TcAMSeMkTQAOBG4DHgL+VtJWkp4HvKkt34zGv4ug3LNne7HtOcBjwC497msos4C32p5kexKwN2vvE7yVtY3emY081wLvl7RdrdfOkl6wnv1ERMQAS49gRESMabYt6Z3AmZJOAn5N6QH8RJcsl1OGWN5J6dk7yfavACRdBNwF/JQyzLJpK0mLKT+izqppcyVNpvTI3VDL7GlfnUiaBLyE0uBrvb8HJT1Zex6PB74l6ePAVcATdZvrJL0KWFR7EVcCRwEruu0rIiIGm2yvf6uIiIgBJmk58Drbj41wPbYBnqqN35nALNuHjWSdIiJibEqPYERExNixN3BOfXbib4H3j3B9IiJijEqPYERERERExIDJZDEREREREREDJg3BiIiIiIiIAZOGYERERERExIBJQzAiIiIiImLApCEYERERERExYNIQjIiIiIiIGDB/BBE2TYl9i9QoAAAAAElFTkSuQmCC
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>As we see above, customers with age between 26 and 35 spend the most on Black Friday. This is useful information if we want to target this group to advertise new products, and blast them with ads reminding them when Black Friday is approaching. It's also apparent that we should not focus on the elderly. Putting commercials television stations frequently viewed by the elderly would not be a good idea. This is because they are highly likely to spend more money than the other groups to buy new products. And people from group of age 0-17 or 55+ spend less money than other. We should limit the ads over these groups because it will cost money if this group is not active shoppers.<br><br>For a more in depth read about age groups and how to maket to them please click the following <a href="https://martech.zone/what-is-generational-marketing/to">link</a> to an artical on generational marketing</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Sum-of-purchases-for-each-product"><section id="sum">Sum of purchases for each product</section><a class="anchor-link" href="#Sum-of-purchases-for-each-product">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>At the end of the day, a retailer would like to know which product has been purchased the most and which product has been purchased the least. It would help a retailer know which items to stock up on, and which items to have less of when Black Friday rolls around. Since we have so many products in our table, we won't be able to graph them all. So we will graph the top 100 purchased products and the bottom 100 purchased product. Then, we can visualize the sum of purchase for the top and bottom 100 products.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>First, let's compute the sum of a purchase for a product</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[12]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">total_purchase_of_a_product</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span>
<span class="n">total_purchase_of_a_product</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">total_purchase_of_a_product</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">total_purchase_of_a_product</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;P&#39;</span><span class="p">,</span> <span class="s1">&#39;&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="nb">int</span><span class="p">)</span>
<span class="n">total_purchase_of_a_product</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Purchase&#39;</span><span class="p">],</span> <span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">total_purchase_of_a_product</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[12]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Product_ID</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>249</th>
      <td>25442</td>
      <td>27532426</td>
    </tr>
    <tr>
      <th>1014</th>
      <td>110742</td>
      <td>26382569</td>
    </tr>
    <tr>
      <th>2441</th>
      <td>255842</td>
      <td>24652442</td>
    </tr>
    <tr>
      <th>1743</th>
      <td>184942</td>
      <td>24060871</td>
    </tr>
    <tr>
      <th>581</th>
      <td>59442</td>
      <td>23948299</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, let's visualize our data:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[13]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">top_100</span> <span class="o">=</span> <span class="n">total_purchase_of_a_product</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">100</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">regplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">top_100</span><span class="p">)</span>

<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">12</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
<span class="n">title</span> <span class="o">=</span> <span class="s2">&quot;Top 100 products that are purchased the most&quot;</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="n">title</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Product ID&#39;</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Purchase in Dollars&#39;</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[14]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">bot_100</span> <span class="o">=</span> <span class="n">total_purchase_of_a_product</span><span class="o">.</span><span class="n">tail</span><span class="p">(</span><span class="mi">100</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">regplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">bot_100</span><span class="p">)</span>

<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">12</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
<span class="n">title</span> <span class="o">=</span> <span class="s2">&quot;Bottom 100 products that are purchased the least&quot;</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="n">title</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Product ID&#39;</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Purchase in Dollars&#39;</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This information is highly valuable especially around this time of year. The best selling Black Friday product are most likely intended to be presents for the holiday season. Retailers should stock up on the top items so they can sell to the holiday buyers.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="-Frequency-Purchase-"><section id="6"> Frequency Purchase </section><a class="anchor-link" href="#-Frequency-Purchase-">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>There are several ways to measure purchase frequency on its own. However, we need to measure whether purchase frequency has increased as a result of the community. For this, we can reuse much of the same process to measure changes in spending.</p>
<p>Frequency of purchase is the number of orders placed by a customer over a defined period of time (typically one month or one year). Greater purchase frequently typically implies higher profitability. An online community might encourage people to use the product more and thus purchase more frequently, or use the product more often and have to replace it most often.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Same as the sum of products, we want to know the top and bottom 100 products.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>First, compute the frequency of a product that is purchased within a group</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[15]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">freq_purchase</span> <span class="o">=</span>  <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">Product_ID</span><span class="o">.</span><span class="n">count</span><span class="p">()</span><span class="o">.</span><span class="n">to_frame</span><span class="p">()</span> <span class="c1"># counting the frequency for each product</span>
<span class="n">freq_purchase</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="o">.</span><span class="n">Product_ID</span> <span class="c1">#create a new column named &quot;Freq&quot;</span>
<span class="n">freq_purchase</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span> 
<span class="n">freq_purchase</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">freq_purchase</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;P&#39;</span><span class="p">,</span> <span class="s1">&#39;&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="nb">int</span><span class="p">)</span>
<span class="n">freq_purchase</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">],</span> <span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">freq_purchase</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[15]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Product_ID</th>
      <th>Freq</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2534</th>
      <td>265242</td>
      <td>1858</td>
    </tr>
    <tr>
      <th>1014</th>
      <td>110742</td>
      <td>1591</td>
    </tr>
    <tr>
      <th>249</th>
      <td>25442</td>
      <td>1586</td>
    </tr>
    <tr>
      <th>1028</th>
      <td>112142</td>
      <td>1539</td>
    </tr>
    <tr>
      <th>565</th>
      <td>57642</td>
      <td>1430</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Then, merge the two tables: freq_purchase and total_purchase_of_a_product</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[16]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Using outer join to merge the two tables together.</span>
<span class="n">freq_purchase</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">total_purchase_of_a_product</span><span class="p">,</span> <span class="n">left_on</span><span class="o">=</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="n">right_on</span><span class="o">=</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="n">how</span><span class="o">=</span><span class="s1">&#39;outer&#39;</span><span class="p">)</span>
<span class="n">freq_purchase</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[16]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Product_ID</th>
      <th>Freq</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>265242</td>
      <td>1858</td>
      <td>13983325</td>
    </tr>
    <tr>
      <th>1</th>
      <td>110742</td>
      <td>1591</td>
      <td>26382569</td>
    </tr>
    <tr>
      <th>2</th>
      <td>25442</td>
      <td>1586</td>
      <td>27532426</td>
    </tr>
    <tr>
      <th>3</th>
      <td>112142</td>
      <td>1539</td>
      <td>23882624</td>
    </tr>
    <tr>
      <th>4</th>
      <td>57642</td>
      <td>1430</td>
      <td>22493690</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Graphing-Frequency-Distribution-of-Top-and-Bottom-100-Purchased-Products">Graphing Frequency Distribution of Top and Bottom 100 Purchased Products<a class="anchor-link" href="#Graphing-Frequency-Distribution-of-Top-and-Bottom-100-Purchased-Products">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[17]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">top_100</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">100</span><span class="p">)</span>

<span class="c1">#Using bar plot to describe the frequency of a product is purchased.</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">top_100</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Freq&#39;</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">25</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
<span class="n">title</span> <span class="o">=</span> <span class="s2">&quot;The most 100 products that are frequently purchased&quot;</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="n">title</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlabel</span><span class="p">(</span><span class="s2">&quot;Product ID&quot;</span><span class="p">)</span> <span class="c1">#Label the x-axis</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="s2">&quot;Frequency Purchased&quot;</span><span class="p">)</span> <span class="c1">#label the y-axis</span>
<span class="n">ax</span><span class="o">.</span><span class="n">get_legend</span><span class="p">()</span><span class="o">.</span><span class="n">remove</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABbMAAAJ7CAYAAADZZwxBAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMS4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvNQv5yAAAIABJREFUeJzs3Xm4LFV5L/7vCzjhgAN4IRA8SFBQSVDRRCMEjkNUcIyKxjwBzVWJ+NP8QnJzzKBbTW64KjExIaLeIGAi4ogDGkXAKXECQzwqJIKiHgERUJzAAdf9o2pL0+zeu8/Qfeqc8/k8Tz27a61VVW9Vdfcfb6/9VrXWAgAAAAAAQ7bd5g4AAAAAAABWIpkNAAAAAMDgSWYDAAAAADB4ktkAAAAAAAyeZDYAAAAAAIMnmQ0AAAAAwOBJZgMAm11VtSmWQ6rqqP717TZ3zJtaVd2yqhaq6oApx76iqj5WVddVVVtm7OOqam1VXV9VX6yqI5YYs1NVvaGqvl1V11bVv1TVXTb2nGalql5ZVZfOYL9PqaqjNsF+7trfy1Vj7Yf079/7bIJjPLCqFjZ2P7NUVb9eVZ/t33sT36Nbukn3on8PXLUZQpqJ/r37vM0dx3Jm9d0AAAyHZDYAMAQPGllW921/Odb+2c0T2tzcMsmLk6yYzE6yY5L/meSHSf590qCqekiStyc5N8mjkpyZ5LSqesTY0NOTHNLv86gkD0hyxnpFv3V4Srrz31h3TXcvV22CfU3ywP4YQ/baJN9J8pvpPsNbqy3hXgAAbBV22NwBAAC01j65+Hpk1vUlo+1931zjGqrW2neq6s6ttcWZkqsnDP2LJB9trT2/Xz+3qu6d5EVJPpgkVfWgdMnG32itfbRv+0aST1XVw1prH9qUsVd3E2/VWrt+U+6XTWsT3ad9k7yutfaRZY5zm9badRtxDDaCzyMAsKUxMxsA2BLtVVVnVdUPquqiqnri+IC+vMZ5fYmDK6rq5VV1i+V2WlUfrqq3VdUzquorVfX9qnpjVd2qLyXw6b7tw1W159i2O1fVKVV1dVX9sB9z4NiYx1bV+X3c366qT1XVb/Td3+v/vmGktMqqSbG21pYt21BVt0pyaJK3jHW9OcmDqmqnfv1RSb65mMju9/3pJF/p+ybtf1Uf42/31+h7VXVlVb14bNxCVV1VVQ+pqs8kuT7Jk/u+varqjKr6br/9e6rql8a2v2NVvam/ZpdX1Z8tEcuS5RyWKotQVc8aKbvyzf5+71RVJyf5rSS/MXL9F/ptHlJdSZfv9ssFVfXkSdclydp+9dzFfY0N27mq3tq/l75cVc8d28eDqurdVXVZf94XVNXTR/qPSvL3I+fYqurDS8XTjzms/7xc2cf/yfHZ+SvcpztX1Wv763V9Vf17Vf3qMsc7pD/n7ZP8XR/fyX3fpVV1fFX9RVWtS/Ldke0eUlUf6T8/V1fV66vq9mP7Priq/rOP4/yqenAf98LImEur6pVj292sRNE059Vv84Kq+t9V9a3+Gp7Qf76mvhdVtUN/P282g7s/53cscz1Pru677PHVfd9dX1Ufr6p7jYxZ/DwevtS2I+vL3ee79Nfj8v4Y/1VVfzAWzvaTrkW/j92q6qT+fX1dVf13Vf1lVd1yLK4XVtXFdePn8F+ratf1vDcrfjcAAFsfM7MBgC3Rm5K8Lskrkvx/Sd5cVXdvra1LutrHSU5LV+bgT5PsneSv0/2Q/0cr7PvXkuzc73fPJK9Kcl2SX03y8iQ/SPLq/viPHNnujCS/1O//qiR/nC6Zed/W2sVVtXeStyX5u77v1knun+TO/fark5yTrrzKmX3b5etzUcbsneQWSS4aa78w3XW4R5LPpJs9Oz5mcdy+UxznFUnem+RJSQ5O8uKquqq1dsLImB2TnJLu+v13ksv6BNjZSX6S5FlJfprkJUk+UlX7t9au6bd9Q7oSKH+Q5Ip013fvfvx6qao/T/LSJP+Y7h7smOSwJLdL8rJ09/uOSRaTy+uq6g79+b2r37aS7N+PW8rlSZ6e5F+SHJOly+O8Pt31eF2SpyU5oarO639ESJK7Jfm3JCemSzb+erofOX7WWjst3fvj+CTH5sbyHd/NZHsleU+SVyb5WbofKd5fVQe31v5tZNyk+/Sh/nz/OMmVSX4/yYeqap/W2hVLHO+zfVyf6ON8W5JvjfT/dpIvpLvOOyRdfe1074cz0r2X7pLkuCR36tdTVb+Q5P1JPt23/UK667zjMue+pPU8r2PTfTZ/J8kvp/su+Wp/naa6F621n1bVKUmOqqqXLv4YVVV3T3JQksetEPLdkvxNuv+2uC7dZ+UDfazrO6t6qft8myQfTlci5yXpvhN+qV9GLXctku6785okf5jk2+m+ZxaS7JLkOf05/2667+U/Sfc+uEu677/b9v3T3ptN9t0AAGxBWmsWi8VisVgsg1nSJRZbkqOW6Duq73vmSNtd0iUvju7XK11y5Q1j2z4zXRLoLssc+8PpavzuNNL2lv6YB4+0Pbdv27Fff2S//hsjY26bLoH32n79SUmu3pDzXuF6PS/9RO2x9l/v93fAWPsv9e2P6NfPSnLGEtv/c5J/X+a4q/r9fHCs/fVJvpFku359oR/3uLFxR/f37e4jbXsk+XGSF/br9+63PWLsOl2T5NKRtoUkVy0RY0vyvP71HdPVGP+bZc7pbUk+PNZ2YL+f26/HPblPv80hY+2H9O0vHWm7Rf8+OW7Cvipdwve1Sc5Z6b5PEdt2/f4+kOSksWu41H36vf6e7DPStkOSS5K8YoVj/fz6j7Rdmi7hf+ux9o8lOXesbXW/j/v06y9PcnX6z13f9vR+zMLYMV45tq+j+nG3W5/z6rf56Ni+zkjyySk+gzd5XybZp9/foSNtL02XiN1hmet4cr/dg0fa7pabfu+t6sccvsS2501xn5+T7oeOA5aJY8VrscQ2O6T78eL6JLfs2/4hyduX2WbFe5MpvxssFovFYrFsfYsyIwDAluiDiy9aa1enm7m3R990j3QzbN/S/2v/DlW1Q7rZhLdOl2hcznmttWtH1i9Ol1j5+Fhb0s0MTboHwH2rjdQGbq39IN2M3of0TWuT7FRdKZJHVNVtpzvVjTZe4qKWaF+qZElNaB/3zrH1d6S7LnuMtLV0M2pHPTDJZ1trX/75oG5m/b/lxmv2gP7vu0fGfD9dAn59PSjJbdLN5lwflyT5fpI3VVe6ZtKM7PUx+v79SZIvZeR6VdWdqurVVfXVdDPXf5Lk2ene2+utqvbo33ffSJcA/UmSRyyxv6Xu08OSnJ/kKyOfpST5SLpE/4Y4u43MJq6qHdPdn/HP7Mf7WO/fD31gkrNaaz8c2dfE8hwrWJ/z+uDY+hdz0/f3VFprX0ry0fQPGa2qSvK7Sd7YWltpNvGVrbWfP+y1tfbVPv4Hrm8cWfo+r07yH621C1bYdtlrUZ0/qKovVtV16e7fvyS5Vbrv5SS5IMmjq+ol1ZVv2n5sn9Pcm0353QAAbEEkswGALdF3xtZ/nC5RnXT/5p4k78uNicCfpKsBnSS/uAH7/l5r7WdjbRk55m5JvrnEvr6ZvoxIa+2/0pUSuHsf21V9vdddVohnQ327/zuefF1c/87IuKUStHfMza/FUq6csL7baCyttR+PjVvxmiXZNd21H39A4Pgxp3GX/u96lW5prX07XeL3Fulm6X+rqs7sy0NsqOXev0k3m/aIdCVcHpEucXfS2JipVNV26RJ+D0734M9D+/29f4n9LXWfdk5XeucnY8szsvJnaZLx+36ndPW1/3HsGD9Kd90Xj7Nrxu59/974/gbEsD7ntdL9Wh//lORJ1dUCX51uhvU0P7As9Z6/Mjf9nE1rqft8l0z32VjpWvxBurIr70z3fffAdOV2MjLupHRlRp6S5FNJvllVLxtJak9zbzbldwMAsAVRMxsA2Nos1lp+dpL/WKL/K0u0bazL09WaHfc/RuJJa+3MJGdW9/DFw5L8bbqHxz11BjFdki4BtG+6GY2L9k1XTuC/+/WL0tXsHbdvuhICKxk/78X10cTYUjO8L09XKmDc6DW7Isntq+o2Y0mr8WNen2T8AXN3Ghtzdf93t3Q1zafWWvtEkkf2dYUflq528ZvSJdw2qaq6dbr3xvNaayeOtG/oJJRfSnLfJI9qrf3ryP5us8TYpe7TNUnOS1ezeNyPNjCm8eN8p29bSPdDz7jL+r9XZOze9+dxu7HxN3s/5MYfSBbN4rym8dZ0NfefnO6HhU+11r44xXZLfb/cNV3N6aQ752Tl806Wvs9X5+b1sTfEk5O8tbX284cxjj6oMkn6HwZfleRVVfWL6UrF/FW68kQnZrp7M+13AwCwlTEzGwDY2vxXuqTIqtbaeUssV6+0gw3wqSR3raqDFxv60gmH5ablSZIkrbVrW2tvSjd7cTHRMz7be6O01n6U5Nx0yaVRRyT5xEgplfcn2bWqFkt7pKoOTDeDfLwUwVKeMLb+xHSJ6nUrbPepJPevqr1Gjrt7uhnEi9fsM/3fx46MuV2Sh4/ta126xNbuI22PGBvziXQ1049cJqZlZ9y21q5rrb0n3czSe00al427l7dKN0v55wnVfhbvY8fG/bjvW+kYi0nr0f3dLV1N9WmcnS7J+bUlPktrp9zHsvqSPJ9Mcs8Jn9nFZPZnkjy8/2wteuISu1yXZL+xtvH3zKY8r2nvxeJM8tPSzVZ+YqYve3PXqnrw4kpV7Znkfukehpl0M5J/kpHz7j8rD8p0zk5y36r65SnHT3Kb3PzHgKdPGtxa+3pr7bh0pZsWP1PT3JtpvxsAgK2MmdkAwFaltfazqjo2yRur6g7pErI/TpecfXySJ43V3N0Ux/xAVf1bktOrak26WY5/lC6x84okqarnpEss/Wu6mab7pEs0n9rv48dV9ZUkT6mqz6ebafm5JcoBpN/fo9I9ZPKAfv1Jfddn+nq6SfKyJB+uqr9NN8v60f3yyJHYP1FVH0hyalX9UbpZ2/8nycdbax+a4vTvXVWvTfL2JAene3jbC8bKsizl5CR/kuT9VfWiJDekf2BeuocdprX2hap6d5LX9Pfy8iR/nO5BjqP+NV2i+qSqOj7JXukeMPlzrbXvVNXLkvxVVd0y3QzgW6X7weElrbVvpJul/riqeny6hOhl6WY1PzPd9ftakt3TPSzvnGXO7Wt9PEdW1bVJftJaO2+F67EY57VV9ZkkL6qq76a7H2uSXJvkDiNDL+r/vqCqzkny3b6UzbiL+nM5vqr+Isntk7wk3Q8+0zg13bX8cFW9MsmX05WkeGCSK1prr5pyPyv5X0nOrqqfpXsQ5/fS1Vg+LMmftdb+O91/MhyT5L1V9TfparO/MN21HvXOJH9fVX+aLun5xNz8vwA25XlNey8W/VN/7OuSvHnKY1yV7jvtL/rtXpougX1y8vPvvXcl+f/7WuvfSXJsbn5tJjk13bX9YFUtpPtRcK8k92itrZlyH0lXs/r5VfWpdP8d8vSMzfjuvy+uSfcDxrXpZqjvk+77YDGWZe/Nenw3AABbGTOzAYCtTmvt9HT1Wg9I92/970jy3CSfzY2zZje1J6RL5Pxtf8xKsrq1tviwyM8l2SVdiYoPJvnzJK/PjQmcpEvg7JzkQ+mScL+QyV7TH+f3+vW39suhiwNaax9P8qR0pTE+kG4W42+31sYf4vbUdKVITkqXSDo/N59xPcn/SpdkfXu6JO/LkvzDShv1M8cfli4R+E9JTkny1SSHtNauGRl6VLrr9bf9uLMzlgBsrV2V5LfSPYjujCS/k+S3lzjmX6crXfCwJO9KlzS/Y7rEadLVbP5guuvwmXSlai5OV5bhf/d9L0+XPH/mMud2fZJnpXtw4Udy4yzSaf12unI4pyb5u3TX9tSxMR9L90PJC9LNcn/thFh+lC6Z+9N0SeKXJfnr3LT0zET9uRya7r39knTX4O/SJR8/vcym66V/rx6c7jPyxiTvSffe+nr6Gtv9Dw6PTvcZeXu6z/Tv5OYJzNele788P12d8x8n+csZntdU92Lk2Oel+zHhHWMPm13OV9MlaxfSvf+/m+Q3Rx+kmeR56R6g+o9JTkg3A3y5H11GY7o+XQ3v96RLlL8/3fW/bLntlvDS/rh/2f/9cbr7MOoT6e71G9L9qPSEJM9qrZ0xEss09+aorPDdAABsfaq1aR5SDwAAN6qqVekSro9prb1380bDtqyqrkryD621hc0dyzT6GtJfSPKw1trZU4w/Ocl9WmsHzjo2AIChU2YEAABgxqrqLknumW52/Ocz5axpAABupMwIAADA7D0m3cNNd0tyVPMvsgAA602ZEQAAAAAABs/MbAAAAAAABk8yGwAAAACAwdtqHwC58847t1WrVm3uMAAAAAAAWMb5559/VWttl5XGbbXJ7FWrVuW8887b3GEAAAAAALCMqvrqNOOUGQEAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMHbYXMHMA+r1pw5se/S4w6bYyQAAAAAAGwIM7MBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABi8mSWzq+qkqrqyqj4/0nZ6VV3QL5dW1QV9+6qqum6k78SRbe5fVWur6uKqenVV1axiBgAAAABgmHaY4b5PTvIPSU5dbGitHbH4uqqOT3LtyPhLWmsHLLGf1yR5dpJPJnlfkkcmef8M4gUAAAAAYKBmNjO7tfbRJNcs1dfPrn5KktOW20dV7ZbkDq21T7TWWrrE+OM3dawAAAAAAAzb5qqZfVCSb7bWvjTStldV/UdVfaSqDurbdk+ybmTMur4NAAAAAIBtyCzLjCznabnprOzLk+zZWru6qu6f5IyquneSpepjt0k7rapnpytJkj333HMThgsAAAAAwOY095nZVbVDkicmOX2xrbX2o9ba1f3r85NckuQe6WZi7zGy+R5JLpu079ba61prB7bWDtxll11mET4AAAAAAJvB5igz8rAkF7XWfl4+pKp2qart+9d3T7JPki+31i5P8r2q+rW+zvbvJnnXZogZAAAAAIDNaGbJ7Ko6LcknktyzqtZV1e/1XU/NzR/8eHCSz1XVfyZ5W5KjW2uLD4/8/ST/N8nF6WZsv39WMQMAAAAAMEwzq5ndWnvahPajlmh7e5K3Txh/XpL7bNLgAAAAAADYomyOMiMAAAAAALBeJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZvh80dwKAt7LRM37XziwMAAAAAYBtnZjYAAAAAAINnZvYM7H/K/hP71h65do6RAAAAAABsHczMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwdthcwfAjS7cd7+JfftddOEcIwEAAAAAGBYzswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGb2bJ7Ko6qaqurKrPj7QtVNU3quqCfnn0SN8Lq+riqvqvqvrNkfZH9m0XV9WaWcULAAAAAMBwzXJm9slJHrlE+6taawf0y/uSpKruleSpSe7db/OPVbV9VW2f5IQkj0pyryRP68cCAAAAALAN2WFWO26tfbSqVk05/HFJ3txa+1GSr1TVxUke2Pdd3Fr7cpJU1Zv7sV/cxOECAAAAADBgm6Nm9vOq6nN9GZI79W27J/n6yJh1fdukdgAAAAAAtiHzTma/JsneSQ5IcnmS4/v2WmJsW6Z9SVX17Ko6r6rO+9a3vrWxsQIAAAAAMBBzTWa31r7ZWruhtfazJK/PjaVE1iX5xZGheyS5bJn2Sft/XWvtwNbagbvsssumDR4AAAAAgM1mrsnsqtptZPUJST7fv353kqdW1a2qaq8k+yT5dJLPJNmnqvaqqlume0jku+cZMwAAAAAAm9/MHgBZVaclOSTJzlW1LsmLkxxSVQekKxVyaZLnJElr7QtV9ZZ0D3b8aZJjWms39Pt5XpIPJNk+yUmttS/MKmYAAAAAAIZpZsns1trTlmj+p2XG/1WSv1qi/X1J3rcJQwMAAAAAYAsz7wdAAgAAAADAepPMBgAAAABg8CSzAQAAAAAYPMlsAAAAAAAGTzIbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8yWwAAAAAAAZPMhsAAAAAgMGTzAYAAAAAYPAkswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8HbY3AGw8U44+pyJfcecuHqOkQAAAAAAzIaZ2QAAAAAADJ6Z2duw4484fGLfsae/d46RAAAAAAAsz8xsAAAAAAAGz8xs1tu6NR+b2LfHcQfNMRIAAAAAYFthZjYAAAAAAIMnmQ0AAAAAwOBJZgMAAAAAMHiS2QAAAAAADJ5kNgAAAAAAg7fD5g6AbcfCwsIG9QEAAAAAmJkNAAAAAMDgSWYDAAAAADB4yowweGefs/fEvoeuvmRi367nXjCx74pDD9iomAAAAACA+TIzGwAAAACAwZPMBgAAAABg8JQZgTGr1pw5se/S4w6bYyQAAAAAwCIzswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8DwAEjaRSQ+O9NBIAAAAANh4ZmYDAAAAADB4ktkAAAAAAAyeMiOwOS3stEzftfOLAwAAAAAGzsxsAAAAAAAGz8xs2ALtf8r+E/vWHrl2jpEAAAAAwHyYmQ0AAAAAwOCZmQ3bkAv33W9i334XXTjHSAAAAABg/ZiZDQAAAADA4ElmAwAAAAAweJLZAAAAAAAMnmQ2AAAAAACDJ5kNAAAAAMDgSWYDAAAAADB4ktkAAAAAAAyeZDYAAAAAAIMnmQ0AAAAAwOBJZgMAAAAAMHiS2QAAAAAADJ5kNgAAAAAAgyeZDQAAAADA4ElmAwAAAAAweJLZAAAAAAAMnmQ2AAAAAACDJ5kNAAAAAMDgzSyZXVUnVdWVVfX5kbZXVNVFVfW5qnpnVd2xb19VVddV1QX9cuLINvevqrVVdXFVvbqqalYxAwAAAAAwTLOcmX1ykkeOtZ2V5D6ttV9O8t9JXjjSd0lr7YB+OXqk/TVJnp1kn34Z3ycAAAAAAFu5HWa149baR6tq1VjbB0dWP5nkScvto6p2S3KH1ton+vVTkzw+yfs3abDAsk44+pyJfcecuHqOkQAAAACwrdqcNbOfmZsmpfeqqv+oqo9U1UF92+5J1o2MWde3AQAAAACwDZnZzOzlVNWfJflpkn/pmy5Psmdr7eqqun+SM6rq3kmWqo/dltnvs9OVJMmee+65aYMG1tvxRxw+se/Y0987x0gAAAAA2NLNfWZ2VR2Z5PAkT2+ttSRprf2otXZ1//r8JJckuUe6mdh7jGy+R5LLJu27tfa61tqBrbUDd9lll1mdAgAAAAAAczbXZHZVPTLJnyR5bGvthyPtu1TV9v3ru6d70OOXW2uXJ/leVf1aVVWS303yrnnGDAAAAADA5jezMiNVdVqSQ5LsXFXrkrw4yQuT3CrJWV1uOp9srR2d5OAkL62qnya5IcnRrbVr+l39fpKTk9wmXY1tD38EAAAAANjGzCyZ3Vp72hLN/zRh7NuTvH1C33lJ7rMJQwMAAAAAYAuzWR4ACbCcdWs+NrFvj+MOmmMkAAAAAAzF3B8ACQAAAAAA68vMbGCrsbCwsEF9Z5+z98S+h66+ZCMiAgAAAGBTMTMbAAAAAIDBk8wGAAAAAGDwJLMBAAAAABg8NbMBNtCu514wse+KQw+YYyQAAAAAWz8zswEAAAAAGDzJbAAAAAAABk8yGwAAAACAwZPMBgAAAABg8DwAEmDOVq05c2LfpccdNsdIAAAAALYcZmYDAAAAADB4ZmYDbCE2eEb3wk7L9F27EREBAAAAzI+Z2QAAAAAADJ6Z2QAsaf9T9p/Yt/bItXOMBAAAAMDMbAAAAAAAtgBmZgOwSV24734T+/a76MI5RgIAAABsTSSzARiEE44+Z2LfMSeunmMkAAAAwBBNTGZX1Z2X27C1ds2mDwcA1s/xRxw+se/Y0987x0gAAACAWVpuZvb5SVqSSrJnkm/3r++Y5GtJ9pp5dAAwI+vWfGxi3x7HHTTHSAAAAIBpTHwAZGttr9ba3ZN8IMljWms7t9bukuTwJO+YV4AAAAAAADAxmT3iAa219y2utNaLo/qWAAAgAElEQVTen+Q3ZhcSAAAAAADc1DQPgLyqqv48yT+nKzvyO0munmlUAAAAAAAwYpqZ2U9LskuSd/bLLn0bAAAAAADMxYozs1tr1yR5QVXdrrX2/TnEBAAAAAAAN7FiMruqHpzk/ya5XZI9q+pXkjyntfbcWQcHAEOzsLCwQX0AAADAxpmmzMirkvxm+jrZrbX/THLwLIMCAAAAAIBR0ySz01r7+ljTDTOIBQAAAAAAlrRimZEkX+9LjbSqumWS5ye5cLZhAcDW5exz9p7Y99DVl8wxEgAAANgyTTMz++gkxyTZPcm6JAf06wAAAAAAMBcrzsxurV2V5OlziAUAAAAAAJa04szsqnp5Vd2hqm5RVWdX1VVV9TvzCA4AAAAAAJLpyow8orX23SSHpyszco8kfzzTqAAAAAAAYMQ0D4C8Rf/30UlOa61dU1UzDAkAWLTruRcs2X7FoQfMORIAAADYvKZJZr+nqi5Kcl2S51bVLkmun21YAAAAAABwoxXLjLTW1iR5UJIDW2s/SfKDJI+bdWAAAAAAALBompnZSbJ7kodX1a1H2k6dQTwAwEZatebMiX2XHnfYHCMBAACATWfFZHZVvTjJIUnuleR9SR6V5OORzAYAAAAAYE5WLDOS5ElJHprkitbaM5L8SpJbzTQqAAAAAAAYMU0y+7rW2s+S/LSq7pDkyiR3n21YAAAAAABwo2lqZp9XVXdM8vok5yf5fpJPzzQqAAAAAAAYsWIyu7X23P7liVX1r0nu0Fr73GzDAgDmzYMjAQAAGLJpZmanqnZPcrfF8VV1cGvto7MMDAAAAAAAFq2YzK6q/5PkiCRfTHJD39ySSGYDAAAAADAX08zMfnySe7bWfjTrYAAAAAAAYCnbTTHmy0luMetAAAAAAABgkokzs6vq79OVE/lhkguq6uwkP5+d3Vp7/uzDAwAAAACA5cuMnNf/PT/Ju+cQCwAAAAAALGliMru1dkqSVNVtk1zfWruhX98+ya3mEx4AAAAAAExXM/vsJLcZWb9Nkg/NJhwAAAAAALi5aZLZt26tfX9xpX+94+xCAgAAAACAm5ommf2Dqrrf4kpV3T/JdbMLCQAAAAAAbmq5B0AuekGSt1bVZf36bkmOmF1IAAAAAABwU8sms6tquyS3TLJvknsmqSQXtdZ+MofYAAAAAAAgyQrJ7Nbaz6rq+Nbag5J8fk4xAQAAAADATUxTM/uDVfVbVVUzjwYAAAAAAJYwTc3sP0xy2yQ/rarr05Uaaa21O8w0MgAAAAAA6K2YzG6t3X4egQAAAAAAwCQrJrOr6uCl2ltrH9304QAAAAAAwM1NU2bkj0de3zrJA5Ocn2T1TCICAAAAAIAxKz4AsrX2mJHl4Unuk+Sb0+y8qk6qqiur6vMjbXeuqrOq6kv93zv17VVVr66qi6vqc1V1v5FtjuzHf6mqjlz/0wQAAAAAYEu2YjJ7CevSJbSncXKSR461rUlydmttnyRn9+tJ8qgk+/TLs5O8JumS30lenORX080Kf/FiAhwAAAAAgG3DNDWz/z5J61e3S3JAkv+cZuettY9W1aqx5sclOaR/fUqSDyf5k7791NZaS/LJqrpjVe3Wjz2rtXZNH89Z6RLkp00TAwAAAAAAW75pamafN/L6p0lOa63920Yc83+01i5Pktba5VV117599yRfHxm3rm+b1A4ADMHCTsv0XTu/OAAAANiqLZvMrqr7JvlBki+01i6ccSy1RFtbpv3mO6h6droSJdlzzz03XWQAAAAAAGxWE2tmV9WLkpye5LeSnFlVz9pEx/xmXz4k/d8r+/Z1SX5xZNweSS5bpv1mWmuva60d2Fo7cJdddtlE4QIAAAAAsLkt9wDII5Ic0Fp7WpIHpJ/xvAm8O8mR/esjk7xrpP13q/NrSa7ty5F8IMkjqupO/YMfH9G3AQAAAACwjViuzMj1rbUfJklr7eqqWi7xvaSqOi3dAxx3rqp1SV6c5Lgkb6mq30vytSRP7oe/L8mjk1yc5IdJntEf+5qqelmSz/TjXrr4MEgAAAAAALYNyyWz966qd/eva2w9rbXHrrTzflb3Uh66xNiW5JgJ+zkpyUkrHQ8AAAAAgK3Tcsnsx42tv3KWgQAAAAAAwCQTk9mttY/MMxAAAAAAAJhkvetgAwAAAADAvElmAwAAAAAweMvVzE6SVNV9Wmufn0cwAMC2Y/9T9p/Yt/bItRP7Ltx3v4l9+1104UbFBAAAwHCtmMxOcmJV3TLJyUne1Fr7zmxDAgDY9E44+pyJfcecuHqOkQAAALAhVkxmt9YeUlX7JHlmkvOq6tNJ3tBaO2vm0QEAbGbHH3H4xL5jT3/vHCMBAADYtk0zMzuttS9V1Z8nOS/Jq5Pct6oqyZ+21t4xywABALZE69Z8bGLfHscdNMdIAAAAtg7T1Mz+5STPSHJYkrOSPKa19tmq+oUkn0gimQ0AsIksLCxsUN/Z5+w9se+hqy/ZiIgAAACGYZqZ2f+Q5PXpZmFft9jYWrusn60NAMAWatdzL5jYd8WhB8wxEgAAgOVNk8x+dJLrWms3JElVbZfk1q21H7bW3jjT6AAAGKRVa86c2HfpcYfNMRIAAGBbMU0y+0NJHpbk+/36jkk+mOTBswoKAICtkyQ4AACwobabYsytW2uLiez0r3ecXUgAAAAAAHBT0ySzf1BV91tcqar7J7lumfEAAAAAALBJTVNm5A+SvLWqLuvXd0tyxOxCAgAAAACAm1oxmd1a+0xV7ZvknkkqyUWttZ/MPDIAAAAAAOhNMzM7SR6QZFU//r5VldbaqTOLCgAARi3stEzftRO79j9l/4l9a49cuzERAQAAc7ZiMruq3phk7yQXJLmhb25JJLMBANgqXbjvfhP79rvowol9Jxx9zsS+Y05cvVExAQDAtm6amdkHJrlXa63NOhgAAAAAAFjKdlOM+XySXWcdCAAAAAAATDLNzOydk3yxqj6d5EeLja21x84sKgAAAAAAGDFNMnth1kEAAMC27PgjDp/Yd+zp751jJAAAMFwrJrNbax+pqrsl2ae19qGq2jHJ9rMPDQAAWM66NR+b2LfHcQfNMRIAAJi9FWtmV9WzkrwtyWv7pt2TnDHLoAAAAAAAYNQ0ZUaOSfLAJJ9Kktbal6rqrjONCgAAmJmFhYX1agcAgCGYJpn9o9baj6sqSVJVOyRpM40KAAAYlLPP2Xti30NXXzKxb9dzL5jYd8WhB0zsW7XmzIl9lx532CbfLgs7LdN37eQ+AADmZsUyI0k+UlV/muQ2VfXwJG9N8p7ZhgUAAAAAADeaJpm9Jsm3kqxN8pwk70vy57MMCgAAAAAARq1YZqS19rMkr+8XAAAAAACYuxWT2VX1lSxRI7u1dveZRAQAAAAAAGOmeQDkgSOvb53kyUnuPJtwAAAAAADg5lasmd1au3pk+UZr7W+TrJ5DbAAAAAAAkGS6MiP3G1ndLt1M7dvPLCIAAAAAABgzTZmR40de/zTJpUmeMpNoAAAAtiD7n7L/xL61R66dYyQAAFu/FZPZrbVD5xEIAAAAAABMMk2ZkT9crr+19jebLhwAAAAAALi5acqMHJjkAUne3a8/JslHk3x9VkEBAAAAAMCoaZLZOye5X2vte0lSVQtJ3tpa+5+zDAwAAAAAABZtN8WYPZP8eGT9x0lWzSQaAAAAAABYwjQzs9+Y5NNV9c4kLckTkpw606gAAAC2Yhfuu9/Evv0uunCOkQAAbDlWTGa31v6qqt6f5KC+6Rmttf+YbVgAAACMO+Hocyb2HXPi6jlGAgAwf9OUGUmSHZN8t7X2d0nWVdVeM4wJAAAAAABuYsWZ2VX14iQHJrlnkjckuUWSf07y67MNDQAAgE3h+CMOn9h37OnvnWMkAAAbbpqa2U9Ict8kn02S1tplVXX7mUYFAADAZrduzccm9u1x3EET+wAAZmGaZPaPW2utqlqSVNVtZxwTAAAAW7CFhYUN6jv7nL0n9j109SUbEREAsDWYJpn9lqp6bZI7VtWzkjwzyetnGxYAAABMZ9dzL5jYd8WhB8wxEgBgllZMZrfWXllVD0/y3XR1s1/UWjtr5pEBAAAAAEBv2WR2VW2f5AOttYclkcAGAABgq7FqzZkT+y497rA5RgIATGPZZHZr7Yaq+mFV7dRau3ZeQQEAAMBQSYIDwOYxTc3s65OsraqzkvxgsbG19vyZRQUAAABbm4WdlukzfwwAVjJNMvvMfgEAAADmbP9T9p/Yt/bItRP7Ltx3v4l9+1104UbFBACbw8RkdlXt2Vr7WmvtlHkGBAAAAAAA47Zbpu+MxRdV9fY5xAIAAAAAAEtarsxIjby++6wDAQAAADa/E44+Z2LfMSeunmMkAHBTy83MbhNeAwAAAADAXC03M/tXquq76WZo36Z/nX69tdbuMPPoAAAAgC3C8UccvmT7sae/d86RALC1mpjMbq1tP89AAAAAgG3LujUfm9i3x3EHTexbWFjYoL6zz9l7Yt9DV18ysQ+AYVhuZjYAAADANm/Xcy+Y2HfFoQdM7Fu15syJfZced9hGxQSwLZLMBgAAABiQDU6CL+y0TN+1E7v2P2X/iX1rj1w7eZ8Ac7bcAyABAAAAAGAQJLMBAAAAABi8uZcZqap7Jjl9pOnuSV6U5I5JnpXkW337n7bW3tdv88Ikv5fkhiTPb619YH4RAwAAADDuwn33m9i330UXTuw74ehzJvYdc+LqjYoJ2LrNPZndWvuvJAckSVVtn+QbSd6Z5BlJXtVae+Xo+Kq6V5KnJrl3kl9I8qGqukdr7Ya5Bg4AAADAZnP8EYdP7Dv29PfOMRJgc9ncZUYemuSS1tpXlxnzuCRvbq39qLX2lSQXJ3ngXKIDAAAAAGAQNncy+6lJThtZf15Vfa6qTqqqO/Vtuyf5+siYdX0bAAAAAADbiLmXGVlUVbdM8tgkL+ybXpPkZUla//f4JM9MUkts3ibs89lJnp0ke+655yaOGAAAAIAtzbo1H5vYt8dxB03sW1hY2KA+YHY2WzI7yaOSfLa19s0kWfybJFX1+iSLxY7WJfnFke32SHLZUjtsrb0uyeuS5MADD1wy4Q0AAAAAs3L2OXtP7Hvo6ksm9u167gUT+6449ICJfavWnDmx79LjDtvk28HmtDmT2U/LSImRqtqttXZ5v/qEJJ/vX787yZuq6m/SPQBynySfnmegAAAAAECShZ2W6bt2fnGwTdosyeyq2jHJw5M8Z6T55VV1QLoSIpcu9rXWvlBVb0nyxSQ/TXJMa+2G+UYMAAAAAGyo/U/Zf2Lf2iPXzjEStmSbJZnd/h97dx4vOVnlf/x7uhsVaGwW2WRVFBFkERBRnAEUFVwAFR3AUXAE9IcK7qIyw4zjgo7iDI6oyOYGKojQKsjuiuxbA80miyCggII4rsDz++M8l04XlVRyUpWbC5/361WvW7eqTpJKni0nqSSlP0laYeC1N1R8/mOSPjbp5QIAAAAAAADQHwvXe+bQ1595zcKOlwR9MJ2XGQEAAAAAAACAsfr8W88ufe9tX3xh6Xuf+adXlL73nm99v/Q9bjLaHZLZAAAAAAAAADBDPJZvMjorFAUAAAAAAAAAQIdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6j2Q2AAAAAAAAAKD3SGYDAAAAAAAAAHqPZDYAAAAAAAAAoPdIZgMAAAAAAAAAeo9kNgAAAAAAAACg90hmAwAAAAAAAAB6b9qS2WZ2s5ktMLPLzOyi/NryZnaGmV2f/y6XXzczO9TMbjCzK8xs0+labgAAAAAAAABA96b7zOxtU0qbpJQ2z/8fIOmslNLTJZ2V/5ekHSQ9PT/2kfSFzpcUAAAAAAAAADBtpjuZPWgnSV/Jz78iaefC619N7jxJy5rZqtOxgAAAAAAAAACA7k1nMjtJOt3MLjazffJrK6eU7pCk/Hel/Ppqkm4txN6WXwMAAAAAAAAAPAbMmcZ5b5VSut3MVpJ0hpldU/FZG/JaesSHPCm+jyStueaa41lKAAAAAAAAAMC0m7Yzs1NKt+e/v5X0XUlbSPrN1OVD8t/f5o/fJmmNQvjqkm4fMs3DU0qbp5Q2X3HFFSe5+AAAAAAAAACADk1LMtvMljazZaaeS3qJpCslzZe0R/7YHpJOzs/nS3qjuS0l3Td1ORIAAAAAAAAAwKPfdF1mZGVJ3zWzqWU4NqX0QzO7UNK3zezNkn4l6bX586dIepmkGyT9SdKbul9kAAAAAAAAAMB0mZZkdkrpRkkbD3n9HkkvGvJ6kvS2DhYNAAAAAAAAANBD03bNbAAAAAAAAAAA6iKZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3iOZDQAAAAAAAADoPZLZAAAAAAAAAIDeI5kNAAAAAAAAAOg9ktkAAAAAAAAAgN4jmQ0AAAAAAAAA6D2S2QAAAAAAAACA3us8mW1ma5jZOWa20MyuMrP98+v/bma/NrPL8uNlhZgPmtkNZnatmb2062UGAAAAAAAAAEyvOdMwzwckvSeldImZLSPpYjM7I7/32ZTSp4sfNrP1Je0qaQNJT5Z0ppmtm1J6sNOlBgAAAAAAAABMm87PzE4p3ZFSuiQ/v1/SQkmrVYTsJOmbKaW/ppRuknSDpC0mv6QAAAAAAAAAgL6Y1mtmm9nakp4t6fz80tvN7AozO8rMlsuvrSbp1kLYbapOfgMAAAAAAAAAHmWmLZltZnMlfUfSO1NKf5D0BUnrSNpE0h2SPjP10SHhqWSa+5jZRWZ20V133TWBpQYAAAAAAAAATIdpSWab2RLyRPY3UkonSlJK6TcppQdTSg9J+rIWXUrkNklrFMJXl3T7sOmmlA5PKW2eUtp8xRVXnNwXAAAAAAAAAAB0qvNktpmZpCMlLUwpHVJ4fdXCx14l6cr8fL6kXc3s8Wb2FElPl3RBV8sLAAAAAAAAAJh+c6ZhnltJeoOkBWZ2WX7tQ5J2M7NN5JcQuVnSWyQppXSVmX1b0tWSHpD0tpTSg50vNQAAAAAAAABg2nSezE4p/UzDr4N9SkXMxyR9bGILBQAAAAAAAADotWm7ASQAAAAAAAAAAHWRzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO+RzAYAAAAAAAAA9B7JbAAAAAAAAABA75HMBgAAAAAAAAD0HslsAAAAAAAAAEDvkcwGAAAAAAAAAPQeyWwAAAAAAAAAQO/NmGS2mW1vZtea2Q1mdsB0Lw8AAAAAAAAAoDszIpltZrMlfV7SDpLWl7Sbma0/vUsFAAAAAAAAAOjKjEhmS9pC0g0ppRtTSn+T9E1JO03zMgEAAAAAAAAAOjJTktmrSbq18P9t+TUAAAAAAAAAwGOApZSmexlGMrPXSnppSmmv/P8bJG2RUnrHwOf2kbRP/vcZkq4tmeSTJN0dWJRIXJfzIo444h47cTNhGYkjjriZFzcTlpE44oibeXEzYRmJI464mRc3E5aROOKIqx+3VkppxZFTSCn1/iHpeZJOK/z/QUkfbDG9i7qK63JexBFH3GMnbiYsI3HEETfz4mbCMhJHHHEzL24mLCNxxBE38+JmwjISRxxx44krPmbKZUYulPR0M3uKmT1O0q6S5k/zMgEAAAAAAAAAOjJnuhegjpTSA2b2dkmnSZot6aiU0lXTvFgAAAAAAAAAgI7MiGS2JKWUTpF0ypgmd3iHcV3OizjiiHvsxM2EZSSOOOJmXtxMWEbiiCNu5sXNhGUkjjjiZl7cTFhG4ogjbjxxD5sRN4AEAAAAAAAAADy2zZRrZgMAAAAAAAAAHsNIZgMAAAAAAAAAeo9kNgAAAAAAAACg9x4TyWwzW2LIa0+awHxmm9lbzOw/zWyrgfcOHPf8utbm+5nZS83szWa29sDr/9Kn5cT0Y/sNF61DZraemb3IzOYOvL79+Jey1XKG24iu2viZouttHtW2rne53SPz6rLfy9N9opmtM+T1jWrENvp+tNPlut7uM8GjvbzMlDFumzYC6DPGgUDMo71/bmMmjeMD8wrtK/ZtH/NRncw2s23N7DZJt5vZ6QMF8fQJzPJLkraWdI+kQ83skMJ7r64zgSadcS7wnzCzr5nZ7gPvHVZ/sWsLfT8z+7ikD0vaUNJZZvaOwttv79Fybmhm55nZrWZ2uJktV3jvgnHHFT7zqDzYYmZrmNk3zeynZvah4vc0s5MqQlvXo0nruqxE65CZ7SfpZEnvkHSlme1UePvjVd8xosVyRuM6bePb1vUW823SL4S3eds+JdCWRdvqzrZ7dF4tynS0jXidpGskfcfMrjKz5xTePqYiLroue99OS93X2WkY74TMlPHjTDCObd6w7Yy2m9E2Ylr6vTz9iY+PW7S5oTFui/mF6mx0OQufaXqgs+v10uk4MGIaylg0rnW/0KS8tCjTna7Ptrpox/I0O93vfgyszxkxjo+w4L5ii7jJlZWU0qP2IelCSRvk57tIul7Slvn/S0fEbijpPEm3Sjpc0nKF9y4oibmi8HxOjjtR0uNrzG9bSbdJukve+a5deO+SkpjvSDpY0s6S5uf/H18Vk99bQ9I3Jf1U0ockLVF476SKuND3k7RA0pz8fFlJp0j67KjtMA3L+TNJ2+dlfK+kqyStU2M5o3GNt9AIju4AACAASURBVHm0bOb3jpB0rKR3SrpY0iE15xfdDmdIequkTSR9TtK5klaosV6i2y+6XiJ1veuyEq1DCyTNzc/XlnSRpP0nWPfaLGckLtTGtygr0e0XnV+kXwht8/x+tE+JtmXRut7Zdm8xr2iZjpaxyyStmp9vIR8Qv3qCdaj37XTL9RmdX3S7d71eonU9Or9oeYn2RdG4SBsR2ub5/UgbH12X0TYiVIdalpfIeum6jYiOcaPzi9bZ6HJG+/Wu10u0D+uyjei6jEXjQmWsRZ2Nlumu12dn7VjL+XW93x2dX7TuRddn1/u0XY/jo+OWSH4gGhcqK3Ue4cCZ8JB0+cD/G0i6VtKrqgp9tCBKumbIa/8m6eeSrh8xv8adsaTLBv7/cJ7XCiMqdbTxCX0/SQsH/p8t6UhJx0u6qkfLObg+t53aDiPWZzQuOgCLNpJdd1aD6+Wfp5Z1xHqJbr/OEszTUFaidejqgf/nSvqhpEMGl2VM2zy6nNG4UBvfoqxEt19nO2nRbV7y/er2KdG2LFrXO9vuLeYVLdPRMrZg4P9V5Qct9xsRF/1+vW+nW67P6Pyi232610vduh6dX7S8dJ3MibQRoW2ePxtp46PrMtpGhOpQy/ISWS9dtxHRMe645le3zkaXM9qvd71eon1Yl23EdJexaFytMhYtL2Ms05Nen10faBlXWzbp/e7o/KJ1L7o+u96n7XocH2mTovmBaFyorNR5hANnwkN+tGCVgddWlx/5uH9EbOOCKOnrkrYf8vpekv4+Yn6NO2NJCyXNGnhtj1w4bhl3gYp+P0nfl7T1kNc/KumhHi3n5ZLmDby2Ud7u90wiruk2j5bN/LmuO6urJD1h4LXtJN0g6Y4JbL/OEszTUFaidehsSZsMvDZH0lclPTiBbR5dzmhcqI1vUVai26+znbToNs+fi/Yp0bYsWtc72+4t5hUt09Eydq7y4LXw2hMlnSXprxNYl71vp1uuz+j8xjXemfgB0mBdj85vXOWl62ROnTYitM2nyufA/3Xa+Oi6jLYRoTrUsrxE1kvXbUR0jBudX7TOhpez6TaYpvUyrvHAJNuIrstYNC5UxqLlpUWZ7np9dn2gJTq/rve7x7U+69a9ca3PSe/Tdj2Oj7RJ0fxANC5UVuo8woEz4ZFX0sZDXl9W0odHxIYHb8FlbdwZS/qUpO2GvL69qpOTEytQJfNbUtKSJe+t1qPl3F35CN/A62tK+vIE4qIDsGgj2XVn9S4N7wSeLemMCWy/zhLM01BWonVo9cEyVnhvqwls8+hyRuNCbXyLshLdfp3tpEW3eX4/2qeEDxxHHl1u9xbzipbpaBnbWNLTh7y+hKTXj3tdtth2XR8I7LrORrd71+slWte7Hht3ncyJtBGhbZ7f76ztbNFGhOpQy/IZ6fu6biNCY9wW84vW2ehyRvdRul4v0T66yzai6zIWjQuVsWh5aVGmu16fXR9oic6v6/3u6PqM1r3o+ux6n7brcXykTYrmB6JxEyubYy3UM+EhadOanwsP3gY+/9Wan+tsh3KcBaru9xsS9/EZspwrTSouus3HVTano7y0WIaR269F5zGuuj6xslISN7IOlcTt2+U2b7Gc0biRbfw461DNut7pTlpkm7d5jLP/atFWd7bd644jhsRFy3S0jdhxUusyuu2mu52uuz7HPL86451pXy81v8s410ud8tJ1MmdcbUStuj7GNj7abkbbiFptUpd9X9dtxDgfXc+v5jJ1eqBznOul5nhgutuI3m3zmVxeJrk+u2zH2sxvzN851KfUnHa07kXXZx/2aSc2jh9jmxTaV4zGjetheSEelcxs08GX5HfgfKUkSyld0nB6K6WUflvx/vwh89tWfkq+Uko7NpzfpoFlPDul9MImMQ2mHfp+ZnbokLg3yH+SoJTSfj1ZzuWHxF0sb+wspfS7ccaVTKvxNs9xlWWzIu6rKaU3No2LMrPrUkrrjvjM2OpRi/Uyqq53WlaidcjM3j0k7oPKdxxOKR3yiKAWWixnNG5sbXydsjLmuh4tm5VtxLi3ebRPqdOWtWirO9vu0Xm1KNPRNmLwjvMm6fOS9s3zO7EkLvr9et9O5890WmfHOd6Z5HopiYvW9TrrZazj4y7VaCPGOsat0cZH281oGzG2OpSnN5G+LzqvMbcRdca445xftM6OXM6SuOg+ysTWy7j39SMmtc9QMq3otovGhfMKk8pj9GR9dtaOtZxf1/vdofUZFV2fNac9I8bxJdMa1SaF9hXHuY85rrIyp+0Eeu4i+d09/1p4bQX5RcqTpNLGsqQgXmBmVQVxdUlXSzoiT98kbS7pM6MWtKwzNrPSztjMrhgSs+7U6ymljUbNtzCtOgUq+v1eLelH8jvPWn5tV3nFbmTCy3m3pFsGXltN0iV5Ok8dZ1xkm+e4SNks7azMbFlp/J2Vmd0v//5T85KkpaZeTyk9sSQ0tP1arJdIXKdlRfE69B/yuy9fVYibLWmZEXGPULPuRZczGhdq46NlRfG6Hi2bkTYivM2jfUq0LVO8re5yu0fHEdEyHW0jvi2/CctvC/NbWr5Dn+Q3+x0m+v1mQjstdVxnFdzuXa+XFnU9ul7C4+MhyzCxZE7w+4XHuMG2M7ouo21EtE3qtO+bhjYiOsaNzi9aZ0PL2WIfpdP1ohb7+kOWfVJtRKdlrEVcOK/QcR6j6/XZ5Ri+zfy63u+Ozm/YtOrUvei+Rmh+miHj+GB5ie4rhuLGWVYeIU3jaeGTfsjvdPpjSS8rvHZTzdiHJN008Ph7/ntjScws+U8ZzlC+OHrZZ0vmd66kcwqPP+e/Z5fEzJdfB3k9SWtJWlvSrfn5WhXzul/SH/Lj/vx4cOr1irjQ95MX8P+WdKzyNYZqxnW9nO+VNyIbNikvLeIab/No2cxxl+Tyso2krfPfO/LzrSewHT4nP3q5csP1Et1+0fUSqetdl5VoHVpT0gmSPilpqQZx0W0eXc5oXKiNb1FW2tT1aNls2i+Etnn+XLRPibZl0bre2XZvMa9omY6WsefIbxLz/6SHf3VXJy76/XrfTrdcn9H5Rbd71+ulTV2PzC9aXqJ9UTQu0kaEtnlhfk3b+Oi6jLYRoTo0hnLddL103UZEx7jR+UXrbHQ5o/161+sl2od12UZ0XcaicaEyFi0vLcp01+uzs3as5fy63u+Ozq9N3Yusz673absex0fapGh+IBoXKit1Hq0n0PeHpLmSPivp+LwB6g4w2wzeVs/z+19Jv6oZE+2MXyXpJ8rX1OmiQEW+X47bLDc475V0cx+XsxBzSG7E6paXxnEttnm0key0syps87Ml7ZfnX2t9RrZfi/USjeusrAysz9p1qBC3k6Sf5zLXRRsRXc7GcQq08dFtHt1+LcpYmwOyjbZ5IS7Sp4SXc2CdNmmrO9vukXkVYiNlOtq2zJK0f57fFg3i2ny/XrfT0fXZZn6R7T5N6yVS19uul6blpetkTpv1Ganrbdr4SLsZbSOibVJnfV/XbURhmzce47aYX+M6G13OlmWz6/USGQ90nXTvuoxF46JlrLM8Rtfrs8U273Q/v812H1inTfqUyPqM1r3o+ux8n7ZF+WzcR7csL9F9xcZxbcpm5XTHMZGZ8JC0SS4Yv20QE0465fiXq8GF4hVPvC+dl3G+pNu6KlBNv1+OMUlvk/T1ni/nK+U/W7tzknEttnmbhGgnnVUhdlaO+6mk2ye5/Vp0Hm3WZydlpRDXqA4V4paS9F+SfjLpbd5yOaNxjdr4MbTvTet6Zztp0W1eiIv0KeHlLEwj0lZPbfe7Jr3d5de7qz2vQly0TEfbiNXkP1dsWqYbrcvotpuOdjqyPscwv6bjnenovyJ1vdV6CZSXrpM5bdZn47retu0MtpvRNqJxm9SiXEcSlJ22ETkmPMYNzq9xnY0uZ5uy2fV6yXFNx4HT0UZ0VsZaxEXLWGd5jK7XZ5ft2BjKWGf73S3WZ7TuRdfndO3TdjKOb1leovuKjePals2h0xzHRGbKIxfEJwbiQgUxxza+w6cCifcct7Gktzb4fKMCJWnZlut/ZUmbyhMCKzeIa13wg9thSUnP6iJO8SRJm7I58c5qIH5VFY6mTnL7teg8onGdlZUuH5FtLmlO4flc+XXXlq8ZG2ojCvGN2/iWdShS19vupEUSjZsGt3+jPmVgOevuTK451bfIf2K6S2CdmqRlOtoOoXFEjh15V/JxlLE2j6bfT9KKub5uKGluR9ug13W2TRs4jeslUtfD8wssX6fJnKbfr+02z3G12/hxtJsttkV0vNNZ39d1G5HjQmPcFvNrXGejy6ngPso0rZemfdh0JN27LmPRuGgZC41XW8yvs/XZZTvWZn5ttvvANGqP65rOr2Xdi/QL0XFE233TzsbxLcvLk7pYxkhZqXpMXY/lUcvMXio/WnFWSunmwuv/klI6qsF0lpS0TkrpyorPDN7hU5I+pNgdPqd2zv9Q8ZnHSfp7yhvRzLaVV7arU0qnNpjXqpKenVI6ZcTnHpBfCP84Sd9JKd1bc/qbSPqipHmSfp1fXl3SvfIkZa0L9jdYzrFsBzN7gfwnHlemlE6v+Nzykt4u6XZJR8rv6vp8SQvlyeLf15zfyG1eEjeybObPLVt3m42YTq3tUBL71ZTSG0d8Zlzbr9Z6icSZ2XMlLUwp/SF//gDluiff5veVxO0n6bsppVsbLtPv5Dd+OE5+XbBaDbeZrSc/gv2QvAP/V/lPg66XtEdKaWHN6dSte3vKbxhyj/xnUp+XX7NrXUnvTykdVxIXbiPG0cY3KStmto78Z5FrSHpAvi6PK9vmo+ZnZm9KKR1dM65OvzB4gxTJz3apfYMUM1sipfT3gdeelFK6e1zLmT93gKS3yG/c9Gn5T+V+LmlLSUeW1XUze5WkH6eUfmdmK+bYqfr3npTSbTWXs27bua2k12jxbX5ESumGipjBu5JL0mEacVfyFm3EPHnfs7M8wSz5TWROlnRwk7a/5o141pd0qDyRtqakS/N8fyJp/7r1YZLtdP6cSXqt/MYzJ8hvBraTpGskfTGl9NCY57enAm1gdH5t48ZQ1+uulw0lfVl+ttGpkj4wNTYyswtSSlvUnF9o/NEirs54YE+NYZvnaZk8eXB/xWei7eZsSXvJ+8sfppR+XnjvwJTSRyvm2brfy9OJluvG4+Ou24iBab44pXRGIK50PGBmG6WUBm+Y10qT5WyyDcxsrqTttXh5OX3UuhxXOStM799SSh+p+dmJtRFDYmrtX+bPRtflevJyvJq8bN8uaX6dcb+ZbV6cX0rpmpFf6pHTqNOWhct0/n6rSTo/pfTHwuvbp5R+WBKzo3zd/SUyz8J02rRjleukzfxyXmhXeaL2TDPbXYvyEYcP9vU15/2rlNKaFe+Hy1lhGtG6F82b1N2nHUv+Kk/r7JRS5c1ozWyWpD3l+xura1F9/2JK6UcN5lVn3LKDfJ/k15LeIb92/eMlPUGeHzir7vwK0zw1pbRDxfuhtmzkfB/NyWwz+7ikF8hvfPdKSf+dUvpcfu+SlNKwnf6p2MY7lPmOnIN3+Hyn/OLxSin9R/B7DO2MzexySduklH5vZu+TDwBOkd/Q76KU0gcrptm4QJnZAvnO8m459mfy5NrJKaU/V8RdJuktKaXzB17fUtKXUkobV8Q2biSj26G4Q2Vme8t/TvJdSS+R9L2U0sElcadIWiDpiZKemZ9/W9KLJW2cUtqpYlkbJ0lyXOMBn8UPRoQ6RzObP/iSpG3lP/NRSmnHkrjo9gslmEumVdnpmNlV8m37gJkdLulP8p2gF+XXhyWyZGb3Sfo/Sb+Ub4fjU0p31Viea+XX/NpNnjw6Qb69zxsR9xP5T4DmSjpY0gckfUvSKyS9M6X0opK4NeVn1v4lDxb21KJ1+eWU0gMlcQvk23gZSZfLBwu/NLOVJZ2RSu5MHm0jWrbxkTq0X57PjyW9TNJlkn6fp7Nvk8FGYZqlA8XBpJKZ/bPyDpB8OzyiAzezh+RH5f9aeHnL/FoaUa63lfQ1+YDmUkn7pHyAYNT6rJhm6c5krkeby3+qdrOkp6aU7jKzpeU7KM8qibs6pbR+fv6t/N2Ol7SdpNenlF5cEtf4wKOZHSw/K+MseaL4JknXyZPSH08pHV8yrwf0yLuS7yKvuyml9C8lcdE24jR52/qVlNKd+bVVJO0habuKdTL0DuPyNi2lkjuMm9l58gHvtWa2haS3pZT2yH3nS1NKu4xa5jydJjv1kTp7mKSVJD1OfvOfx0v6nrz+/ialtH9FbGRnOdQGlkxr5M7PiPiqxFi4rge3w88kfVReV/eS9Cb5LxV+aWaXppSeXREb2lkex072wPSGrs8229wCB+ZatJtH5JgLJL0hz/fd+b3Sbd623wuWl8Z9X8l06iQQwm1ExTQrE0CRODN7UN7/HCdff1c3nX6T+eX3IwdyXyfpffK6sK38hm2z5L/eeX1KaUFJXNfjq7EkNvO0Ru0zRPcvo+vyA/L9hW9KmmpDVpfvy32zYn5byw/M3Su/LMPPJS0nv5ncG6pyIsG2LFSmc1l5m3zston8APrJ+b2qtuzP8vHVqXmep6WUHqwxv9ABr8g6qbEsVf36NyTNkbfz98r3/U6U75taSmmPkrhhJ5FJPib8cEpp+ZK4UDkrmVadk91C/UKLfdrovungARqT9HT5voMq9oWPlnSLpDPl+wt/kJ9F/gF5ru1zJXGN8x/5u+0maVlJ35f08pTSeWb2TEnfqKhDZWNDk/T9lNKqJXGhtqyW1NHp5NPxkCcV5+Tny8oTZJ/N/186IvY++cD3p/Kd1hVrzC90h88a0x16XWP5zt/U84skLZmfz5F0RcX0XifpQklHyHeYvybpG5KuUOHi8UPiLik8XzJP50T52SjHVsRdX/HeDRXvfUA+mDlA0j/nxwFTr417OxTLRF4/K+bnS0taUBF3Wf5rkn497L2SuIMlHZ2/1wnypOPe8h3L11bE7Se/ieOB8sbgMEkfkzda24yoD6/I2/oe+Rl7u06Vm4q4b8gToN/LZeW78h2hY+SJk9LyIj/St438AMs2ku7Iz7eewPa7Sovq++Hy5PcLJB0k6cSKuCsGHgsk/WXq/5KYhcPqRY1tfqm88X6JPJl2lzzhtYcqLpOgxevempLen9fvjaq4VMxAmb6hbJpD4q4srPtP5u3xz5KOknTUqLqQn98+8F5VmxRtI0JtfMs6NDs/X0rSjwrbpGp+g2WsWNb+WnO7HyjptFxWjp/6nkNi2ty06UJJGxSmc72kLUetzxHTLL0u/1SZkDRbnvSdVSyDFXHXFp5fXFYGh8SdksvzF+QH9j4n6R8kfUQ+UBy6zQvP50j6eX6+3IhljN6VPNpGXBt8L3ojnssryurVFXEXFJ7vLe/PD5LvNFf16+E6m/8uIe/3HlfYllX9+n6SrpV0kjxhuNOw7zokLtoGNu6HamyjqroXqusttsNlA/9vOzXPEeszOg4MxUXWZ3SbD9YV+TjrXfJkwJ7yRPjQspL/Nm03ryg8nyMfJ52ofECjIi7U77UsL5G+L1SHFG8j5pc8vifp/6q2Q8lj1HjgUknPyuvvBnlS4ABJa4/YBtHljO6jXKFF48cnyROGkrSRpHPHXc7kCZ9hj/slPVAR92dJd8v3a142Ne9Rj0g5U3z/Mrour5O0xJDXH6fq8falhWV7ivykPslPzjp9xHqJtGXRMr1A+fIX8hN8LpIntBdb1yXzWy6X47Mk/UZ+5u3WI+Z3WK4D8+X7tcdLeqM8ifs/41wnNcpfnTH1nPzdpuqTlZXN/P5fJP2nfCw2+Lh3AuVsWFv0x6n/K+Ia9wv5s9F92ui+6VQ5WU/SWrmM3pqfrzVq+xX+Py//fbwKeYchcY3zHwPr8taB96r2ox6UnzhzzpDHn6u+mwJtWa060Sa474/BDS8f+B2ZC/1VI2JDO5Q5NnKHz8adsXxg+Kz8/IeSlsvPn6ARA9pIgVJJByH/+cUeFXGHSvqBpH+SnwX3/Pz8B5L+tyIu1EhGt4O8E11O0gryM9tHfvfC+lxOPuC6T7kTztOp2qmPJkmiA77owYho5zhL3nGfIWmT/NrE7pSreIK5cacjb0PelJ8fLWnz/HxdSRfW2Qb5/yUk7Sg/Q6D0ul8Vde8Zkg4ate3y830H3qsqY8UB2MVafGf58oq4+ZI+Ib+56NnyMzy2kneop1XERduIUBvfog4tkPT4/Hw5FRKpI9bnb+Rnj6w18FhbFddt0+I7QJdIWrpQbqp2gKI3SBlMUG4gT+i9arDsDnwuujN5jKRj5QfWjpPvVL4+b8NvV8R9SZ6AXjKXsZ3z69vKz4Ipi2t84FHeLyxfKB/nFd4bNY6I3JU82kacLj/IVUxKryxP6p05Yp6Ru9GfKL9s0fPlZxsdVVje62qW6SY79dE6W5zfD+ts88L8IjvL0TYwvPNT8hiVGIvW9eh2uFzSvIHXNpIntO+piIvuLEfjGq/P6DbPsY0PzCnebl4z5LWD5OOsqnUS6vdalpfGfV+LOhRtI34vv/fM1gOPbeRndJfFRccDg33DFvKbfd2q6n236HK22UeZOoC75MD6HRUXGV/9SiXXsdVAkmZwuyuW2IzsM0T3L6Pr8pphy5KXsergdnGfYbYW328cNd6JtGXRMn31wP9z5XmQQ8rmVTK/VeTjnl+MKCvRA17REy+i/fqV8j5uOfn4e2rs+gRVJ0PPlbRZyXtV6yVazqInu0X3iaL7tKF90xz7Kvll93bM/9cZV18svzyI5GdW/2TYdxgS1zj/IR+rvEV+tvQV8nzNavI8589GlLGnB8pKqC2r8wgHzoSH/LT5rYe8/lFJD42IDe1QFj7f6A6fCnTG8h2By+VnVX1Vfpb1UfKdrt3HXaAkvbfFtniZfJDwvbxdvqgRF35XsJEc+OzSdbeD/OyrG+U/ebpR0ir59blljUF+fzf5IOg38p/jnSlP4P5a/tPdsrhQkkTxAV/0YESocyzET91h9/OqOKJcElu7HimYYM6fadTp5HV2TK5z58t/gnej/IzYjZtug/xe6Rnykg5pst4KcW/RkJt3SHqa/JIcZXGnSXphfv6dqXooH4hXdfxPlF+64YBcb3bJ9f0wSauOWNYd1LyNCLXxLerQ/vJO/3B5+zRV3lasKqPyJMMLSt6rOpB0jfyGI5sNrndVtEmFzzS6QYq871hl4LXV5Wcz3l8RF92ZnCNvP3fNz58vTwi9X3mQWhK3hKR/z/P9lfya8PfLEzxrVsQ1PvAoH7jeIk8W/0r+U7ypbV667QamUfuu5Iq3EcvJzzi5Rp68+J38J7ifVI0b0SlwQ2hJn8p18GPKB/nlbeOWFXFtduojdfZUDW8DV1HhLPEh70d3lgfbwNeofhsY2fmJJsaidT26HXYfVi5yXfxyRVx0Zzka13h9DtnmTfq9xgfmFG83vy5p+yGv7yW//05ZXKjfa1leQn1fsA5F24hTJW1b8t4kxgNlY3hTdQIoupzRfZRPyseQH5L3Jx/Kry8/Ii46vvqopC3KlqUiLpTYjJQzxfcvo+tye/mZzqfm9Xm4vP+6QUPagELcUbl87i4/k/iQ/PpSGnIwbCA20pZFy/TZyidJFV6bI8+FPFgRVzXGWKtOnJod8IqeeBHt19+Vy9ctuSyfJb9XxQJVn/j0DJVcgUAVNzxsUc5CJ7sp3i+E9mnzZxrvmxZil5aPGedLuq3G518o38+4Tt5WPDe/vqKkT1XENc5/yC8d9SX5L1VXydvjSnmi/pkV89pF0jNK3tu5Ii7UltVaz22C+/7IjcfQnT9Jq42IDe1QtljWaGc8O1e0/SW9R77jveyIeU2sQI15nYQayQksx1KSnjLiM7O16Ccec+TXMxy1ExNKkig+4AsdjFCwcxwynZer4pIYY9hOoQRzIb5Rp5NjlpHffXsz1bjDsaR1uyq3LdflGvIk6E/kHfjv5YPHSyW9aLqXr7CcoTY+WofyZzaQd+brdfD9zhl4rJpff0QisGIaJumJNT+73bC6Ik9cfrgiLtR/jWkdzZO0Qs3PDjvweKZGH3hcPrfplX3rmL7PWNoI+eVT3iPpJTU+u4Wk5xTi/k1jusv4kHndrNhOfbjOlkxvaUkrVbwf2lkew/ppuvMTTYyV1fV5I+r6WLdDje8X3VmOxoXWZ4vvFzow12J+xbq+vqR316nrCvZ70fIivwxUqO9rWodGTKe0jej6oYqTlCY0v/CBXPkJTO+V9OLCa7OUD2yMu5wFv18osTlQPlqVM9Xbv4yuy1nyyzi9Jq/TLTXiUiq5PdpXfnBsby36VcWSo9ZJpC2Llmn5gddVSt7bqiJum+D8oge8oidehPshSU+W9OT8fNm87YeOz8fxiJSzge14fC5vI092U3CfSNO8TyvPE7y15mefp4Z9tFrmPwLfZz35ddjnDrxemZuLtmWjHo/qG0AOMr/p4bryoz+VN78zs3VTStc1nP7DNwUys2XlP72dujD9u1JKv4kt+fiZ2cvkleTylO9kbX4X1SVSSn8tiXm7/IL+d5vZ0+RHcDeS/zR1r1R+I4rnyM/g+rX87JWj5NcTvV6eQLi0YjlnydfhavKkzG3yo0ylN2zI2/n9WnQ32L/JK/gXU0rHVMQtO6pc1NGwnC0v6anyay/VnreZbSC/2eSVKXCX6abM7MmSlFK6PZft7eQdzwUj4kyLtl+SX4f+ghRseGzEnXLzZ5aRr9M58gFmo3pnZhtLel5K6YsjPrempD+klO41s7Xlya5rUsO7W0eZ2XUppXVHfGaOpDfLzyJ5shZtg5MlHZlG3Nk63whiXeV1Ka97VTeJ3Vx+Jn3jul4xzcNTSvsE4tarqhvROjTuMh1hZrPlnf+fan5+ZFmpiN00Nbhjd8NpT53RuLqkU1NKxxbeOyyltG9J3EYppSuC85wt/2XSA7l+bCK/5MgdNeNrte8l/eWG8jMuSvvLHNu4bRm4wdRe9T8wtAAAIABJREFU8psjnaTRN5g6SH5AfI78LJkt5APg7eSXSPhYSdzD28DMlpBfzmRqvPPRumWzML2l5AcEb6r4TOM6a34D479P1c98Q7NN5Wden1oRt7r8Ejl3Dnlvq5TSz0viVpEfDEj57zskvVqeyNu/QTmr1Q9Nh+B2CJeXyDiwTVxTber6wHTmyU+KuGfE56Lt5mBdf648aVxZ1wvxK+Z5PiC/rv4fqz5fiBvbeLVJ39e0DuXxy8M3OqyzrGY2J+Wbh+W+YT153/C7OvMsTGf5pjFNmd+Q9OFxS52xcXQfZdh0It/PzPZNKR3WYr6l40Az2yYFbio5ZDq1y1m0Dg1MY8eU0vwan5u2sWrdtqzlPELfb1x1NscvLf81zG9rfLaLdRLKY5jZifJLx53UtEyOo5yZ2SskPT+l9KEm8y7E1+oXAvu08+R97U7ymwRLfp+KkyUdHFzXVW1SaDxeiG+b/6iTVwjdfLUQ37gfGimSAZ8pD0mHFZ6/QH5U7Bz5tZjqnIlg8sHeq+XJoOcqX56j5PPFa0sdIT9bbS35ma0n1VzmYdf4e1LZ/OQXwF9nDOtqxxqfuarw/AeSXpWfb6N8LbWSuAvklXO3vO53ya+/SNIvGi5nnZ9Lnyy/ucLq8iNa/yq/i+xXVH2zvAfkZ+m9WQ3OwIuWM0kbtdhejcpmjpknv6HLNfJrft0jb4wOHvV9g/N7iRadGXVEfkydGVV6tqA80TDssZmkO9qW9XFsB/nPiW/K63Kv/PdI+U0Y3l0Rt6Gk83LZOFz5OvdT9aQi7n4tfh3i++U3YbhfnvQqiztO/hOiLXN9WD0//4Kkb434jnMKz+fKE2qV9S9a1+Vnvg57rKD4GS9NL2mzb43PhMr0GMpok34hVFZy7LA6d5v8Z32bBpe99Awr+c/9Dpa0s/zspu9o0U/Sq67b+2Be5/8paf0Gy/I4Fdot+U893yNph4qYaPse7S+jbUura1HLzxD7g/JZ/PIzsaruiVAc73xGflbI1vJrtX91xHZo3J/kuDWV+yr5z213Ub5vSEXM5Vp0P5H3ya8NeaB8R+ETI2JnKV9bMZedTTW6DfyhPIF9gPyM1A/k5X6HSm4yOhBfu65XTKPOOCk0flTw1wltysvAdJ4mP1FhZL2PlrPAdwvV9RrTHdp2Kt5uRuv6+vKx8Q3yk0POl7dRx2jgOugl8ZF6GxmXNW7f8+e2ll9250z5GXvfl19H/EeS1qiI21M+jr5OPu65Uf7LxVsl7VYRd+DAup36SfnNyj8rL4mL1tlny8edC7Xo10jX5Ncm0a9vled1Va5zZ+R1c6s86VsW9+6Bx3vkN2h8tyr6vhHLWedsz5XlbfuzVeMXloW4zeXtyiur1kdhOzeuQ/K2q/h4jaQ7p/6viIvuf02VsadG1nfT9TJiOqdO4PuF6myLutBmPz8y/ojmMX4tvyni7+SXxHuV8nXBR8SNbZ9o1HcbdxlTvbzXafIx3CqF11aRj+8mcQPPUB8dKS9atK94v5rlFaL3k9lEY+6HHp52m+C+P7T44PmcqZUlP2ox6mdqjSvowPwG79xeeX1T+aDrNvmNJk9X4U6+KhmcyjvCT8t3ri+QJ82fXGO9RDvH4o0MLhx4r2ogXNzJ/lXZe0PiogO+wesoXZj/zlLFNb9yBX2FpG/IO7uT5dckrLysTLScKZ6QiXbiZY3yB1TRKLeY38JiOS68/hRV34gieqfcjRRLFDfeDvJB+pLyZOv9WjxxVHUdyJ/Jf/68rPynNldp0c0equrC5+Q/by/e3O2mGstZdW3Qqpu07anYTlq0rj+oRZcemHpM/f+3irhDSx6fU3VnHNppipbp6EOxfiFUVvLnHpIn+xarc/nv2cHvUDVwG+wnPyxPIqxQ9v2mypKkZ8mv1XyDPGF5wLBtMxDXOLGpePse7S+jbUv0WtSXln1ucPtUxF2mnITV6BsDR/uTaJL/ysLzi5T7c/mZK1XLubP8cjR3yM/KOV/eL90m6ZU118tgG1i1PhvX9fxedJwUHT9Gd5aj5eUc5WS+pDfk73eEfLz2jgmUs8bjCAXreo11NrTtHCxHatBuDnteo2yep3yNTPmZYl/Jz/eWdMKI7xCtt5FxWejAlbw/mWpnnyLpu/n5iyWdXhG3QNKTcswftGgst/KIMl3sU36gnGzP67bqpnfROnuZhrQF8hMbKq8X27Rs5vcukJ+48Tz5uOoF+fVNVX0g9375dZr/TX5j0oPkBxcOUvX1fqPjwFByRYGDH9E6JG9vvy+/Du7U4/7896iKuOj+V6iMtVgvoZOXWny/UJ1tURei+/nR8Uc0j3Fp/ruMvJ89RT4WOVqT2c8fNm65UaPHLY3LWI4bzHu9Wg3zXg3fi7ZJ0T66cXlRPK8QvZ/M2Puhh6fRJrjvDy0+YBi8i2zpzl1+v3EFzYVmKjFyoxY/Q2DUEZULJW2Qn+8i/1n+llXLOvD9/kF+s5k75YP/qut/RjvHj8mPIj9Vfr3td8rPuHiTpO9XxP1CvmPxWvn116ZugLC1qpMB0QHfuVo0eHqlCneTH9H4FOe3pKTXyX92c4+qrz0ZKmeKJ2SinUe0UY7O73oVzu4tvP44+U8Wy+Kid8qNJoobbwfl+iw/gvpbLX5n5KqE0+BO6LZ5PW2pip3Q/NnN5J3TfvIDM3VulnFernfF5Zslvxbi+RVx0Z20aF2/XuXX1Kva5vdL2kd+9+XBx90j4iI7TaEyHX0o0C9Ey0phHj9W4Yxj1RvcRAduC4tlM7+2R667t1TEDd64aQv5QOpWVfcNjRObirfv0f4y2rbcrNi1qM+XtFR+XpzXvMH1PBB3oxYdDF848F7VTWKj/Uk0yX+u8lmg8gH3VLLrCSPiLpUf7J1qA6cSEWupui27vPD8o8O2bUlctK5Hx0nR8WN0ZzlaXop19kLl6+PLz1yqWp/RctZ4HKFgXc+xjdtOxdvNaF0fPEGkWHaG3ji38H603kbGZdEDV1cUns8e+H5VN9m7rPD89rJpDokrTn8wYVG3rjeps9dXvFc1Fh9HQmawrleVszXlZ4d+slBO64xzo+PAUHJFgYMf0Tokv0zfWZL+n/TwpWFvqrFOovtfoTLWYr1ET16Kfr9onQ3XBcX286Pjj9Z5jMJry0t6qypOZBlTOWsybokeeJzKex2lZnmv0+WXrS0mfFeWnwR4ZkVctE2K9tHR8hLJK0Rvvhrqh+o8woEz4SHpT/KfeS7IBWtqJ2aWKgZRUyu9aQXVoqTI1GOqwq2i0T+7HezoNpBfi/pVZQW4pPGZLR+IH10xr1DnmD/3plzZ7s7r9GpJH1f1z6Q2kZ8VfKr82lT/I08cXaXqGzVEB3wby48o3yvfMVk3v76ipP0q4sp2VOZJ2mPc5Wxw+6l+QibaeUQb5ej8PihvYD8gvzP27vn5pZI+WBEXvVNuKFEc2Q7yHddj5Tvyx0n6mqTXy884+nbFvC4frCvyM8Gul3RPWVzhs7Pknc5PVXFH68Ln15YnbX8rP/J9XX7+LVXcdEbxAd/GemRdv1de159fEfc2ldykQtVn351dNl1VtGmK7zSFynT0oUC/EC0rhbi58p/+H5/X0yR3Jj8labshr2+v6oFPWVttkrauiGuc2FS7ccSeat5fHqNA21IxvcobTKnkxivyg1kbVsQdrcV3DFbOr68i6ayKuGh/Ek3ybyRvd7+aH7/My32RKm4+pcUTMlcOvFfVn3xEw28U9TRVn4EXqusaQ2Ks8Fqd8WN0ZzlaXi5VvpmvPMHxhMKyViUaWyc78v91xxF7qmFdz3GN207F281oXT9Rfrm+58vP2jwqv76EKn7hlT8TrbeRcVn0wNVR8vZ1d/nY6JD8+lKq/jXnfEmfkN+87Gz55XO2ku//nVYRd2+O/Z787MelIuuksF5H1dlD5Qmjf8rb8Pn5+Q8k/e84y2aOKx7Q23ngvco+M39mJ/nZlruofnIlMg6MJvkbH/xoWYdmyW+kek6uBxMbq0bLWIv1Ej15Kfr9onU2Whei+/nR8Uc0jxG6eXPJdjigSTkbXOay7xAtY/m96EGh5eT7idfI81a/kx9M/qSqL+ERbZOifXSovOT3m+YVojdfDfVDdR6P6htAmtlaAy/dkVL6m5k9SdI/ppROrIj9oHyQ/k15oyP5jUF2le9QfqIkbj35hc3PT4WL6BdvDlkSd5GkV6TCzYbyDYi+Lz8rZJkhMd9MKe1aNs0q+cY475D/NOED8pvXPDUwna+llN7QMOYf5A36gpTS6RWfu1d+51mT70islfLF/c3sypTSs2rO7wV5fleOmN97U0qfrv9NHo4LlTMzuzSl9Owhr1uO+3FJXLRsLifvZIo3MviNvHM/OKX0+3HOL8euL2lHLX4DpvkppavLYoZMo+72u1y+3u4rvLaR/HqSy6eUViiJa7wd8o3jXiu/gcEJefl2l/807/Mppf8rmdfu8oHoeQOvrynpX1NKe1d8vy0kpZTShbkObSs/4npKRczj5Nevvl1+Lbwd5B3IVZIOTyU3gDSz+fkzy8h/AnapfDC+nbyDfmnFPJ8pv9lk0zaw+P3Wlw+erxnx/ZaX9JfU8GZzhfid5Ad4PivpU3XawPz9dlKLMt1g+Rr3C0Omsaq87gwt/xVxm8jXy7NSSiuO+OzZ8p8NnjvkvZtSSk+pOc+6dX33VLjpWV25PfiaPLkp+U7Mj+UJz0OGTbNF+/44eRt5e0rpTDN7vbzuXa3quhdqW7pmZo+Xf79f5++3u/z7LVT194v2X8fIE5FLyw8wPCBPWL1Q0jIppddVLOts+S9Gijf+OS1V38DzUkmbpZQeMrMtUr7ZcZ7W5WXjj3xznO+mlG4d9n7F/EJ1PTpOio4fK/rLefLE1VdK4qLlZRtJn1fux+U/Qf+h/KzB08rGbC3KWXQcUey/NpD3Xwur+q8c17jtNLPnyvvG+8xsSXlC4dnKCfTiso+D+U2/P6R803j5ePH+vM2fOTieGYg9RoF6GxyXNW7fc9wS8ss9TH2/o1JKD+Z1u1JK6ZaSuCfKD8QneXLspfITfm6R/ypj6M1ezWzrgZcuTin9Md8Ya5eU0udL4trs8+2g4eOWqvFVqF83sx3lJ8j8aeD1dSS9JqX0qRrLu5Sk/5CfOf2PIz4bGgea2aGS1pEf5Cy2EW+UJ5zeXhJ3lHybnyVfp79OKb07L/MlKaX1hsSE61BhGqvJx2SbT2qs2rKMRdbLLvJcwLVD3ts5pXRSxfwi3y9aZ6N1IbqfHx1/hPIYObbxPliOi2yH6LilcRkrxDbOe7UYz7XaN20qUl6G7KO8Qd7mflrSl8vGZC2Xs3E/VGu66VGczB7GzFZINe8k27SCmtk7JL1dgTt8mtl2ku5KKV0+8Po8SW9PI+5gmj9bKxEwEFO7c8wJrkEvlB+BUkppx5K4C1JKW+Tne0vaV9JJ8p3L76WUDi6Jiw74ivPbS75Nvjtqfl2LJmRy7FgTamb2ppTS0V3Nb8SyDJaXt6nG9rNgorjNdhgHM1spjbgTtgXvcGxm38gxS0q6T75D+V35DRktpbRHSVx0wLefvH5fowZt4JDv91z5NdBq3cG5jSY7TV2L9AvRdrpk/iZPOPxhxOeiO5Ohut5GJLEZnM9U3VtKfiZerbo3Uwz5fnPlB7xeJEkppT0rYiM7P50m+c3sOfKd7L8MvL62/DJmXy+Ju0/S/8nPAD9O0vEppbtqzC80BhwyTrokJ0kqx0k5dh35md9ryJOM10s6rioZGt1Zblle5sm3dbHOnpxSumbEPBsfTI+MI6L9c45t3Haa2VXyXzI9YGaHy5PEJ8jX5cYppVfXndakRettdFzWVfteMf+R47kxzqvxPl8hts64s9OEzHQIJvlDBz+GTKezshLVpIy1OCgUOgmwSy3GuNF2LDT+iBrnPlidPFuL/E7rumdmT5b036qX9yqO546Vj+fuHjWPrkXKy6NqHyW1OK277w/53b6nbhyzufyafTfIEzJbT2B+oTt8tpjfBYXne8uv/3WQ/OdZB0xgfpdI+rr8Du1b57935Oel61OL//zhQi1+zbwFDZdhpRqfCc1P/nPXL8jPAlpB0r/nbfptSatWxG1feL6s/OeKV8gbvtp3xp7Oh2rc8TswzSfKf871NQ3cNFDSYV2Ulwmur+hd5ZcfeKwgv9btcqr+yVLoDsda9BPfOfKz8Gfn/ytvulUyrTp1L3qX4+j3K9a9eZOue4XtHr7Te0dls3E7nWOXkp+p/j75T7P3kP9y41MacumEMSxrtK0O1b/gMs6VXzriKvkBobvk16Lfc0RcqO5phvQn42xbpvE7nDqBaV4q/9nmS/K2u0t+Juoe8gND0/6983LuJ99pPVB+eYbD5Nf1vFrSNg2nVadvmPHlpeK7hfqvFvNbWHg++DP2ypvNB+e3ufwSB1+XH/g4I7eFF0p69nSv/zF8v9A4Qo8czy2veuO5jQrPl8h1cL78sjRLVcSF9vmiy1kyrRVqfGa2pLfIb3q31cB7B1bERcfVYxsP1GnLgtONjv1D63LEspT2e9Ey1mK97Ce/nNZJeX3sVNyuFXGDdfaIOnV2xLIcPolt35dH1fdTfB+smGfbTJ5nu16BPNuk6l7F/EaWEwXHc1o8/7H7wHul+Y+Ov3+nYzIF+706j1l6dHt5WnQE5b8k/VNK6WnyC8V/JjpRMzu15K3ZKR9VTCndLE8i7GBmh8gLx7jnt0Th+T6SXpxS+g95pXt9xfQ2N7NzzOzrZraGmZ1hZvea2YVm9oifwxRsLuli+Z3T70sp/Uh+g4Yfp5KfymSzzGw5M1tBfrTnLklKfkbGAxXLufzgQ9IFeVrLj3t+8muVXi3/udk5kv4s6eXy6wh9sSLu44Xnn5Ynjl4pH+h/qSKuVMU2D8eZ2RUljwXya2ePezmPlpf770jazcy+Y/5TY8l/VlQmWl7mmdnBZnaNmd2THwvza8s2+2YPT7Ps+y0nTzSdY2YXmNm78tHeUe6W16Gpx0XyMxIuyc/LPJBSejD5WQG/TPlM2ZTSnyU9VBE3y/ynRMvIBynz8uuP1+Ltx2Ja1L1oGxj9fsW69xlNvu5NbfcfNdzuY1exnNF2WvI2cGVJT5Ffx+w58jbN5Af6xrmcUrytjta/yHJ+Qz5Af6n8DP5D5Xd739bMPl4SIwXrnibQn0xI9PuVGtF/PdHMPmFmX8tnzxbfO6wibtOSx2byX4+MdTnlP9N9KKV0ekrpzfJLLh0m/8nujeOeX4t+b295QuCj8rOv1k8pfTgv52cr5jfYN6yg+uOySF8U+n4D5WW3gfeqysuw8fF9eXxcVl6i/Ve0XF9pZm/Kzy83s83z59eVNPafBsvL76fkfcK5kr6UUponv2xd6brMy3SJmR1o/iuA2sxs+8LzeWZ2ZB6vHmt+9t5YYrLoOGJwPHex6o3njik8P1h+Pf3PyBNHVfsaoX2+6HLmOvak/HxzM7tR0vlmdos98szKoi/JD57fI+nQPP6bUvWrgWi/HoqLjnPNbK6ZfcTMrsxtw11mdp6Z7Vkxu+jYP7QuW/R70TIWbcv2ll8eYWf5/sK/mtn+U2EVsxuss3eqRp0dts0L/djLxvzdwnFVRowHQt9P8T6smGf7tDzP9nSNyLO1qHvR7TBsfuePmp/i47li/mNXq5//GLuK8jL2MfwIxxSeN+n3RprTJngGWMLM5qSUHpDf1fpCSUopXVcoVEOZWdklQUzlHcGdZrZJSumyPJ8/mtkr5DcX2XAC85tlfh3kWRpIBJhZVSLgMPmR1mXlA9N3pZRebGYvyu89b1hQSukhSZ81s+Pz39+oXhmaJ++8TVIys1VSSnea2VxVd1Z3y4/uFU11/kl+5/hxzm/llNLnJMnM9k0pfTK//jkze3NFXNHmKaWp7fVZMyv9mUZwm4fj5Emql8pvYjAY94jrgI1hfuuklF6Tn59kZh+WdLb59fSqRLfft+WXUtgm5euOmtkq8iOox8s710d+idj3+31K6b2S3mt+/erdJF1iZgvlP9M+vCTu/fLEwftSSgvy/G9Ko68p/DczWyoPNDYrLPs8VQ80jpRf8mO2PLl5fN4h2VJ+LdEy0boXbQOj369o4nVP8e0eElnOFu205DfLfZ2ZmXyHfruUUjKzn2rRdUjHspxZtK6HtkNwOddOKR2Tnx9iZhemlP7TPJl0tfw6mMNE615R7TI9DULfr0VZOVp+xs93JP2Lmb1GfsbLX1W9c3Ch/JIPw8pTVTI0upyLzSf5dQfnS5pv/lPYcc8v1O9lcyQ9KN95WSYv76/Mf8pbJto3ROtD2ffbU9Xfb7C87KJ65aVqfPwFDR8ft+m/IuV6L0n/Y2YHyrfHL8zsVvmJGHuNmF/EEimlUyXJzD6ZUjpBklJKZ5nZqEvOFBONd8ovvfOtlNLtI+I+Lj8DTlo8wfxqebJq5zHFDGrS5kbHc8U24kWSnpNS+ruZ/UQV/azi+3zR5Xx5SumA/HzqhLALzQ+aHCs/cD7MFimljfJ8/lfSYWZ2oryfHnu/3iIu2pZ9Q/5z/O3l1+VfWt6GHWhm66aUho0Jotsgui5D/Z7iZUyKtWWLnQBjfo+EE8zvVVL3JMAmdfYu+TYvTjvl/1caGuGi449QXIvxQPT7RfuwaJ4tWvei2yE6v9B4TvH8R0iwvIxjH6WJaL83WurBqe6Tesgv9H66/Hqh/y6/Rs4/ys+u+tqI2AflA+hzhjz+XBITusNni/ndLD8ydFP+u0p+fa4qfmqoxX/a/auy92qs35fLbzYT3T5LSXpKxfvvlQ9MNyy8dtME51e8A/dHB96r+sn7bZLeLek9eTtY4b2qn+c03uYt446UXztp2HvHTmB+C1W4c31+bQ/5z/VvmcD2uzb4XqTutbnj9+rynfBD5AmEOncmD93hOH/myZKenJ8vK79D/BYjYkJ1T/G7HEfv4Nx13Qtv98gjupwD06jdTqvQb8ivRVd87/JJLufA9EbV9dB2CNb1c5XbTXli5LTCe6XtSn4/UvdCZXo6HsHvF617lw38/2H5T59XGFYeCp+7UtLTS967dQLLuW5wXUbnF+339pf/LPtw+Q7Nm/LrK0r6SUVceFwWLC/R7xctL43Hx2rXP4eWM392GUkby5MPE7sEkaRfyM/MfK08IbBzfn1r+U2oq2IvKTz/B/nBgjtzud6nZtzgOhq6fxOJye+F21zFxnM3yhPsr1HhkjH5vap+9mYF9vlaLOc1kubk5+cNvFe1T3TNkNcOyuX6+jrbvPBanX49Ghcd514+8P+F+e+sYd+97TYIrstov9emjDVuy+R93iYDr82R35TzwYp5Rcf+10taM7Beov1JNC46Hoh+v+g+WCjP1qLuRddndH7R8dxY8x815hctL43HZC2WMdTv1Zr2JBa4Tw/5z1a+Jb/uzQJJp8h/OrPEiLhQR9BiOcc2P41OBIQHptOw/Rp3/i3m9RENuS6s/KcQJ1TEHTTwmLru6yqSvjrubT5Tyqb8Z6nbDXl9e1UMwlos5+nysx9WLry2svyuxWeO8/vJ74LcdnlfKb/27p3jXhdjWp+d1b0Wy9h13Wu93Rt+v67r+hElbeA6kn7Wo+UMbYdgXd9Y0gXyG6T8TNIz8usrStpvAt8tVKZnyqNF3QvtHMgH588oeW/ncS/nNKyXUL+XP7dBXj/rNVzWLsdl0X49Wl46HR9Hl7PLR24DT5N0qqT1JP1Pbg+vkvT8EbHRRGPjZFUkJr/Xus1Vg/Gc/OzC4mPlwvzOCmyfyn2+FssZTVR9XYVrGhde30vS3yviov16eFwWacvU4gB3YBtE12Wo32tTxiJtmeInwETH/m+T3yR3aHkf53drGRcdD4S+X5uH4nm2SN0L95eR+bVYJ13nPzodrwaXcaz93mLTnu4v18HKW09+Ovvcgdcf0TkMvD/WjqDGcnY2P7UYmE7jduwk8deivDSOi27zmVQ2K9bLDhNYzuUkfVJ+Nsnv8uP/t3cvoZJcdRzHfz9nxjADvgVRULKQ+CCZXIkxiBCDKBIRzEIXQQiJK3eCi4AKJq40roMoogZhFqKbAQkiRidm4YNBJjPCREHwsYggRIhxLjPO8HdRZWjjvdPd/6rz76ry+4GGe6vvqTrn1P886tzqrov9ttc0OA+DY0Xdd0XdvEm6Xb2q2t6A/JW1vSHnPVm20rbe7/c96j7+JXVPDP+suru7fZ00u8hnZZ/7DnUfEW5+zqtjrPo14BykLw6q+4jiekmNeyPlufnYkC1fNl5UPD8eEteVr74PzMx3sguUWy9WZdKspC2dz0m6Q/87zn6k4fnL5vMuHbxQdXRNuoPmEWvLN8Z52Cbdyt9ts8B8Uv/9D+6b+u3X/Qf3gHNQWpcDYqx6AS8bK1vXZ7ZsA9INuUZJxUv1eVj5u23a3uAY2+Z4jeqlxfpH+TVYMp9Nxr2dF6xxpaWekrvBfh8oLkfZ8arLtmXeVgf/0fOp7i6EzFOVU+lanIcpxWaLemmRz0y6AbHSpE8qqL+mbW9Avkrb3hJies0+H+oneWfVPYn7p5K+KOnnkr4woXyWnfe+zT5Tdc6nFGPVrxbjXos+d0rj7K7zucuxobpe5lK+Bvlo0gdWnocW43q2bzlgnH1i6Di7wfmrnCel5hEDzsMoY+YYfdlh6UaMlU3rclLXGmP3ZQNiZTJz3BbpWpRvTV5GibOWba/V8dbsfzLz+BblS+aj2bi388I1rrgL6v8jIunGvgI/0/++8XdDH7DfPw/N21SPV122KeUzGy8t4ixbvinFZqv2N4X6nFKsVL+m1EdUt70pnb+GfeARdR8pfV7SK/vtx5X8vuYp9dWZfFaf8ynFWPWrxbg3pfF5SvUypXzOpV7mUr4G+ZjUtVQmXYs+YmC6UcfZ6vO3QX1uXb7q81AZm9Wx0qrNDojBUfuyKbW9sWNlSLql9y1TSlddLwPyMqV5RJPYPKplSz8l1/b5w95S932xy261AAAEvklEQVR9o6o8XnXZsnaQz2y8pNJlyzej2BzjKdUbK67P0lipNpc+QsVtL3u8rB2ch6sRcU3SJdt/iIjnJSki9m0f+kTzufTVxW09axZ9RNYOxr3qPiLl/2A+UHo86nNU5ddSmXQ7GNez6VLj7ADVfWC2fEu+BquOlfJ5RHFfVlqfMxqHFt23zGVc1/KvFTOaxebSF7P/ansvIs5JUkS8YPujkr4t6ZY1ad8g6cOS/v6S7Vb38IexVR6vumxZ1fnMxks2XbZ8c4nNIe2vMp+ZdNWxUm0ufUR125tLTGddsX0iIi5Juu3Fg9mvknS9ycZc+urKtp41lz4iq3rcq+4jspY+H6g+HvU5nl1cS2XSVfcR2XTZcTarug/Mlm/J12DVsbKLeURlX1Zdn3MZh5bet8xlXF/6tWJGs9hc+mL2fZKurm6IiKuS7rP9jTVpf6juIwLnXvqG7TOj5XA3x6suW1Z1PrPxkk2XLd9cYnNI+8uorM/qWKk2lz6iuu3NJaaz7oyIy5IUEauTi2Pqnhh+mLn01ZVtPWsufURW9bhX3UdkLX0+UH086nM8u7iWyqSr7iOy6bLjbFZ1H5gt35KvwapjZRfziMq+rLo+5zIOLb1vmcu4vvRrxYxmsenovq8EAAAAAAAAAIDJetmuMwAAAAAAAAAAwDosZgMAAAAAAAAAJo/FbAAAAGAEtq/ZPmf7t7a/b/vEgH3db/vRAWnfdMh7j9n+eP/zGdu/s33e9jO2H7X96myeAQAAgNZYzAYAAADGsR8RexFxs6Qrkj69+qY7FfPv+yUduJh9gE9GxElJJyVdlnS6VaYAAACAoVjMBgAAAMb3lKS32r7R9kXbX5P0G0lvtn2v7Qv9HdyP/CeB7Qds/972k5Let7L9xbup+99fWPn5wX5fT9v+Sv9375Z0qr9L/PgmmY2IK5IelPQW27cOLTwAAADQAovZAAAAwIhsH5V0t6QL/aa3SfpuRLxL0r8kPSLpA5L2JN1u+x7bb5T0JXWL2B+S9M4NjnO3pHsk3RERt0r6akT8QNJZdXdc70XE/qb5johrkp6W9PZN0wAAAACVju46AwAAAMBCHLd9rv/5KUnfUvd1H3+KiF/222+XdCYi/iZJtk9JurN/b3X79yTdtOZ4H5T0nYi4JEkR8dwIZfAI+wAAAACaYDEbAAAAGMd+ROytbrAtSf9c3XSd9HHI9qvqP1HpbocvX9nXYWm2ZvuIpFskXRxrnwAAAMCY+JoRAAAAoM6vJL3f9uv7xeN7JT3Zb7/L9utsH5P0iZU0f5R0W//zxyQd63/+saRP2T4hSbZf22//h6RXbJOp/phflvSXiDi/dakAAACAAtyZDQAAABSJiGdtf07Sz9TdWf14RJyWJNsPS/qFpGfVPSzySJ/sm5JO2/61pCfU3+kdET+yvSfprO0rkh6X9HlJj0n6uu19Se9d873Zp2xflnSDpJ+oWywHAAAAJskRo30yEQAAAAAAAACAJviaEQAAAAAAAADA5LGYDQAAAAAAAACYPBazAQAAAAAAAACTx2I2AAAAAAAAAGDyWMwGAAAAAAAAAEwei9kAAAAAAAAAgMljMRsAAAAAAAAAMHksZgMAAAAAAAAAJu/f+Z1rxPaQsLYAAAAASUVORK5CYII=
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[18]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">bot_100</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="o">.</span><span class="n">tail</span><span class="p">(</span><span class="mi">100</span><span class="p">)</span>

<span class="c1">#Using bar plot to describe the frequency of a product is purchased.</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">bot_100</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Freq&#39;</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">25</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
<span class="n">title</span> <span class="o">=</span> <span class="s2">&quot;The least 100 products that are frequently purchased&quot;</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="n">title</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">15</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlabel</span><span class="p">(</span><span class="s2">&quot;Product ID&quot;</span><span class="p">)</span> <span class="c1">#Label the x-axis</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="s2">&quot;Frequency Purchased&quot;</span><span class="p">)</span> <span class="c1">#label the y-axis</span>
<span class="n">ax</span><span class="o">.</span><span class="n">get_legend</span><span class="p">()</span><span class="o">.</span><span class="n">remove</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="City-Category"><section id="citycategory">City Category</section><a class="anchor-link" href="#City-Category">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Graphing-the-amount-of-purchase-from-different-city-category">Graphing the amount of purchase from different city category<a class="anchor-link" href="#Graphing-the-amount-of-purchase-from-different-city-category">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[19]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">groups</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;City_Category&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">groups</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;City_Category&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase From A City Category&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;City Category&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase in U.S Dollar&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[19]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;The Amount of Purchase in U.S Dollar&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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L3kJN91001of89JLL2XnnXdeB9V1z2sEJUmSJE2r7d/xjXV6vEs/8FeTbnPf+96Xs88+G4ADDjiAo446ikMOOWSo469atYqNNlq/o5Q9gpIkSZJ67UlPehIXXXTR3Xr0PvShD3H44YcD8JSnPIV3vvOd7Lnnnnz0ox/lD3/4A/vuuy/z5s1j3rx5/PCHPwTg9ttv5zWveQ077bQTe+21FzfffDMAxxxzDLvtthvz5s3jRS960Z97IL/yla+w8847M2/ePJ785Cf/+RiHHnoou+22G7vuuiuf/vSn1/lrNghKkiRJ6q1Vq1bxzW9+k1122WXSba+77jq+973v8ba3vY03velN7LnnnpxzzjmcddZZ7LTTTgBceOGFvP71r+e8885js80248QTTwTghS98IWeccQbnnHMOO+64I8ceeywARxxxBKeeeirnnHMOS5YsAeDYY49l00035YwzzuCMM87gmGOO4ZJLLlmnr9sgKEmSJKl3br75ZubPn8+CBQuYM2cOBx988KT7vOxlL/vz8+985zu87nWvA5rrDTfddFMA5s6dy/z58wF43OMex6WXXgrAueeey5Oe9CR22WUXvvjFL3LeeecBsMcee3DQQQdxzDHHcPvttwPw7W9/m89//vPMnz+fhQsXsmLFCi688MJ19trBawQlSZIk9dDgNYIjNtpoI+64444/L4++PcP973//SY97n/vc58/PZ8yY8eehoQcddBAnnXQS8+bN43Of+xynn346AEcddRQ/+clP+MY3vsH8+fM5++yzqSo+/vGP86xnPWtNX96k7BGUJEmSJGCrrbbiyiuvZMWKFdx6662cfPLJ42779Kc/nSOPPBJorum74YYbJjz2ypUr2Xrrrbntttv44he/+Of23/zmNyxcuJAjjjiCLbfckssvv5xnPetZHHnkkdx2220A/PrXv+bGG29cB6/wTvYISpIkSRKw8cYb8+53v5uFCxcyd+5cHvWoR4277Uc/+lEWLVrEsccey4wZMzjyyCPZeuutx93+fe97HwsXLmS77bZjl112YeXKlQAceuihXHjhhVQVT3/605k3bx677rorl156KY997GOpKmbNmsVJJ520Tl9rqmqdHnA6LViwoJYuXTrdZUiSJEmawPnnn8+OO+443WWs98b6PiY5s6oWTLavQ0MlSZIkqWcMgpIkSZLUMwZBSZIk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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Graphing-Frequency-Distribution-of-Product-Categories">Graphing Frequency Distribution of Product Categories<a class="anchor-link" href="#Graphing-Frequency-Distribution-of-Product-Categories">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[20]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Create a frequency table of Product_Category from category_table</span>
<span class="n">freq_category</span> <span class="o">=</span> <span class="n">category_table</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">&#39;Product_Category&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">count</span><span class="p">()</span>
<span class="n">freq_category</span> <span class="o">=</span> <span class="n">freq_category</span><span class="o">.</span><span class="n">drop</span><span class="p">([</span><span class="s1">&#39;Age&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="c1"># Plotting the distribution with bar chart</span>
<span class="n">ax</span><span class="o">=</span><span class="n">freq_category</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">kind</span><span class="o">=</span><span class="s1">&#39;bar&#39;</span><span class="p">,</span> <span class="n">legend</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">10</span><span class="p">,</span><span class="mi">6</span><span class="p">))</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xticklabels</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">19</span><span class="p">))</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_title</span><span class="p">(</span><span class="s2">&quot;Frequency Distribution of Product Categories&quot;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlabel</span><span class="p">(</span><span class="s2">&quot;Categories&quot;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="s2">&quot;Counts&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[20]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;Counts&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Top-5-selling-products"><section id="7">Top 5 selling products</section><a class="anchor-link" href="#Top-5-selling-products">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Find-The-Target-audiance-for-top-5-best-selling-products">Find The Target audiance for top 5 best selling products<a class="anchor-link" href="#Find-The-Target-audiance-for-top-5-best-selling-products">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[21]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">freq_purchase_by_PID</span> <span class="o">=</span>  <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">Product_ID</span><span class="o">.</span><span class="n">count</span><span class="p">()</span><span class="o">.</span><span class="n">to_frame</span><span class="p">()</span> <span class="c1"># counting the frequency for each product</span>
<span class="n">freq_purchase_by_PID</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">freq_purchase_by_PID</span><span class="o">.</span><span class="n">Product_ID</span> <span class="c1">#create a new column named &quot;Freq&quot;</span>
<span class="n">freq_purchase_by_PID</span> <span class="o">=</span> <span class="n">freq_purchase_by_PID</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span> 
<span class="n">freq_purchase_by_PID</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">top_5</span> <span class="o">=</span> <span class="n">freq_purchase_by_PID</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">],</span> <span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
<span class="n">top_5</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[21]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Product_ID</th>
      <th>Freq</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2534</th>
      <td>P00265242</td>
      <td>1858</td>
    </tr>
    <tr>
      <th>1014</th>
      <td>P00110742</td>
      <td>1591</td>
    </tr>
    <tr>
      <th>249</th>
      <td>P00025442</td>
      <td>1586</td>
    </tr>
    <tr>
      <th>1028</th>
      <td>P00112142</td>
      <td>1539</td>
    </tr>
    <tr>
      <th>565</th>
      <td>P00057642</td>
      <td>1430</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>It looks like our best 5 selling products are:</p>
<ul>
    <li>P00265242 = 1858</li>
    <li>P00110742 = 1591</li>
    <li>P00025442 = 1586</li>
    <li>P00112142 = 1539</li>
    <li>P00057642 = 1430</li>
</ul>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Having found the top selling products, one thing we could be interested in is finding the target occupation to advertise/appeal to when considering these five products.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[22]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Most sold product</span>
<span class="n">top_5</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">isin</span><span class="p">([</span><span class="s1">&#39;P00265242&#39;</span><span class="p">,</span><span class="s1">&#39;P00110742&#39;</span><span class="p">,</span><span class="s1">&#39;P00025442&#39;</span><span class="p">,</span><span class="s1">&#39;P00112142&#39;</span><span class="p">,</span><span class="s1">&#39;P00057642&#39;</span><span class="p">])]</span>
<span class="n">groups</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Occupation&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">groups</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Occupation&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase By Different Occupations&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Occupation&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;The Amount of Purchase in U.S Dollar&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[22]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;The Amount of Purchase in U.S Dollar&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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I8gBAACMjCAHAAAwMhtqHzkAAGDju+qqq7Jp06Z8//vfn3cpo7Xzzjtn7733zk477bRFjxfkAACAzbJp06bsuuuu2XfffVNV8y5ndLo7l156aTZt2pT99ttvi9owtBIAANgs3//+93Pzm99ciNtCVZWb3/zmW9WjKcgBAACbTYjbOlv7/AlyAADA6Oywww455JBDcsABB+TRj350vvvd7251m+eee24OOOCAdahu9uwjBwAAbJV9X/iedW3v3Jf//Jrz3PjGN86pp56aJHn84x+f17zmNXne8543VftXX311dtxx3FFIjxwAADBq97nPffLlL3/5Oj1qf/Inf5JjjjkmSXL/+98/v/M7v5P73e9+eeUrX5lvfOMbeeQjH5mDDz44Bx98cD72sY8lSX74wx/maU97Wvbff/886EEPyve+970kyWtf+9ocdthhOfjgg/NLv/RLP+oBfPvb354DDjggBx98cO573/v+qI0XvOAFOeyww3LQQQflr//6r9d9nQU5AABgtK6++ur88z//cw488MA1573sssvykY98JM9//vPzrGc9K/e73/1y2mmn5TOf+Uz233//JMlZZ52VZzzjGTnjjDOyxx575B3veEeS5FGPelQ+/elP57TTTstd7nKXHHfccUmSl73sZXnf+96X0047Le9617uSJMcdd1x23333fPrTn86nP/3pvPa1r80555yzrustyAEAAKPzve99L4ccckgOPfTQ7LPPPnnqU5+65mMe85jH/Oj6Bz/4wfzGb/xGksn+drvvvnuSZL/99sshhxySJLnHPe6Rc889N0ly+umn5z73uU8OPPDAnHDCCTnjjDOSJPe+971z1FFH5bWvfW1++MMfJkne//7352/+5m9yyCGH5PDDD8+ll16as846a93WPbGPHAAAMEKL95FbsOOOO+aaa6750e2lh/ffZZdd1mz3Rje60Y+u77DDDj8aWnnUUUflxBNPzMEHH5zjjz8+H/7wh5Mkr3nNa/LJT34y73nPe3LIIYfk1FNPTXfnVa96VR784Adv6eqtSY8cAABwvXDLW94yF110US699NJceeWVOemkk1ac98gjj8yrX/3qJJN92i6//PJV277iiity61vfOldddVVOOOGEH03/yle+ksMPPzwve9nLsueee+b888/Pgx/84Lz61a/OVVddlST50pe+lO985zvr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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>It would seem that Occupation 4 and 0 are the top buyers of our products. Say that these two occupations are business related. We could use this information to put an ad over these products with a person in a business suit enjoying the product.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>We can see from our previous graphs that the top selling 
product is P00265242. The top consumer city is city B. Now lets try to advertise the best selling product in the 
largest consumer city.
Our goal is to make an ad that appeals to the largest consumer group of product P00265242 in city B.
When making the ad we need to take into account the target age group, the taget gender, and the target marital status</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[23]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Highest spending city</span>
<span class="n">city_B</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s2">&quot;City_Category&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;B&quot;</span><span class="p">]</span>
<span class="c1">#Most sold product</span>
<span class="n">city_B_best_seller</span> <span class="o">=</span> <span class="n">city_B</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">city_B</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">]</span><span class="o">==</span><span class="s1">&#39;P00265242&#39;</span><span class="p">]</span>
<span class="c1">#city_b_cat_5 = pd.merge(city_A,catagory_5, on=&#39;Product_ID&#39;, how=&#39;inner&#39;)</span>
<span class="n">freq_purchase_by_age</span> <span class="o">=</span>  <span class="n">city_B_best_seller</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Age&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">Product_ID</span><span class="o">.</span><span class="n">count</span><span class="p">()</span><span class="o">.</span><span class="n">to_frame</span><span class="p">()</span>
<span class="n">freq_purchase_by_age</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">freq_purchase_by_age</span><span class="o">.</span><span class="n">Product_ID</span> <span class="c1">#create a new column named &quot;Freq&quot;</span>
<span class="n">freq_purchase_by_age</span> <span class="o">=</span> <span class="n">freq_purchase_by_age</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span> 
<span class="n">freq_purchase_by_age</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">freq_purchase_by_age</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Age&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Freq&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Age Groups that live in city B&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Amount of Product P00265242 Purchased&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[23]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;Amount of Product P00265242 Purchased&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Unsuprisingly, based on graphs above, we can see that the target age group should be ages from 26 to 35. Now lets see how many of our taget
age are male or female.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">target</span> <span class="o">=</span> <span class="n">city_B_best_seller</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">city_B_best_seller</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span><span class="o">==</span><span class="s1">&#39;26-35&#39;</span><span class="p">]</span>
<span class="n">freq_purchase_by_gender</span> <span class="o">=</span>  <span class="n">target</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Gender&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">Product_ID</span><span class="o">.</span><span class="n">count</span><span class="p">()</span><span class="o">.</span><span class="n">to_frame</span><span class="p">()</span>
<span class="n">freq_purchase_by_gender</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">freq_purchase_by_gender</span><span class="o">.</span><span class="n">Product_ID</span> <span class="c1">#create a new column named &quot;Freq&quot;</span>
<span class="n">freq_purchase_by_gender</span> <span class="o">=</span> <span class="n">freq_purchase_by_gender</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span> 
<span class="n">freq_purchase_by_gender</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">freq_purchase_by_gender</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Gender&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Freq&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Gender Groups that live in city B&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Amount of Product P00265242 Purchased&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[24]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;Amount of Product P00265242 Purchased&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>We can now narrow our target group to 26-35 year old men. Lets see if the taget group is single or not</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[25]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">target</span> <span class="o">=</span> <span class="n">target</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">target</span><span class="p">[</span><span class="s1">&#39;Gender&#39;</span><span class="p">]</span><span class="o">==</span><span class="s1">&#39;M&#39;</span><span class="p">]</span>
<span class="n">freq_purchase_by_status</span> <span class="o">=</span>  <span class="n">target</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Marital_Status&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">Product_ID</span><span class="o">.</span><span class="n">count</span><span class="p">()</span><span class="o">.</span><span class="n">to_frame</span><span class="p">()</span>
<span class="n">freq_purchase_by_status</span><span class="p">[</span><span class="s1">&#39;Freq&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">freq_purchase_by_status</span><span class="o">.</span><span class="n">Product_ID</span> <span class="c1">#create a new column named &quot;Freq&quot;</span>
<span class="n">freq_purchase_by_status</span> <span class="o">=</span> <span class="n">freq_purchase_by_status</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;Product_ID&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span> 
<span class="n">freq_purchase_by_status</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">freq_purchase_by_status</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Marital_Status&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Freq&#39;</span><span class="p">,</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">figure</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Marital_Status&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Amount of Product P00265242 Purchased&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[25]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Text(0,0.5,&#39;Amount of Product P00265242 Purchased&#39;)</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>As an advertising company we should focus on creating an ad that will appeal to single men around the age of 25-36 who live in city B.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Let's continue with the previous scenario. Suppose this time we want to find a target age group for each product category.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="-Product-Category-"><section id="8"> Product Category </section><a class="anchor-link" href="#-Product-Category-">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Graphing-percentage-of-purchase-from-each-age-group-by-category">Graphing percentage of purchase from each age group by category<a class="anchor-link" href="#Graphing-percentage-of-purchase-from-each-age-group-by-category">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Find-the-target-audiance-for-each-product-category">Find the target audiance for each product category<a class="anchor-link" href="#Find-the-target-audiance-for-each-product-category">&#182;</a></h4>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[26]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Obtain a list of age groups</span>
<span class="n">age_column</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">Age</span><span class="o">.</span><span class="n">unique</span><span class="p">()</span>
<span class="n">age_column</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
<span class="c1"># Create a new dataframe for counting</span>
<span class="n">age_count</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">index</span><span class="o">=</span><span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">19</span><span class="p">),</span> <span class="n">columns</span><span class="o">=</span><span class="n">age_column</span><span class="p">)</span>

<span class="c1"># Obtain total purchases made by each age group for every category</span>
<span class="k">for</span> <span class="n">cate_num</span><span class="p">,</span> <span class="n">cate_group</span> <span class="ow">in</span> <span class="n">category_table</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">&#39;Product_Category&#39;</span><span class="p">):</span>
    <span class="n">count</span> <span class="o">=</span> <span class="n">cate_group</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">&#39;Age&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">count</span><span class="p">()</span>
    <span class="k">for</span> <span class="n">age_group</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">count</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
        <span class="n">age_count</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">cate_num</span><span class="p">,</span> <span class="n">age_group</span><span class="p">]</span> <span class="o">=</span> <span class="n">count</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">age_group</span><span class="p">,</span> <span class="s1">&#39;Product_Category&#39;</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[27]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># From raw value to percentage</span>
<span class="n">totals</span> <span class="o">=</span> <span class="n">age_count</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span><span class="o">.</span><span class="n">values</span>
<span class="n">age_17</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;0-17&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>
<span class="n">age18_25</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;18-25&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>
<span class="n">age26_35</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;26-35&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>
<span class="n">age36_45</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;36-45&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>
<span class="n">age46_50</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;46-50&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>
<span class="n">age51_55</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;51-55&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>
<span class="n">age55_</span> <span class="o">=</span> <span class="p">[</span><span class="n">i</span> <span class="o">/</span> <span class="n">j</span> <span class="o">*</span> <span class="mi">100</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_count</span><span class="p">[</span><span class="s1">&#39;55+&#39;</span><span class="p">],</span> <span class="n">totals</span><span class="p">)]</span>

<span class="c1"># plot</span>
<span class="n">barWidth</span> <span class="o">=</span> <span class="mf">0.85</span>
<span class="n">names</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">19</span><span class="p">))</span>
<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span><span class="mi">18</span><span class="p">))</span>

<span class="c1"># Set size</span>
<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">()</span>
<span class="n">fig</span><span class="o">.</span><span class="n">set_size_inches</span><span class="p">(</span><span class="mi">16</span><span class="p">,</span> <span class="mi">8</span><span class="p">)</span>

<span class="c1"># Create bars</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age_17</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#d699ff&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age18_25</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="n">age_17</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#99b3ff&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age26_35</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="p">[</span><span class="n">i</span><span class="o">+</span><span class="n">j</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_17</span><span class="p">,</span><span class="n">age18_25</span><span class="p">)],</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#80ffe5&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age36_45</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="p">[</span><span class="n">i</span><span class="o">+</span><span class="n">j</span><span class="o">+</span><span class="n">k</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span><span class="p">,</span><span class="n">k</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_17</span><span class="p">,</span><span class="n">age18_25</span><span class="p">,</span><span class="n">age26_35</span><span class="p">)],</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#80ff80&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age46_50</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="p">[</span><span class="n">i</span><span class="o">+</span><span class="n">j</span><span class="o">+</span><span class="n">k</span><span class="o">+</span><span class="n">l</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span><span class="p">,</span><span class="n">k</span><span class="p">,</span><span class="n">l</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_17</span><span class="p">,</span><span class="n">age18_25</span><span class="p">,</span><span class="n">age26_35</span><span class="p">,</span><span class="n">age36_45</span><span class="p">)],</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#ffff66&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age51_55</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="p">[</span><span class="n">i</span><span class="o">+</span><span class="n">j</span><span class="o">+</span><span class="n">k</span><span class="o">+</span><span class="n">l</span><span class="o">+</span><span class="n">m</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span><span class="p">,</span><span class="n">k</span><span class="p">,</span><span class="n">l</span><span class="p">,</span><span class="n">m</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_17</span><span class="p">,</span><span class="n">age18_25</span><span class="p">,</span><span class="n">age26_35</span><span class="p">,</span><span class="n">age36_45</span><span class="p">,</span><span class="n">age46_50</span><span class="p">)],</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#ffcc99&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">age55_</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="p">[</span><span class="n">i</span><span class="o">+</span><span class="n">j</span><span class="o">+</span><span class="n">k</span><span class="o">+</span><span class="n">l</span><span class="o">+</span><span class="n">m</span><span class="o">+</span><span class="n">n</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span><span class="p">,</span><span class="n">k</span><span class="p">,</span><span class="n">l</span><span class="p">,</span><span class="n">m</span><span class="p">,</span><span class="n">n</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">age_17</span><span class="p">,</span><span class="n">age18_25</span><span class="p">,</span><span class="n">age26_35</span><span class="p">,</span><span class="n">age36_45</span><span class="p">,</span><span class="n">age46_50</span><span class="p">,</span><span class="n">age51_55</span><span class="p">)],</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#ff9999&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;white&#39;</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="n">barWidth</span><span class="p">)</span>

<span class="c1"># Add title and labels</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">(</span><span class="n">r</span><span class="p">,</span> <span class="n">names</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Product Categories&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Percentage&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;Percentage of Purchases Made by Age Groups for Each Category&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">age_column</span><span class="p">,</span><span class="n">loc</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">bbox_to_anchor</span><span class="o">=</span><span class="p">(</span><span class="mf">1.0</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
<span class="c1"># Show graphic</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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WEjyAQAAAGQGWqggTVRUVOiSSy7J79Onz/477rjj48rpQ4cO3fHXv/615ZAhQz5btmxZ07KyslDHjh0jc+fOXRe9/rvvvtv0mGOOOSBJc+bMad2zZ899krR+/fpwly5dIqFQSAsXLmxeUVGh3NzcuBN8iSQfAAAAQKaghQrSxKuvvnrEvHnzjurdu/e+wsLCIkmaOHHipuuuu277iBEjCnr37n10dnZ2xfTp09fGaqo/bty4LmvWrGlmZq5Lly4HH3300WJJevLJJ9s89thjHbKyslyzZs0qZs2atSbW+jUhyQcAAACAZErXFggBaX1QJheJp0f8RMrLVs293Z955pm7nXNLY817/vnn19b2Hi+//PJHsaaPHz++ZPz48SVxBVqNzP9GAQBorNL1pFEKzIkjANSLdG2BEJDWB7WNaX8Y5dVncQ2O/74IjopIev5QVUSkEIcagCRI15NGKT1/jwEAaATIPBAcobCkH6Q6ikOFfpvqCAAAAAA0EondwQ8AAAAAANIWST4AAAAAAAFBc30gldK1HwGJvgQAAACADMQZPJBK6dqPgERfAgAAAEA19u7dayeeeGLhwYMHrby83IYOHVo6derUzRUVFbr++uvz5s+f3yYUCrkrrrii5LbbbttWXTmjRo3qOmfOnHZ79+59W5IeeOCBoyZMmNAlNze3TJKuuuqqbWPHjt2eSGwk+QAAoOHQggkAUM/KVDYgW9n19gNeprJItrJrHJavWbNmbsmSJatbtWpVceDAAfvqV7/a97XXXtu5fPnyZhs3bsz+6KOPlmdlZWnTpk3VxvX3v/+9+c6dOw+ZP3To0NJZs2atP9z4+U8GAACJZ8OhBRMAoJ5lKzs8URPrrbwJmlDrP95QKKRWrVpVSNLBgwctEomYmWnmzJkdnnnmmTVZWVmSpLy8vEis9SORiG666aYuzz333Np+/fq1rrfgRZIPAACJJwAASFgkElH//v2L1q9f33TUqFHbTj/99D0bNmxo+sQTT7R54YUX2rRt2zby8MMPrz/mmGMOVF337rvv7nDOOefsyM/PL6s676WXXmrdp0+fI3r06LH/oYce2tCrV69DlqkJvesDAAAAAJCgcDisVatWrVi/fv2y//73vy3+85//NDt48KA1a9bMLV++fOWVV15ZMnr06IKq661bty573rx5bcaPH3/IvfoXX3zxjvXr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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>What an interesting find! As we have observed in previous graphs, the 26 to 35 age group was the overall biggest spender. However, as you can observe, they are not only the top spenders overall, they are the top spenders for every category. <br>
In the role of a retailer or advertising agency this information is invaluable. Not only does it tell us the age groups that spend the most across the board, 18 to 45, it shows us how little groups like 0 to 17 and 55+ spend.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Hypothesis-testing-for-the-mean-of-different-groups-of-age"><section id="hypothesis">Hypothesis testing for the mean of different groups of age</section><a class="anchor-link" href="#Hypothesis-testing-for-the-mean-of-different-groups-of-age">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Next, we are going to perform hypothesis testing on the mean purchase of male and female at significant level α = 0.05. <br>
Base on the previous observation, <br>
the <b>null hypothesis</b> is that mean purchase made by males and females are equal, and <br>
our <b>alternative hypothesis</b> is mean purchase made by males and females are different.</p>
<p>$
H_0 : μ_{male} = μ_{female} \\
H_1 : μ_{male} ≠ μ_{female} \\
α = 0.05
$</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[28]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">female_Purchase</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Gender&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;F&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">male_Purchase</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Gender&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;M&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="c1"># Perform a standard independent 2 sample test that assumes equal population variances for male and female</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;2 sample test (assuming equal variance)&quot;</span><span class="p">)</span>
<span class="n">f_val</span><span class="p">,</span> <span class="n">p_val</span> <span class="o">=</span> <span class="n">stats</span><span class="o">.</span><span class="n">ttest_ind</span><span class="p">(</span><span class="n">male_Purchase</span><span class="p">,</span> <span class="n">female_Purchase</span><span class="p">)</span> 
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;F-statistic = &quot;</span><span class="p">,</span> <span class="n">f_val</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;P-value = &quot;</span><span class="p">,</span> <span class="n">p_val</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>2 sample test (assuming equal variance)
F-statistic =  44.13462293864972
P-value =  0.0
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Because the p-value = 0.0 &lt; α = 0.05, there is enough evidence to prove that mean purchase made by males is significantly different female.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[29]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># perform Welch’s t-test, which does not assume equal population variance </span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Welch’s t-test&quot;</span><span class="p">)</span>
<span class="n">f_val</span><span class="p">,</span> <span class="n">p_val</span> <span class="o">=</span> <span class="n">stats</span><span class="o">.</span><span class="n">ttest_ind</span><span class="p">(</span><span class="n">male_Purchase</span><span class="p">,</span> <span class="n">female_Purchase</span><span class="p">,</span> <span class="n">equal_var</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> 
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;F-statistic = &quot;</span><span class="p">,</span> <span class="n">f_val</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;P-value = &quot;</span><span class="p">,</span> <span class="n">p_val</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Welch’s t-test
F-statistic =  45.67264701908008
P-value =  0.0
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Because the means are significantly different, we should expect the variance of these two population also differ. <br>For different population variance, Welch's t-test will have a higher accuracy. <br>Result of Welch's t-test also indicates the population means are different since the p-value = 0.0 &lt; α = 0.05.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Analysis-of-Variance-"><section id="ANOVA">Analysis of Variance </section><a class="anchor-link" href="#Analysis-of-Variance-">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>For three or more population means, performing three or more hypothesis testing separately with <b>null hypothesis</b> $H_0: μ_1 = μ_2 = ... = μ_n$ would increase the probability of <b>Type I Error</b> (rejection of a true null hypothesis) so that it could be much higher than the level of significant α. <br><br>
In stead of a 2 sample t-test,
<b>Analysis of Variance (ANOVA)</b> is an inferential method used to test the equality of three or more population means.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now let's perform an ANOVA on the mean purchase of each age group. As the previous graphs show, different age groups have different purchase power. We are going to test if the mean purchases of different age group is statistically significantly different.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Using scipy.stats to perform 1-way ANOVA that tests the null hypothesis that two or more groups have the same population mean.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[30]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">age_17</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;0-17&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">age18_25</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;18-25&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">age26_35</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;26-35&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">age36_45</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;36-45&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">age46_50</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;46-50&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">age51_55</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;51-55&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>
<span class="n">age55_</span><span class="o">=</span> <span class="n">blackfriday</span><span class="p">[</span><span class="n">blackfriday</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;55+&#39;</span><span class="p">][</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]</span>

<span class="n">f_val</span><span class="p">,</span> <span class="n">p_val</span> <span class="o">=</span> <span class="n">stats</span><span class="o">.</span><span class="n">f_oneway</span><span class="p">(</span><span class="n">age_17</span><span class="p">,</span> <span class="n">age18_25</span><span class="p">,</span> <span class="n">age26_35</span><span class="p">,</span> <span class="n">age36_45</span><span class="p">,</span> <span class="n">age46_50</span><span class="p">,</span> <span class="n">age51_55</span><span class="p">,</span> <span class="n">age55_</span><span class="p">)</span> 
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;One-way ANOVA&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;F-statistic = &quot;</span><span class="p">,</span> <span class="n">f_val</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;P-value = &quot;</span><span class="p">,</span> <span class="n">p_val</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>One-way ANOVA
F-statistic =  43.48718107271441
P-value =  1.9552104879020313e-53
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Using Statsmodels to produce ANOVA table</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[31]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">model</span> <span class="o">=</span> <span class="n">ols</span><span class="p">(</span><span class="s1">&#39;Purchase ~ Age&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">blackfriday</span><span class="p">)</span><span class="o">.</span><span class="n">fit</span><span class="p">()</span>
<span class="n">anova_table</span> <span class="o">=</span> <span class="n">sm</span><span class="o">.</span><span class="n">stats</span><span class="o">.</span><span class="n">anova_lm</span><span class="p">(</span><span class="n">model</span><span class="p">,</span> <span class="n">typ</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
<span class="nb">print</span> <span class="p">(</span><span class="n">anova_table</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>                sum_sq        df          F        PR(&gt;F)
Age       6.470585e+09       6.0  43.487181  1.955210e-53
Residual  1.333110e+13  537570.0        NaN           NaN
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Sure enough, since the p-value is significantly small, we have enough statistical evidence to prove that the mean purchase of different age group is significantly different.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Linear-Regression-"><section id="9">Linear Regression </section><a class="anchor-link" href="#Linear-Regression-">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="A-simple-linear-regression-of-purchases-:-Purchases-=-B0-+-B1-*-Frequency">A simple linear regression of purchases : Purchases = B0 + B1 * Frequency<a class="anchor-link" href="#A-simple-linear-regression-of-purchases-:-Purchases-=-B0-+-B1-*-Frequency">&#182;</a></h4>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[32]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">display</span><span class="p">(</span><span class="n">freq_purchase</span><span class="o">.</span><span class="n">head</span><span class="p">())</span>
<span class="n">X</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="p">[[</span><span class="s1">&#39;Freq&#39;</span><span class="p">]]</span><span class="o">.</span><span class="n">values</span><span class="o">.</span><span class="n">reshape</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">freq_purchase</span><span class="p">[[</span><span class="s1">&#39;Purchase&#39;</span><span class="p">]]</span>
<span class="n">X_train</span><span class="p">,</span> <span class="n">X_test</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="n">y_test</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">test_size</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">reg</span> <span class="o">=</span> <span class="n">linear_model</span><span class="o">.</span><span class="n">LinearRegression</span><span class="p">()</span>
<span class="n">reg</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">)</span>
<span class="n">display</span><span class="p">(</span><span class="s2">&quot;Intercept: &quot;</span><span class="p">,</span> <span class="n">reg</span><span class="o">.</span><span class="n">intercept_</span><span class="p">,</span> <span class="s2">&quot;Coefficient: &quot;</span><span class="p">,</span> <span class="n">reg</span><span class="o">.</span><span class="n">coef_</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>



<div class="output_html rendered_html output_subarea ">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Product_ID</th>
      <th>Freq</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>265242</td>
      <td>1858</td>
      <td>13983325</td>
    </tr>
    <tr>
      <th>1</th>
      <td>110742</td>
      <td>1591</td>
      <td>26382569</td>
    </tr>
    <tr>
      <th>2</th>
      <td>25442</td>
      <td>1586</td>
      <td>27532426</td>
    </tr>
    <tr>
      <th>3</th>
      <td>112142</td>
      <td>1539</td>
      <td>23882624</td>
    </tr>
    <tr>
      <th>4</th>
      <td>57642</td>
      <td>1430</td>
      <td>22493690</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_text output_subarea ">
<pre>&#39;Intercept: &#39;</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_text output_subarea ">
<pre>array([-244185.19322591])</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_text output_subarea ">
<pre>&#39;Coefficient: &#39;</pre>
</div>

</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_text output_subarea ">
<pre>array([[10832.34609059]])</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Our linear model is Purchase = -244185.20 +  10832.35 * Frequency</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[33]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">y_pred</span> <span class="o">=</span> <span class="n">reg</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
<span class="n">y_pred</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[33]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>array([[5345305.38951792],
       [ 145779.26603529],
       [1683972.4108989 ],
       ...,
       [-222520.50104473],
       [ 828217.06974238],
       [ 286599.76521294]])</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Let's plot this model's prediction</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[34]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="s2">&quot;b.&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">X_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">,</span> <span class="s2">&quot;r-&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAXcAAAEDCAYAAADOc0QpAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMS4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvNQv5yAAAIABJREFUeJztnXmcXFWZ979PVS/GkbXBAQMhOCIQjSbSLC1DaBaBoEAEFxYJohKCxNcoEQFfJSMzRlAYBlCSVsKkgUEYg8BowmqaZVIs2RAhLJE1JAgGNfCSvc/7x6mbulV9a+uuvX7fz6c+VXXuufc+dav7d0895znPY845hBBCNBaxahsghBCi9EjchRCiAZG4CyFEAyJxF0KIBkTiLoQQDYjEXQghGpCqiruZzTazN8zsjwX0/XczW5Z8PGdmf6uEjUIIUY9YNePczWwc8A7Q65z7aBH7fQMY65z7StmME0KIOqaqI3fn3IPAW+E2M/snM7vLzBab2UNmtk/ErqcAN1fESCGEqENaqm1ABD3AZOfc82Z2IPBz4PBgo5ntAewJ/L5K9gkhRM1TU+JuZu8DPgn8t5kFze0Z3U4Gfu2c21JJ24QQop6oKXHHu4n+5pwbk6PPycC5FbJHCCHqkpoKhXTOrQVeNLPPA5jn48F2M9sb2AFIVMlEIYSoC6odCnkzXqj3NrOVZvZV4DTgq2b2BPAUcEJol1OAXzmlshRCiJxUNRRSCCFEeagpt4wQQojSULUJ1Z122smNHDmyWqcXQoi6ZPHixX9xzu2cr1/VxH3kyJEsWrSoWqcXQoi6xMxeLqSf3DJCCNGASNyFEKIBySvuZra7mS0ws+Vm9pSZfTOiT7eZ/T2UtfEH5TFXCCFEIRTic98MnOecW2Jm2wCLzexe59zTGf0ecs59pvQmCiGEKJa8I3fn3Grn3JLk67eB5cDwchsmhBBi8BTlczezkcBY4NGIzV1m9oSZzTezj2TZf5KZLTKzRW+++WbRxgohhCiMgsU9mbFxLjA1mQMmzBJgD+fcx4GrgdujjuGc63HOdTrnOnfeOW+YphCiRkgkYMYM/yzqg4Li3M2sFS/sNznnbsvcHhZ759w8M/u5me3knPtL6UwVQlSDRAKOOAI2boS2Nrj/fujqqrZVIh+FRMsYcB2w3Dl3RZY+uyT7YWYHJI+7ppSGCiGqQ1+fF/YtW/xzX1+1LRKFUMjI/WDgdOBJM1uWbLsIGAHgnJsJfA44x8w2A+uAk5W5UYjGoLvbj9iDkXt3d7UtEoWQV9ydcw8DlqfPNcA1pTJKCFE7dHV5V0xfnxd2uWTqg1qrxCSEqEG6uooT9URCN4NqI3EXQpSUUk7A6iYxeCTuQoiSEjUBOxhhVpTO0FDiMCFESQkmYOPxoU3AKkpnaGjkLoQoKaWagFWUztCQuAshSk6xE7DZjqEoncEjcRdC1CyluEk0K/K5CyEiUT6Z+kYjdyHEABSpUv9o5C6EGIAiVeofibsQYgClCmcU1UNuGSHEABSpUv9I3IUQkShSpb6RW0YIIRoQibsQQjQgEnchhGhAJO5CCNGASNyFEKIBkbgLIUQDInEXQogGROIuhBANiMRdCCEaEIm7EEI0IBJ3IYRoQCTuQgjRgEjchRAlRRWcagNlhRRClAxVcKodNHIXoo6o9VGxKjjVDhq5C1En1MOoOKjgFNioCk7VQ+IuRJ0QHhWvXw+9vbUn7qrgVDtI3IWoE7q7oaXFi7tzMHs2TJxYewKqCk61QV6fu5ntbmYLzGy5mT1lZt+M6GNmdpWZrTCzP5jZJ8pjrhDNS1cXnHkmmPn3W7ZU16dd6/7/ZqeQkftm4Dzn3BIz2wZYbGb3OueeDvUZD+yVfBwIXJt8FkKUkIkTYc6c6vu068H/3+zkHbk751Y755YkX78NLAeGZ3Q7Aeh1nkeA7c1s15JbK0STE/i0L7mkuoKqqJjapyifu5mNBMYCj2ZsGg68Gnq/Mtm2OmP/ScAkgBEjRhRnqRACqA2ftqJiap+Cxd3M3gfMBaY659Zmbo7YxQ1ocK4H6AHo7OwcsF0IUR8oKqb2KUjczawVL+w3Oedui+iyEtg99H43YNXQzROidkgkJGZhauEXhMhOXnE3MwOuA5Y7567I0u1OYIqZ/Qo/kfp359zqLH2FqDs0gSjqjUJG7gcDpwNPmtmyZNtFwAgA59xMYB5wLLACeBc4s/SmClE9oiYQJe6ilskr7s65h4n2qYf7OODcUhklRK2hCURRb2iFqhAFoAlEUW9I3IUokGpPIGpCVxSDxF2IOkATuqJYlM9diDpAK0JFsUjchagDggndeFwTuqIw5JYRog7QhK4oFom7EHVCtSd0RX0ht4wQQjQgEnchhGhAJO5C1AiqbCRKiXzuQtQAimMXpUYjdyFqAMWxi1IjcRciD5VwlyiOXZQauWWEyEG53SXhfDGKYxelROIuRA7Kmcc96sZx4YWlObYQcssIkYNyukvkZxflRCN3IXJQzmX/KgAiyonEXYg8lGvZv/LFlIA334Tjj4eLLoLjjqu2NTWFxF2IKqJ8MYPk7bdh//3h2Wf9+xtvlLhnIJ+7EKJ+2LgRDj8ctt02Jew//Sncckt17apBJO5CiNqnvx++9CVob4cFC3zbtGm+/bzzqmtbjSK3jBCidnEOzj/fj84DTj0VbrgBYhqb5kLiLoSoTa64In1UfthhcNddPrRI5EXiLsQQCa8yrfTkaDXPXTZuvBFOPz31fu+94fHHYZttqmdTHSJxF2IIVDObY8NlkrzrLhg/PvV+m21gxQp4//urZ1MdI6eVEEOgmqtMG2aF62OPgVm6sL/wAqxdK2EfAhJ3IYZANbM51n0myWee8aJ+4IGptmXL/CTqnntWz64GQW4ZIYZANVeZ1u0K19deg9139yIesGBBHd6dahtz4QtcQTo7O92iRYuqcm4homjIycla4q9/hdGjvbgH/PrXcNJJ1bOpDjGzxc65znz9NHIXggacnKwl1q2DceMgPJi79lqYPLl6NjUB8rkLQQNNTtYSmzfDCSfAe9+bEvbp0707RsJedvKKu5nNNrM3zOyPWbZ3m9nfzWxZ8vGD0pspRHmp+8nJWiIQ79ZWuPNO33b22T5VwMUXV9e2JqIQt8x/AtcAvTn6POSc+0xJLBKiCtTt5GSt8cMfpgv4ccfBbbdBizzAlSbvFXfOPWhmI8tvihDVRel3h0BPjx+dB3R2woMPwrBh1bOpySmVz73LzJ4ws/lm9pFsncxskpktMrNFb775ZolOLYSoGrfd5mPVA2H/wAfgrbd8ugAJe1UpxW+lJcAezrl3zOxY4HZgr6iOzrkeoAd8KGQJzi2EqAYPPJA+MWEGr74Kw4dXzSSRzpBH7s65tc65d5Kv5wGtZrbTkC0TQtQeTzzhhTws7MuX+8lSCXtNMWRxN7NdzMySrw9IHnPNUI8rhKghXnzRi/qYMam2RMJHxuyzT/XsElnJ65Yxs5uBbmAnM1sJXAy0AjjnZgKfA84xs83AOuBkV61lr0IUSCIBvcn4r4kTNZGalTfegA99yNcsDZg/H445pno2iYJQ+gHRdCQS3quwcaN/39rqXcgS+BCZBajB3w3DedZFVSg0/YBWqIqmo68PNm1Kvd+0KTWKb3qyFaB2TsJeIhIJmDHDP5cTrSwQTUd3ty+/uWVLtS2pIfr7vX/qpptSbdOmwWWXeV+7KAmVzGGkkbuoGSo1ounqgp//3KcaMPP/ZBMnlvecNYtzXsTj8ZSwn3qqv/P95CcS9hJTyRxGGrmLmqDSWRlHj4azzvKvm3ZCVQWoK06Qwyj4Oy9nDiOJu6gJokY05RLczBtJ043aVYC6alQyh5HEXdQElRzRVPJGUlPMnw/HHpt6rwLUVaFSOYwk7qImqOSIppI3kprg0UfhoIPS2154QXVKGxyJu6gZKjWiKfRGUvdl9555BvbdN71t2TL4+MerY4+oKBJ30ZSEbyRRIl7XZfdUgFogcRdNTjYRr0u/vApQixCKcxdNTba447oqu7dunS+OseOOKWG/9lo/cpewNy0auYumJtvkal2U3du8GU48Ef7nf1Jt06erTqkAJO6iyQmLeEdHauQe+ORrUtSdg3POgVmzUm2TJ/tlt1pRKpJI3EXNUqloleDYdTGB+i//4kfnASpALbKgvwhRk1Q6WqXmJ1BnzfKj84D99/d5ilWnVGRBE6qiJqlkgiWo4QnUoAB1IOzDh/sC1I89JmEXOdHIXdQkxawiLYX7puYmUOuoAHXdL/ZqUCTuoiYpZhVpqdw32SZQKypeTzyRXqcUfAHqGq1TWteLvRocibuoKMUIZSHRKuX2lVdMvF58ET74wYEnz8wJU2PU/FxFEyOfu6gYgVB+//v+uRRFOcrtKw+L14YNPlClpMVE3njDl7QLC/v8+T7cscaFHWp4rkJI3EXlKMckaeC+ueSS8oyqA/GKxXwluvvuK9GN6e23vavlH//Rvwa44QYv6sccM1SzK0a5r78YPHLLiAGUy8dcbKrdQu0o52KjQLymT/fC3t8/RPfDxo1w9NHpd7af/jS9IlKdUbOLvZocibtIo5w+5mIiUhIJX/UtsGPBguLsKOUNqqvLi/tDDw0hB3x/v69+9F//lWr7znfg0ku1qlSUBYm7SKPcE2SFjvJ6e72PG/xzb6/frxDRLscNatChks55Eb/88lTbaaf5DxSTV1SUD4m7SKOWqxT19MCUKf7G096eXbTLdYMq2v1w+eUwbVrqvQpQiwqioYNIo1YmyCZO9Bpo5p/HjoVzz4VNm7yHY8OG7BOyVY/guPFGb3gg7HvvDWvXwu9/L2EXFUMjdzGAckyQFesD7+qCq6+GuXN9SvI1a7yoB8Tj2UW7aqtNVYBa1BASd1F2ivGB9/R4QR8zxov7xo1+IvPKK70rZsMG76q+5prqRdAMoIIFqLXUXxSKxF2UnUJ94D09cPbZ/vU993jPhnN+nzVraiz3C1S8ALWW+otikLiLslPoJO3cuenvzfwoPdgnajRelZHsa6/Bbrult1WgALWW+otiyCvuZjYb+AzwhnPuoxHbDfgP4FjgXeDLzrklpTZU1C+F+sBPOsmP2AOmTYPtt8++T8VHsn/9K3z0o7BqVapt7lxf6q4C1HIkk6g9Chm5/ydwDdCbZft4YK/k40Dg2uSzEFspxAc+aZJ/DiZRg/fZqNhIdt06OOQQWLw41TZzZsqHVCFqLi2xqGnyirtz7kEzG5mjywlAr3POAY+Y2fZmtqtzbnWJbBQNSDZ3yqRJ+UU9oOwj2RosQK2l/qJQSuFzHw68Gnq/MtkmcReRlMqdUraRrApQiwagFOIe9dfuIjuaTQImAYwYMaIEpxb1SCndKSUfyWYWoD7+eO8nUgFqUWeUYoXqSmD30PvdgFVRHZ1zPc65Tudc584771yCU4t6pOorSKOYNcuPypPC/s6++8O778Idd0jYRV1SCnG/E5honoOAv8vfLnJRzhQHiQTMmFFEvvWMAtSvMZydYm/x/pceI7FMBahhENdU1ASFhELeDHQDO5nZSuBioBXAOTcTmIcPg1yBD4U8s1zGiupR6njycqU4KNiXH1GA+urzX+VbPx3Oli0QVxw5oIVT9Uwh0TKn5NnugHNLZpGoOYr9B6/WEvmCfPk5ClB3JqDtKsWRh9HCqfpFzkSRl6g6otOn18jCohA5QyOjClA/8ggcmFqS0chx5IO94WrhVP0icRd5Cf7B16/3mRnvucd7NcLVkQLxeOWV4kd6pRrpR4rzG2/Ahz6UqlMKPntjljqljRhHPpQbbiPf8BodiXuTkU9Io7Z3dfmsjMk5R2BgdaRAPOJxH1zinM8L09GR357ubp+nvbV16D/7t4rz22/D3p3w3HOpjTfcAF/60uAPXuNk+26H6lppxBteMyBxbyLyjeBybV+zxgt21DGnT/diH+RbP+44+O1vvZhMnQqjR2cXh95efz7wz8ENY9A0YAHqQsj13cm10pyoElMTETWCy9y+YUPKtx7eHghEQGurr450xBFw331e2IMMjrvs4m8E/f3R5ykL/f1w6qk+6Xtwwu98x7c3uLBD9LxIELpYK9W1RGWRuDcR+RYPdXSkRt/9/ekulaAy0gEHwIQJvljG3LmpEXssBkce6cUjKJFXyCKliRO9Hpv554kTi/xQzvn0kfE43HyzbzvtNK9yl13WNOkCgu82FvPfx333+RtvWOAvvFDC3kzILdNE5JscW7MmJQ6xmH8fkEh4F8vGjT6acN48n1cr6Nvenh5BU8gkXOAjvuoqf66iJ+xUgHorwXc7fXrql5RCF5sbibvYSne3F+ko32z4Z38wug8mTY88cmBoZL5JuCGFTN54I5x+eur9PvvAY4/5mqVNTFeX/x4eekj+dSFxbyryCWqukX1Hh/dwBA9IuVKyxbznYlARHJkFqLfdFp5/vqkKUOeLdlLoogiQuNcZQ4kJL0RQg/e9vf4R+MCnTvX7OZeKmonHfYjkYASkqAiOChagrmUK/bWj0EUBEve6YqirPwsR1CDuPAhPvP56OPNM/z4zFLK/P90vXwwFjTArXIC61lEqAFEMEvc6ohSLUfIJal+fX1AUEIh8W1t6LDv4cMih+HQzR5jBr5KjPvIa+52QUYC6rw8OPXTwJ2sAFK8uikHiXkeU4p8730/27m4v2mFRnzjRP/r6vO996VK/beLE0o0cEwk46fC/smj9R/hAuIhXBQtQ1zryp4tiMBe17LACdHZ2ukWLFlXl3PXMYHzuxe6TSHh/OxQm4EPODbNuHS/vcQh7vJkqQD3/hJmMv72yBaiFqAfMbLFzrjNvP4l7Y1PuLI1DOn5EAeqLmc6l7RenJSUTQqQoVNy1QrXB6e312RyzpRyIIl/lnfD2fCkNInHOZyFrbd0q7NcyGaOfS+xizjxTwi7EUJHPvYHp6YFf/CI9dDGXnz5wx1x/vZ9Ujcd9moFJk9L7hEfqV15Z5DxARgHq5/Y9no8+M5dNzv8ptrQMIgWBEGIAEvcGJZGAc8/1I2rwC46+8pXcqQCOOMKP8oObQX+/P0Y4q2PmSH3NmgIn+WbOhHPOSb3ff3944AHWLBtGyxGwZYNf7XrNNRq1C1EKJO4NQuakZl9fStghfUQcNQEaiHZULHs45DIqYidnBM5tt8FJJ6XeDx8OTz4JO+wAVC8CpFqlAIWoFBL3BiBqUrOjI12ov/WtgYU1whOgQXqBWMy7Y/r7/f7t7emuloLFOLMAdSzmyzQNHz6ga6VXVKros2gGJO4NQLZJzXCGx7Vr/SRoVBk88OkF+vtTfvbRo7MLeE4xXrbMJ3oPkyxAXStopadoBiTuDUC2xU1Bhsd4HH75Sx952NLi30OqbyB2/f1+9L5mzSBG0wUUoK4EhbhbtNJTNAMS9zomLGRhVwn411de6YX6rrvgwQd9++bNMG4cjBqVOk4usYsSy7S2fyquAHUxn6nQGq/hbYUm1tJKT9HwOOeq8thvv/1cM7NwoXM/+pF/Hsx+s2Y5N2yYc7GYc62t/v3Chc5NmOBcPO7bhw3zbQccEORy9I999/Xb4vFUn1mznDvqKP8cPldmv6Btu9ha96x9OP3AN9ww5GvS1uacmX/OvDZR9oT50Y/8NvDPP/rRkMwRoiYBFrkCNFYj9ypQ6Agzc5SaSPhiQxs3evdJuCTe17/u2zZvTu2/fr0PKe/u9rUsAnbe2SdcdM4nA5s61VdX2rzZF3oIQh8zfdO9vfDKio38bt3RHEZf6oCXXw7f/vaQr0u+Ytn5fOXhXyAtLX5+IZHQyFw0JxL3KlDIhF7UDaC314sxDAxZDIc9BjjnS6499BCcf76f6xwzxrtrwrHsYeEP25MmlrF+unu+xBf7b97a94qW79D1wKV0fXLwdUrDN7B85POVB+6W3l6YPdsv4JozR9EwojlR+oEqkK9QNURXs3/66eLPFdTS3H57uPtu/xx1IwA/8g/b09UF99/nmP/RaazfFN8q7DdxGsd8agtdD142ZGE/4gj4/vf989ixuYtlB+J9ySXRgh3cKMB/xqJSIgjRYGjkXmaiJgALmdALbgBBDvX77st+jlGjvJslnGs9IBZLF+xM14VzXgTjcb+CNS0L5OWX0xUqQH0/h/Npm0/sPW3c/y9DHw0HeW+cS612XbAgfSQ/Y0Zhk57hXzpREUFCNB2FOObL8WiGCdV8E4CF7H/UUX5yNDxvGX6MG+fc5MnOtbf7icioPqNGDZwoDSZzIyd2e3vTDvA0+7j3sdbFYt6ewU4Ch/dbuNDbHJwmmEBduNB/nnHjBk4Mz5rlXEtLelvA5Mmpzx+L+feDmbAWotahwAlViXsZKUX0RnCDiBL41lYvivG4f54wwYtfthtBWODDx98qgvPmpe+w3Xbusd/+Oe8NKlO8w+9nzfJ2Zgpy+NqYeTHOFPzgYeYjfoL+gYAH13PhwoGfO+qzCtEIFCrucsuUkY4O7xZxrnj3QGYM+/Tp3jUTuF522w06O33G3KBw9apV8JnPwFtvwf/+70Df+ty50RkeP71hLhf2fy69c7IA9f7kdiFlTvx+4xvw7//uz93a6iNwAjs2bIierA2qPQXzDJk4lz7pC/66hmP6Mz/rYGu7CtEwFHIHAI4BngVWABdEbP8y8CawLPn4Wr5jNvrIPTzibmkpbiQZ5c4JXBKB68HMb4/HB7pj2tp8/wkTco9meyc9NGCYvGzOsqI+Z3gEHoul/8LItKu1daBrJnPEHzVyj3qcf376cdraUtva2+WOEY0LpRq5m1kc+BnwKWAl8LiZ3emcy4zduMU5N6U0t5z6J2pJfzYywwGnT09NNG7Y4Cce58xJHSuQsWxRL5s2+fOdfz787nf+fWurj18HfK6XUaM4PbTPROZwU2wi7ZPh/r0KnywNj8BjsfQ4+yAJ2ebN0el8wykOgmtw1VW+Ruvrr8Muu/jn229PP2cs5qN+wsfp6yuuNKAQjU4hbpkDgBXOuRcAzOxXwAnAIALzmodC85eE3RrxuBfvcOrd/n4vcMGNAlICn43W1lTOmPBCp0V3rqLrk+lZGV85+98468WLtrp8ik2k1dXl4+bnzvUx9Fdf7W9IsRj87GepBGQdHf6GE7WoqKfH543v7/chkOEwx0QidYMKPnss5o+XaYcEXYgUhYj7cODV0PuVQFQ2qJPMbBzwHPAt59yrmR3MbBIwCWDEiBHFW1tHRIU7ZsujHoQ7Bml2w8RifgTb0pI+Ug8yPkJK8A4+2IdFhkeuLS3wD1vW8vct28GPQwc+6yzo6WEEMD3hFzoNJpFWIuFXuG7c6I8R5LPJ9M9nW5GbSMCUKakRf9gvH2CW+ozgP/fUqelFRIQQ6RQi7lGrVDLHjf8D3Oyc22Bmk4E5wOEDdnKuB+gBXyC7SFvrjrCAP/lkSgQz86gHIh01Go/HU4t5Zs5M9XMuXfCcg8cfhx//OHVe27SR9Rva0w94+OH+5Bl2DiaRViDs4Vj1pUsh874dlcYgOFfmZKhZetqAYLtz6ddJqXqFyE0h4r4S2D30fjdgVbiDcy7sUf4FcOnQTat/wi6XIBdMputjzZr0UXgmX/iCf3799YHbsgreQQ6GD+eg1au39n2F3bnp317mwovS79XhXxMXXljcZ+vuTo9ucQ6uu86LceCWmTRp4MKp2bN9n6AGa3u7H7EHN6tw2oDwvoHbavNmLU4SIh+FiPvjwF5mtifwGnAycGq4g5nt6pwLlOR4YHlJraxTwiPWYHIxc4l/d7cXt3Dt0jDPP5+qbRpFPJ6atGxrg6//dzdc9EBan2GxDVh7G/cflr5vIQnMsqXY7etL+cEDgptX8HrKlJTrJPhl8MorXryjarBmbuvr8zecqHTGStUrRB4KCakBjsX70v8EfC/Z9kPg+OTrGcBTwBPAAmCffMds9FBI5waGNJ5//sC0us759+EFPeGQvyCFb1Q4YHjxz9LOrw7ssHZtztTC+RZZZUv5G6Qcbm3NHa4YtVI016rdoa7oFaIZQCtUa4NADM8/P/fS+cyUAsFNICx4ra0+lUAQ297a6twd+18yUFVXrSrYtmLyo0+enN4/M44+Kq69vX3g8XPdcAab516IZqFQcdcK1RKSLUkYwKGHpkeEhCcVM9lxRzjggHSXRm8vXH99KkHYROYwZ9OXvdMsIEet0qjc8OFqTVGVlv72t5QfvK3NbwtPjO6yCwwblopxf//7/SrZYLJ37FhYvHhgdsZcbhWFNApRGiTuJSIzVjssmn196Yt7wPuWnfMx6ePHp5bqt7TAb38Ld9zh2wJBfOEF7+M+sv9u7ia9hN242MOM/9eDuTBLDerAtx7En3/72wPj0QPBD3Khb96cWjTV0uI/z+jRfqJz/Xq/7YUX4Iwz/GTvvHmwerX/TLGYvwZf/aqPEgp8+h0dhRUpEUIMHYl7CciM1V6/Hs45xwtga6uPeAlPloYjYzZs8ELe1gZnn52+InPjRvja12DFChi9aQlb3H5p5z2RudwRO5H2dri0O7t9mbH0P/mJbw+ibaYk1xWHwxoDgj5Ll/qb1SGHwD33+G3Bc3BjCvbbe2//S2X06PTJ0EKKlAghSoPEfQgE7otXXkmP1Q68zuBH2zfdlPs4zqUiT559Nn3bu0+/yAY+mNb2zdjVbJw0hWPGwv4RC4Yy6egYKNhhtmzxK0zDK2MDYrFUeGI49DJz//B+y5d791EQzhgOsSxk1a4QYuhI3AdJOIwwFkv5puNxGD4cXnqp+GP+8pep0f+OrGENO6Vtv4zv8F0uI25wyYj0DI9R9gXL/qdOjRZtSLlexoyBBx5I3aRiMfjnf/b+/yDzZBRm/jNnir5zA1ebDnaxlBCieCTugyTsYtiyJSVy11wDDz6YXdxz5YXZsgXewzrW8d609lv5PDdPuJV58yC+JXfx58Bvfv31qYRdUcIciHpw3iuugA9/OFXKr7/fpxNoacm+wOrjH4cvftFPvF522cDt4bS8AZowrQzZ1ieI5kHiXiThEXFbW8pHHbgsrrvOR4hEEYvBKadEu2libgv/zw2jjdTKoKWM4RMsYdw444Hf+HNfdpkfSff0eAEfP95HrYwd6/3i118/MPFYODdL2LUSvsls3jywRqtzqRIZwwpFAAAOhklEQVR8wXGC1bRtbXDttV44ZswYuMq2tXVgFkhRGQpZnCYaH4l7EWT+01x5pRfUcHRJZlGJMLEYbLNNuhDGzLHMfYzR7o9b+62PDWNb3mZTf5zWVp8vJuB3v0svfpGZDjeTsP8/Hodjj/UTuNl+PYQJClWHI39g4IgwWGUbpAgYUItVVBRNXAuQuBdF+J9m/Xo/An/Pe7xPe9kyuPfe3KIZFtn+fpjLiZzofpPW532xd+lvH8Y1SUHt6EiPD88MqcxGVL6azZv9KD+bqyZMW1tukQ5sCtws+ao1yUVQOQpNNy0aG4l7DgL/NXi3xyuvpLY5533r4EMCTzstv2jG4/44MzZN4zwuT9t25f/9C9NmdHj//XqYP98L8cUXp+LfP/3p/LncAywqlyew7bbZtwU2nnWWtzOqwEi2n/zZfOlyEVQeTVwLQOkHoli40C+1z1VsOuoxZkzu7d+wqwY07sGLW/PDhEvF5crXUoxNhe6/776pPDW50hIUW/S7FEXChRApKDD9QKzaN5daI5GAww7zudMLdYEELFsW3X4ic3EYV7n/s7VtLEswHCvjIwG/knPMmPzncM6PrgdLtsiXQw9NTZBG+WwDgp/88XhhP/mL7S+EKA1yy2TQ2+snKkvBwTzMwxyS1nYUd/PaqKP48IdhJN790tOTXXQzcQ7OOw+eey41MZrpqjHzYYrZbjaZtLenCoJAbp9tsT/5691FoPkCUa+YK8SBWwY6OzvdokWLqnLuKIJ/4ltvLVwUs7EPy1nOqLS2iczhBlIKGo/D7rsPbrFTS4sX8GBVazyeKk4di3nx/4//yH2TMvPhitkmTSVqmi8QtYmZLXbOdebrp5E76Ym1hnKv25VVrCK9APVF/BszuGhA3y1bBifsMNBd1N/vJ0FHjIhOVLbbbtDZCXfemYpX/9SnYPr07GKlxUYKKRT1jcQd74pZt27w+2/DWtayXVpbD2dx8S49/k1EibxSEqTXDacjCLtVbr3Vt919d6otl7ALj0IKRT3T9G6Znh6YPHlwI/ZWNrKR9ALU93M4R3I/bW3ebVKpyztsWLrbIMqtIldL8eiaiVqjULdMU4t7IuGTYxU6mZnC8RrD+QCpAtQvM4KRvATkCCIvI/E4XHJJcUWuhRD1R6Hi3tShkBdcULyw/57DcMTShL2NDYzkZcot7Hvtlf5+zBgf6VLqMMNEwueLSSRKczwhROVpWp/7d7+bWmFaCL/ga3yN69LatmEt77BNiS2LprXV50d/8kmfe/2kk7yPvdRuA0WICNEYNI24JxJ+pL50qfeDv/NOYft9j3/lX/l+WtuurOJ1di2DlQNpafHVmIJwxa6u9InTUke1KEJEiMagKcQ9kfDl4fIlywozkTnM4ctpbfuwnGfJUqi0RAQLkjJFvVJkRoh0dHgXjSYUhagvGlrcg/znixYVLuxHMbAA9cE8zEIOLoOFKcx8yoPRo6sbnRFeURpUcZKLRoj6o2HFvdgQx7EsYQkDC1D/hhNLatdpp8Ftt3nBBD+h65z3qY8eXZybpVxheoENM2bIRSNEvdKQ4t7TA2efXVjfkbzIixkFqKdwNT9jSkltes97fEqA8CToK6/4wtNBqb5ixLMSE59axCNE/dJw4l6osEcVoP4x3+VCfpxlj+LITOa1caMfmUNqZJxI+AiYKPHMNyqvxMRnvSf9EqKZaShxTyTyC/sw3uVd/iGt7VY+zxe5tWR2jBsHDz880CWUKcDZxDMYla9f728S06bBpZemH6tSo2rlmBGiPmmIRUyJBHz2s/DJT2bvE2MLG2hLE/aljMHoL6mwm8Ejj3gfelDxyMxHvzz2GJxzTvrioK4uv6o0LKB9fanC2/39flK4pyf9PF1dvrbpfvvB0UcXZpsWJwnRPNR9+oH8KQQcf+BjjCZVgPr/8V62ZS39DKHqRQZhN0xQqm7ECB9xsnQpXHddKkVvW1u0GyVwxXR0+JtA+DMddZRP/BXu292dmphtb4cFC7KPsgfjo1deFSFqj6ZI+ZtI5B6tz+VETiS9APUw3mU9wwZ9zvZknrANG1Ij8m99C9auhdmzvQ+8rS09Pn3GjPQUvJs2DRT3TPE95RRfgDvgpJPSxbavL3WzgPx+997e1K+BbH3DxwetVBWinqlbcc8l7D9hGtMyClB38BfeomPI5w0XwDjkEBg1CiZM8MI3dmwqNUBYCAP/eLBvPO4jZRKJVL/MCdKPfARmzUodb/TodLG98krv+glG7rn87omEv/EEvyxaWgb2zby5nHGGwiCFqGsKKbQKHAM8C6wALojY3g7cktz+KDAy3zGHUiA7W/HnY5gXWYB6KAWlC3m0tjo3YYIvcB1VVNq5VNHtCROca28f2C9XUWrnogtNB8cMCltnI7yvme+fq0887vvkskcIUR0osEB2IcIeB/4EfBBoA54ARmX0+TowM/n6ZOCWfMcdrLhHieuBJAY0jmFJ2UU92yMQ3yiiRDpg4cKUaGeST/xzUci+UX1y2SOEqA6FinshbpkDgBXOuRcAzOxXwAnA06E+JwDTk69/DVxjZpY0pGRYRkbdvXmGZ9g3re1jPMGTfKyUp007f75PZJbbRZKv+HSusneDjTkvZN9sfeSKEaI+yRstY2afA45xzn0t+f504EDn3JRQnz8m+6xMvv9Tss9fMo41CZgEMGLEiP1efvnl4oxNivtwVrKS3dO2HUofD3JoUcfLRTzuwwy7u+Hqq9N93fPnw+23p/ePxbwP/Mwz8yf7UhSKEGKwlDJaJqoCReYdoZA+OOd6gB7woZAFnHsAe/ASL7Hn1vef5TZu57ODORQTJsD48T5UEfyEaPA6LNATJqSL8aRJPu78uuvgAx/wx1izpnCx1sIgIUS5KUTcV0LaMHk3YFWWPivNrAXYDnirJBaGcA46bBv+l08yhzP4BZPStm+3Hey9txfZ7bf3z0FxizFjfLji66/DLrsUl0o3SownTUrPqy6EELVEIW6ZFuA54AjgNeBx4FTn3FOhPucCo51zk83sZOBE59wXch23FmqoCiFEvVEyt4xzbrOZTQHuxkfOzHbOPWVmP8TP2t4JXAfcYGYr8CP2k4dmvhBCiKFQ0CIm59w8YF5G2w9Cr9cDny+taUIIIQZLQyQOE0IIkY7EXQghGhCJuxBCNCASdyGEaEAk7kII0YBI3IUQogGpWiUmM3sTKC65TIqdgL/k7VVdZGNpkI2lQTaWhlqwcQ/n3M75OlVN3IeCmS0qZIVWNZGNpUE2lgbZWBrqwcYAuWWEEKIBkbgLIUQDUq/i3lNtAwpANpYG2VgaZGNpqAcbgTr1uQshhMhNvY7chRBC5EDiLoQQDUjdibuZHWNmz5rZCjO7oEo27G5mC8xsuZk9ZWbfTLZPN7PXzGxZ8nFsaJ8LkzY/a2ZHV9DWl8zsyaQ9i5JtO5rZvWb2fPJ5h2S7mdlVSTv/YGafKLNte4eu1TIzW2tmU2vhOprZbDN7I1kfOGgr+rqZ2RnJ/s+b2RkVsPEnZvZM0o7fmNn2yfaRZrYudE1nhvbZL/k3siL5OaLKZpbSxqK/33L+32ex8ZaQfS+Z2bJke1Wu46BwztXNA18s5E/AB4E24AlgVBXs2BX4RPL1NvhKVaOA6cC0iP6jkra2A3smP0O8Qra+BOyU0XYZcEHy9QXApcnXxwLz8TVxDwIerfB3+zqwRy1cR2Ac8Angj4O9bsCOwAvJ5x2Sr3cos41HAS3J15eGbBwZ7pdxnMeArqT984HxZbaxqO+33P/3UTZmbL8c+EE1r+NgHvU2cj8AWOGce8E5txH4FXBCpY1wzq12zi1Jvn4bWA4Mz7HLCcCvnHMbnHMvAivwn6VanADMSb6eA0wItfc6zyPA9ma2a4VsOgL4k3Mu16rlil1H59yDDKwDXOx1Oxq41zn3lnPur8C9wDHltNE5d49zbnPy7SP4msdZSdq5rXMu4bxC9YY+V1lszEG277es//e5bEyOvr8A3JzrGOW+joOh3sR9OPBq6P1Kcotq2TGzkcBY4NFk05TkT+LZwc92qmu3A+4xs8VmFpT0/kfn3GrwNyrg/TVg58mk/wPV2nWE4q9bte39Cn4EGbCnmS01swfM7JBk2/CkXQGVsrGY77ea1/EQ4M/OuedDbbV0HbNSb+Ie5cOqWiynmb0PmAtMdc6tBa4F/gkYA6zG/5yD6tp9sHPuE8B44FwzG5ejb1XsNLM24Hjgv5NNtXgdc5HNrqrZa2bfAzYDNyWbVgMjnHNjgW8D/2Vm21bJxmK/32p+76eQPuiopeuYk3oT95XA7qH3uwGrqmGImbXihf0m59xtAM65Pzvntjjn+oFfkHIZVM1u59yq5PMbwG+SNv05cLckn9+osp3jgSXOuT8nba2565ik2OtWFXuTE7efAU5LughIujrWJF8vxvuwP5y0Mey6KbuNg/h+q3UdW4ATgVuCtlq6jvmoN3F/HNjLzPZMjvZOBu6stBFJP9x1wHLn3BWh9rB/+rNAMPt+J3CymbWb2Z7AXvjJl3Lb+Q9mtk3wGj/Z9sekPUHkxhnAHSE7JyajPw4C/h64IcpM2uio1q5jiGKv293AUWa2Q9L1cFSyrWyY2THAd4HjnXPvhtp3NrN48vUH8dfuhaSdb5vZQcm/64mhz1UuG4v9fqv1f38k8Ixzbqu7pZauY16qOZs7mAc+MuE5/B3ze1Wy4Z/xP7n+ACxLPo4FbgCeTLbfCewa2ud7SZufpUKz6PjogieSj6eC6wV0APcDzyefd0y2G/CzpJ1PAp0VsPG9wBpgu1Bb1a8j/mazGtiEH5V9dTDXDe/3XpF8nFkBG1fg/dPB3+XMZN+Tkn8DTwBLgONCx+nEC+yfgGtIrlwvo41Ff7/l/L+PsjHZ/p/A5Iy+VbmOg3ko/YAQQjQg9eaWEUIIUQASdyGEaEAk7kII0YBI3IUQogGRuAshRAMicRdCiAZE4i6EEA3I/wcMzt5UYlYaGQAAAABJRU5ErkJggg==
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><b>R-squared</b> is a statistical measure of how close the data are to the fitted regression line. It is also known as the coefficient of determination, or the coefficient of multiple determination for multiple regression. <a href="http://blog.minitab.com/blog/adventures-in-statistics-2/regression-analysis-how-do-i-interpret-r-squared-and-assess-the-goodness-of-fit">Read more</a> 
<br><br>
Most of the time if R-squared score is greater than 60% then it is good enough to use the model. In general, the higher the R-squared, the better the model fits your data. <br><br>Let's check out this model whether it is good or bad with R-squared.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[35]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">reg</span><span class="o">.</span><span class="n">score</span><span class="p">(</span><span class="n">X_test</span><span class="p">,</span> <span class="n">y_test</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[35]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0.835688539457739</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>It turns out that this r-squared score is very good. Most of the time, we can use this model to predict the new and unseen input. <br>16% indicates that the model explains none of the variability of the response data around its mean.
<br>84% indicates that the model explains all the variability of the response data around its mean.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><b>Fit a multiple linear regression model for Purchase using Occupation and Age</b>
<br><br>
Since most of the variables in the dataset are categorical, it is necessary to convert these qualitative (characteristic) values to quantitative (numerical) values.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Occupations in the dataset are already represented as numbers so we just need to assign each age group a numeric value. From the 
Exploratory Data Analysis, we know the rank of the purchase power of each group, which is a numeric representation of each age group and can be used for the linear regression model.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[36]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">numeric</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="p">[[</span><span class="s1">&#39;Age&#39;</span><span class="p">,</span> <span class="s1">&#39;Occupation&#39;</span><span class="p">,</span> <span class="s1">&#39;Purchase&#39;</span><span class="p">,</span> <span class="s1">&#39;Stay_In_Current_City_Years&#39;</span><span class="p">,</span> <span class="s1">&#39;Marital_Status&#39;</span><span class="p">]]</span>
<span class="n">numeric</span> <span class="o">=</span> <span class="n">numeric</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[37]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Assign each age group a numeric value based on the rank of the amount of purchase</span>
<span class="c1">#     1 is assigned to Age group 26-35</span>
<span class="c1">#     2 is assigned to Age group 36-45</span>
<span class="c1">#     3 is assigned to Age group 18-25</span>
<span class="c1">#     4 is assigned to Age group 46-50</span>
<span class="c1">#     5 is assigned to Age group 51-55</span>
<span class="c1">#     6 is assigned to Age group 55+</span>
<span class="c1">#     7 is assigned to Age group 0-17 </span>

<span class="k">for</span> <span class="n">index</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">numeric</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
    <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;26-35&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">1</span>
    <span class="k">elif</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;36-45&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">2</span>
    <span class="k">elif</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;18-25&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">3</span>
    <span class="k">elif</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;46-50&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">4</span>
    <span class="k">elif</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;51-55&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">5</span>
    <span class="k">elif</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;55+&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">6</span>
    <span class="k">elif</span> <span class="n">row</span><span class="p">[</span><span class="s1">&#39;Age&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;0-17&#39;</span><span class="p">:</span>
        <span class="n">numeric</span><span class="o">.</span><span class="n">at</span><span class="p">[</span><span class="n">index</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">7</span>
<span class="n">numeric</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[37]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Age</th>
      <th>Occupation</th>
      <th>Purchase</th>
      <th>Stay_In_Current_City_Years</th>
      <th>Marital_Status</th>
      <th>rank</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0-17</td>
      <td>10</td>
      <td>8370</td>
      <td>2</td>
      <td>0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>0-17</td>
      <td>10</td>
      <td>15200</td>
      <td>2</td>
      <td>0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>0-17</td>
      <td>10</td>
      <td>1422</td>
      <td>2</td>
      <td>0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>0-17</td>
      <td>10</td>
      <td>1057</td>
      <td>2</td>
      <td>0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>55+</td>
      <td>16</td>
      <td>7969</td>
      <td>4</td>
      <td>0</td>
      <td>6.0</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[38]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X</span> <span class="o">=</span> <span class="n">numeric</span><span class="p">[[</span><span class="s1">&#39;Occupation&#39;</span><span class="p">,</span> <span class="s1">&#39;rank&#39;</span><span class="p">]]</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">numeric</span><span class="o">.</span><span class="n">Purchase</span>
<span class="n">reg</span> <span class="o">=</span> <span class="n">linear_model</span><span class="o">.</span><span class="n">LinearRegression</span><span class="p">()</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">y</span><span class="p">)</span>
<span class="n">X</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[38]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Occupation</th>
      <th>rank</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>10</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>10</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>10</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>10</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>16</td>
      <td>6.0</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[39]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">est1</span> <span class="o">=</span> <span class="n">sm</span><span class="o">.</span><span class="n">OLS</span><span class="p">(</span><span class="n">y</span><span class="p">,</span> <span class="n">X</span><span class="p">)</span><span class="o">.</span><span class="n">fit</span><span class="p">()</span>
<span class="nb">print</span><span class="p">(</span><span class="n">est1</span><span class="o">.</span><span class="n">summary</span><span class="p">())</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>                            OLS Regression Results                            
==============================================================================
Dep. Variable:               Purchase   R-squared:                       0.617
Model:                            OLS   Adj. R-squared:                  0.617
Method:                 Least Squares   F-statistic:                 4.330e+05
Date:                Sat, 15 Dec 2018   Prob (F-statistic):               0.00
Time:                        00:12:32   Log-Likelihood:            -5.4864e+06
No. Observations:              537577   AIC:                         1.097e+07
Df Residuals:                  537575   BIC:                         1.097e+07
Df Model:                           2                                         
Covariance Type:            nonrobust                                         
==============================================================================
                 coef    std err          t      P&gt;|t|      [0.025      0.975]
------------------------------------------------------------------------------
Occupation   373.7333      1.145    326.332      0.000     371.489     375.978
rank        1774.2126      4.045    438.614      0.000    1766.284    1782.141
==============================================================================
Omnibus:                     2780.401   Durbin-Watson:                   1.059
Prob(Omnibus):                  0.000   Jarque-Bera (JB):             2740.387
Skew:                           0.160   Prob(JB):                         0.00
Kurtosis:                       2.860   Cond. No.                         4.88
==============================================================================

Warnings:
[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The R-square indicates that: <br></p>
<p>38.3% indicates that the model explains none of the variability of the response data around its mean.
<br>61.7% indicates that the model explains all the variability of the response data around its mean.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Logistic-Regression-"><section id="10">Logistic Regression </section><a class="anchor-link" href="#Logistic-Regression-">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><b>Classify Gender Given Occupation</b></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>There is a challenge in our dataset which is imbalance between the number of male and female. The number of observations for female are only one third over male. Standard classifier algorithms like Logistic Regression has a bias towards classes which have number of instances. The tend to only predict the majority class. The features of minority are treated as noise and are often ignored. Thus there is a high probability of misclassification of the minority class as compared to the majority class.
<br><br>
There are several approaches to handle imbalance datasets: 
<br></p>
<p><ul>
    <li>Random Resampling</li>
    <li>Cluster-Based Over Sampling</li>
    <li>Informed Over Sampling: Synthetic Minority Over-sampling Technique</li>
    <li>Modified synthetic minority oversampling technique</li>
</ul>
<br>
In our case, I would like to try out the Random Resampling Approach.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[40]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">purchase_by_user</span> <span class="o">=</span> <span class="n">blackfriday</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;User_ID&#39;</span><span class="p">,</span> <span class="s1">&#39;Gender&#39;</span><span class="p">,</span> <span class="s1">&#39;Occupation&#39;</span><span class="p">,</span> <span class="s1">&#39;Mean_age&#39;</span><span class="p">,</span> <span class="s1">&#39;Marital_Status&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">agg</span><span class="p">({</span><span class="s1">&#39;Purchase&#39;</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">})</span>
<span class="n">purchase_by_user</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">purchase_by_user</span><span class="o">.</span><span class="n">Gender</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="o">.</span><span class="n">Gender</span><span class="o">.</span><span class="n">map</span><span class="p">({</span><span class="s1">&#39;F&#39;</span><span class="p">:</span><span class="mi">0</span><span class="p">,</span> <span class="s1">&#39;M&#39;</span><span class="p">:</span> <span class="mi">1</span><span class="p">})</span>
<span class="n">purchase_by_user</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[40]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>User_ID</th>
      <th>Gender</th>
      <th>Occupation</th>
      <th>Mean_age</th>
      <th>Marital_Status</th>
      <th>Purchase</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1000001</td>
      <td>0</td>
      <td>10</td>
      <td>8.5</td>
      <td>0</td>
      <td>333481</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1000002</td>
      <td>1</td>
      <td>16</td>
      <td>67.5</td>
      <td>0</td>
      <td>810353</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1000003</td>
      <td>1</td>
      <td>15</td>
      <td>30.5</td>
      <td>0</td>
      <td>341635</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1000004</td>
      <td>1</td>
      <td>7</td>
      <td>48.0</td>
      <td>1</td>
      <td>205987</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1000005</td>
      <td>1</td>
      <td>20</td>
      <td>30.5</td>
      <td>1</td>
      <td>821001</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[41]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">male</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="p">[</span><span class="n">purchase_by_user</span><span class="o">.</span><span class="n">Gender</span><span class="o">==</span><span class="mi">1</span><span class="p">]</span> <span class="c1"># Get all male </span>
<span class="n">female</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="p">[</span><span class="n">purchase_by_user</span><span class="o">.</span><span class="n">Gender</span><span class="o">==</span><span class="mi">0</span><span class="p">]</span> <span class="c1"># Get all female</span>
<span class="n">male</span> <span class="o">=</span> <span class="n">male</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="nb">int</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">male</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span><span class="p">))</span> <span class="c1"># only need half of the male population</span>
<span class="n">new_df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">concat</span><span class="p">([</span><span class="n">male</span><span class="p">,</span> <span class="n">female</span><span class="p">,</span> <span class="n">female</span><span class="p">])</span> <span class="c1"># double the number of female population</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[42]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X</span> <span class="o">=</span> <span class="n">new_df</span><span class="p">[[</span><span class="s1">&#39;Occupation&#39;</span><span class="p">]]</span><span class="o">.</span><span class="n">values</span><span class="o">.</span><span class="n">reshape</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span><span class="mi">1</span><span class="p">)</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">new_df</span><span class="p">[</span><span class="s1">&#39;Gender&#39;</span><span class="p">]</span> <span class="c1">#1 as Male, 0 as Female</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[43]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X_train</span><span class="p">,</span> <span class="n">X_test</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="n">y_test</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">test_size</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">log_reg</span> <span class="o">=</span> <span class="n">linear_model</span><span class="o">.</span><span class="n">LogisticRegression</span><span class="p">()</span>
<span class="n">log_reg</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span><span class="n">y_train</span><span class="p">)</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">log_reg</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Accuracy of logistic regression classifier on test set: </span><span class="si">{:.2f}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">log_reg</span><span class="o">.</span><span class="n">score</span><span class="p">(</span><span class="n">X_test</span><span class="p">,</span> <span class="n">y_test</span><span class="p">)))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Accuracy of logistic regression classifier on test set: 0.64
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Compute-precision,-recall,-F-measure-and-support">Compute precision, recall, F-measure and support<a class="anchor-link" href="#Compute-precision,-recall,-F-measure-and-support">&#182;</a></h3><p><br> Precision-Recall is a useful measure of success of prediction when the classes are very imbalanced. In information retrieval, precision is a measure of result relevancy, while recall is a measure of how many truly relevant results are returned.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[44]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">classification_report</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>             precision    recall  f1-score   support

          0       0.64      0.93      0.76      1003
          1       0.62      0.18      0.28       631

avg / total       0.64      0.64      0.58      1634

</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Precision: 64% female and 62% male selected instances are relevant.
<br> Recall: 93% female and only 18% male relevant instances are selected.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, let's try Bagging Classifier to see if the result is better than Logistic Regression</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[45]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">sklearn.ensemble</span> <span class="k">import</span> <span class="n">BaggingClassifier</span>
<span class="kn">from</span> <span class="nn">sklearn.tree</span> <span class="k">import</span> <span class="n">DecisionTreeClassifier</span>

<span class="n">bag_clf</span> <span class="o">=</span> <span class="n">BaggingClassifier</span><span class="p">(</span><span class="n">DecisionTreeClassifier</span><span class="p">(),</span> <span class="n">n_estimators</span><span class="o">=</span><span class="mi">1000</span><span class="p">,</span> <span class="n">max_samples</span><span class="o">=</span><span class="mf">0.8</span><span class="p">,</span> <span class="n">bootstrap</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">n_jobs</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">oob_score</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">bag_clf</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">)</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">bag_clf</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
<span class="n">bag_clf</span><span class="o">.</span><span class="n">oob_score_</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[45]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0.6590551181102362</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>According to this oob evaluation, this BaggingClassifier is likely to achieve about 65.9% accuracy on the test set. Let's verify this:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[46]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">accuracy_score</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[46]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0.6542227662178702</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>We get 65.4% accuracy on the test set. It is close enough.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Compute-precision,-recall,-F-measure-and-support">Compute precision, recall, F-measure and support<a class="anchor-link" href="#Compute-precision,-recall,-F-measure-and-support">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[47]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">classification_report</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>             precision    recall  f1-score   support

          0       0.66      0.89      0.76      1003
          1       0.61      0.28      0.39       631

avg / total       0.64      0.65      0.61      1634

</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>As we can see, the result is a little bit better than Logistic Regression. But there is a tradeoff when we use BaggingClassifier. The precision in female increases but the recall decreases. With male, the precision decreases while the recall increases. 
<br>
<br>Precision: 66% female and 61% male selected instances are relevant. 
<br>Recall: 89% female and only 28% male relevant instances are selected.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><b>Classify Marrital Status Given Mean Age</b></p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[48]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="p">[[</span><span class="s1">&#39;Mean_age&#39;</span><span class="p">]]</span><span class="o">.</span><span class="n">values</span><span class="o">.</span><span class="n">reshape</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span><span class="mi">1</span><span class="p">)</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">purchase_by_user</span><span class="p">[</span><span class="s1">&#39;Marital_Status&#39;</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[49]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X_train</span><span class="p">,</span> <span class="n">X_test</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="n">y_test</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">test_size</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">log_reg</span> <span class="o">=</span> <span class="n">linear_model</span><span class="o">.</span><span class="n">LogisticRegression</span><span class="p">()</span>
<span class="n">log_reg</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span><span class="n">y_train</span><span class="p">)</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">log_reg</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Accuracy of logistic regression classifier on test set: </span><span class="si">{:.2f}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">log_reg</span><span class="o">.</span><span class="n">score</span><span class="p">(</span><span class="n">X_test</span><span class="p">,</span> <span class="n">y_test</span><span class="p">)))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Accuracy of logistic regression classifier on test set: 0.67
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Compute-precision,-recall,-F-measure-and-support">Compute precision, recall, F-measure and support<a class="anchor-link" href="#Compute-precision,-recall,-F-measure-and-support">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[50]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">classification_report</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>             precision    recall  f1-score   support

          0       0.67      0.87      0.76      1032
          1       0.68      0.39      0.50       736

avg / total       0.67      0.67      0.65      1768

</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, let's try Bagging Classifier to see if the result is better than Logistic Regression</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[51]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">bag_clf</span> <span class="o">=</span> <span class="n">BaggingClassifier</span><span class="p">(</span><span class="n">DecisionTreeClassifier</span><span class="p">(),</span> <span class="n">n_estimators</span><span class="o">=</span><span class="mi">1000</span><span class="p">,</span> <span class="n">max_samples</span><span class="o">=</span><span class="mf">0.8</span><span class="p">,</span> <span class="n">bootstrap</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">n_jobs</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">oob_score</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">bag_clf</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">)</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">bag_clf</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>
<span class="n">bag_clf</span><span class="o">.</span><span class="n">oob_score_</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[51]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0.670870725200097</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>According to this oob evaluation, this BaggingClassifier is likely to achieve about 67.1% accuracy on the test set. Let's verify this:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[52]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">accuracy_score</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[52]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0.6702488687782805</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>We get 67.0% accuracy on the test set. It is close enough.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Compute-precision,-recall,-F-measure-and-support">Compute precision, recall, F-measure and support<a class="anchor-link" href="#Compute-precision,-recall,-F-measure-and-support">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[53]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">classification_report</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>             precision    recall  f1-score   support

          0       0.67      0.87      0.76      1032
          1       0.68      0.39      0.50       736

avg / total       0.67      0.67      0.65      1768

</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Conclusion"><section id="conclusion">Conclusion</section><a class="anchor-link" href="#Conclusion">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Black Friday is the biggest day of shopping in the year. The goal of our project was to take the dataset of Black Friday sales and use the techniques we learned throughout the semester to extract data that will help advertisers and retailers make the most of it. Using Exploratory data analysis, and regression  we saw  how attributes such as age, gender, marital status, and more affect the way one should expect people to shop that day. The result of this project will help retailers advertise to the right target groups for their products, leading to more happy purchases, resulting in a happier holiday season!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><img src="happy.jpg" width="900" height="600"/></p>

</div>
</div>
</div>
    </div>
  </div>
</body>

 


</html>
