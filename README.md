<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<title>dog_app</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
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
<h1 id="Artificial-Intelligence-Nanodegree">Artificial Intelligence Nanodegree<a class="anchor-link" href="#Artificial-Intelligence-Nanodegree">&#182;</a></h1><h2 id="Convolutional-Neural-Networks">Convolutional Neural Networks<a class="anchor-link" href="#Convolutional-Neural-Networks">&#182;</a></h2><h2 id="Project:-Write-an-Algorithm-for-a-Dog-Identification-App">Project: Write an Algorithm for a Dog Identification App<a class="anchor-link" href="#Project:-Write-an-Algorithm-for-a-Dog-Identification-App">&#182;</a></h2><hr>
<p>In this notebook, some template code has already been provided for you, and you will need to implement additional functionality to successfully complete this project. You will not need to modify the included code beyond what is requested. Sections that begin with <strong>'(IMPLEMENTATION)'</strong> in the header indicate that the following block of code will require additional functionality which you must provide. Instructions will be provided for each section, and the specifics of the implementation are marked in the code block with a 'TODO' statement. Please be sure to read the instructions carefully!</p>
<blockquote><p><strong>Note</strong>: Once you have completed all of the code implementations, you need to finalize your work by exporting the iPython Notebook as an HTML document. Before exporting the notebook to html, all of the code cells need to have been run so that reviewers can see the final implementation and output. You can then export the notebook by using the menu above and navigating to  \n",
    "<strong>File -&gt; Download as -&gt; HTML (.html)</strong>. Include the finished document along with this notebook as your submission.</p>
</blockquote>
<p>In addition to implementing code, there will be questions that you must answer which relate to the project and your implementation. Each section where you will answer a question is preceded by a <strong>'Question X'</strong> header. Carefully read each question and provide thorough answers in the following text boxes that begin with <strong>'Answer:'</strong>. Your project submission will be evaluated based on your answers to each of the questions and the implementation you provide.</p>
<blockquote><p><strong>Note:</strong> Code and Markdown cells can be executed using the <strong>Shift + Enter</strong> keyboard shortcut.  Markdown cells can be edited by double-clicking the cell to enter edit mode.</p>
</blockquote>
<p>The rubric contains <em>optional</em> "Stand Out Suggestions" for enhancing the project beyond the minimum requirements. If you decide to pursue the "Stand Out Suggestions", you should include the code in this IPython notebook.</p>
<hr>
<h3 id="Why-We're-Here">Why We're Here<a class="anchor-link" href="#Why-We're-Here">&#182;</a></h3><p>In this notebook, you will make the first steps towards developing an algorithm that could be used as part of a mobile or web app.  At the end of this project, your code will accept any user-supplied image as input.  If a dog is detected in the image, it will provide an estimate of the dog's breed.  If a human is detected, it will provide an estimate of the dog breed that is most resembling.  The image below displays potential sample output of your finished project (... but we expect that each student's algorithm will behave differently!).</p>
<p><img src="images/sample_dog_output.png" alt="Sample Dog Output"></p>
<p>In this real-world setting, you will need to piece together a series of models to perform different tasks; for instance, the algorithm that detects humans in an image will be different from the CNN that infers dog breed.  There are many points of possible failure, and no perfect algorithm exists.  Your imperfect solution will nonetheless create a fun user experience!</p>
<h3 id="The-Road-Ahead">The Road Ahead<a class="anchor-link" href="#The-Road-Ahead">&#182;</a></h3><p>We break the notebook into separate steps.  Feel free to use the links below to navigate the notebook.</p>
<ul>
<li><a href="#step0">Step 0</a>: Import Datasets</li>
<li><a href="#step1">Step 1</a>: Detect Humans</li>
<li><a href="#step2">Step 2</a>: Detect Dogs</li>
<li><a href="#step3">Step 3</a>: Create a CNN to Classify Dog Breeds (from Scratch)</li>
<li><a href="#step4">Step 4</a>: Use a CNN to Classify Dog Breeds (using Transfer Learning)</li>
<li><a href="#step5">Step 5</a>: Create a CNN to Classify Dog Breeds (using Transfer Learning)</li>
<li><a href="#step6">Step 6</a>: Write your Algorithm</li>
<li><a href="#step7">Step 7</a>: Test Your Algorithm</li>
</ul>
<hr>
<p><a id='step0'></a></p>
<h2 id="Step-0:-Import-Datasets">Step 0: Import Datasets<a class="anchor-link" href="#Step-0:-Import-Datasets">&#182;</a></h2><h3 id="Import-Dog-Dataset">Import Dog Dataset<a class="anchor-link" href="#Import-Dog-Dataset">&#182;</a></h3><p>In the code cell below, we import a dataset of dog images.  We populate a few variables through the use of the <code>load_files</code> function from the scikit-learn library:</p>
<ul>
<li><code>train_files</code>, <code>valid_files</code>, <code>test_files</code> - numpy arrays containing file paths to images</li>
<li><code>train_targets</code>, <code>valid_targets</code>, <code>test_targets</code> - numpy arrays containing onehot-encoded classification labels </li>
<li><code>dog_names</code> - list of string-valued dog breed names for translating labels</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[15]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">sklearn.datasets</span> <span class="k">import</span> <span class="n">load_files</span>       
<span class="kn">from</span> <span class="nn">keras.utils</span> <span class="k">import</span> <span class="n">np_utils</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">from</span> <span class="nn">glob</span> <span class="k">import</span> <span class="n">glob</span>

<span class="c1"># define function to load train, test, and validation datasets</span>
<span class="k">def</span> <span class="nf">load_dataset</span><span class="p">(</span><span class="n">path</span><span class="p">):</span>
    <span class="n">data</span> <span class="o">=</span> <span class="n">load_files</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
    <span class="n">dog_files</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s1">&#39;filenames&#39;</span><span class="p">])</span>
    <span class="n">dog_targets</span> <span class="o">=</span> <span class="n">np_utils</span><span class="o">.</span><span class="n">to_categorical</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s1">&#39;target&#39;</span><span class="p">]),</span> <span class="mi">133</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">dog_files</span><span class="p">,</span> <span class="n">dog_targets</span>

<span class="c1"># load train, test, and validation datasets</span>
<span class="n">train_files</span><span class="p">,</span> <span class="n">train_targets</span> <span class="o">=</span> <span class="n">load_dataset</span><span class="p">(</span><span class="s1">&#39;/data/dog_images/train&#39;</span><span class="p">)</span>
<span class="n">valid_files</span><span class="p">,</span> <span class="n">valid_targets</span> <span class="o">=</span> <span class="n">load_dataset</span><span class="p">(</span><span class="s1">&#39;/data/dog_images/valid&#39;</span><span class="p">)</span>
<span class="n">test_files</span><span class="p">,</span> <span class="n">test_targets</span> <span class="o">=</span> <span class="n">load_dataset</span><span class="p">(</span><span class="s1">&#39;/data/dog_images/test&#39;</span><span class="p">)</span>

<span class="c1"># load list of dog names</span>
<span class="n">dog_names</span> <span class="o">=</span> <span class="p">[</span><span class="n">item</span><span class="p">[</span><span class="mi">20</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="k">for</span> <span class="n">item</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;/data/dog_images/train/*/&quot;</span><span class="p">))]</span>

<span class="c1"># print statistics about the dataset</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;There are </span><span class="si">%d</span><span class="s1"> total dog categories.&#39;</span> <span class="o">%</span> <span class="nb">len</span><span class="p">(</span><span class="n">dog_names</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;There are </span><span class="si">%s</span><span class="s1"> total dog images.</span><span class="se">\n</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="nb">len</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">hstack</span><span class="p">([</span><span class="n">train_files</span><span class="p">,</span> <span class="n">valid_files</span><span class="p">,</span> <span class="n">test_files</span><span class="p">])))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;There are </span><span class="si">%d</span><span class="s1"> training dog images.&#39;</span> <span class="o">%</span> <span class="nb">len</span><span class="p">(</span><span class="n">train_files</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;There are </span><span class="si">%d</span><span class="s1"> validation dog images.&#39;</span> <span class="o">%</span> <span class="nb">len</span><span class="p">(</span><span class="n">valid_files</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;There are </span><span class="si">%d</span><span class="s1"> test dog images.&#39;</span><span class="o">%</span> <span class="nb">len</span><span class="p">(</span><span class="n">test_files</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>There are 133 total dog categories.
There are 8351 total dog images.

There are 6680 training dog images.
There are 835 validation dog images.
There are 836 test dog images.
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
<h3 id="Import-Human-Dataset">Import Human Dataset<a class="anchor-link" href="#Import-Human-Dataset">&#182;</a></h3><p>In the code cell below, we import a dataset of human images, where the file paths are stored in the numpy array <code>human_files</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[16]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">random</span>
<span class="n">random</span><span class="o">.</span><span class="n">seed</span><span class="p">(</span><span class="mi">8675309</span><span class="p">)</span>

<span class="c1"># load filenames in shuffled human dataset</span>
<span class="n">human_files</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;/data/lfw/*/*&quot;</span><span class="p">))</span>
<span class="n">random</span><span class="o">.</span><span class="n">shuffle</span><span class="p">(</span><span class="n">human_files</span><span class="p">)</span>

<span class="c1"># print statistics about the dataset</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;There are </span><span class="si">%d</span><span class="s1"> total human images.&#39;</span> <span class="o">%</span> <span class="nb">len</span><span class="p">(</span><span class="n">human_files</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>There are 13233 total human images.
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
<hr>
<p><a id='step1'></a></p>
<h2 id="Step-1:-Detect-Humans">Step 1: Detect Humans<a class="anchor-link" href="#Step-1:-Detect-Humans">&#182;</a></h2><p>We use OpenCV's implementation of <a href="http://docs.opencv.org/trunk/d7/d8b/tutorial_py_face_detection.html">Haar feature-based cascade classifiers</a> to detect human faces in images.  OpenCV provides many pre-trained face detectors, stored as XML files on <a href="https://github.com/opencv/opencv/tree/master/data/haarcascades">github</a>.  We have downloaded one of these detectors and stored it in the <code>haarcascades</code> directory.</p>
<p>In the next code cell, we demonstrate how to use this detector to find human faces in a sample image.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[17]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">cv2</span>                
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>                        
<span class="o">%</span><span class="k">matplotlib</span> inline                               

<span class="c1"># extract pre-trained face detector</span>
<span class="n">face_cascade</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">CascadeClassifier</span><span class="p">(</span><span class="s1">&#39;haarcascades/haarcascade_frontalface_alt.xml&#39;</span><span class="p">)</span>

<span class="c1"># load color (BGR) image</span>
<span class="n">img</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">human_files</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span>
<span class="c1"># convert BGR image to grayscale</span>
<span class="n">gray</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">cvtColor</span><span class="p">(</span><span class="n">img</span><span class="p">,</span> <span class="n">cv2</span><span class="o">.</span><span class="n">COLOR_BGR2GRAY</span><span class="p">)</span>

<span class="c1"># find faces in image</span>
<span class="n">faces</span> <span class="o">=</span> <span class="n">face_cascade</span><span class="o">.</span><span class="n">detectMultiScale</span><span class="p">(</span><span class="n">gray</span><span class="p">)</span>

<span class="c1"># print number of faces detected in the image</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Number of faces detected:&#39;</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">faces</span><span class="p">))</span>

<span class="c1"># get bounding box for each detected face</span>
<span class="k">for</span> <span class="p">(</span><span class="n">x</span><span class="p">,</span><span class="n">y</span><span class="p">,</span><span class="n">w</span><span class="p">,</span><span class="n">h</span><span class="p">)</span> <span class="ow">in</span> <span class="n">faces</span><span class="p">:</span>
    <span class="c1"># add bounding box to color image</span>
    <span class="n">cv2</span><span class="o">.</span><span class="n">rectangle</span><span class="p">(</span><span class="n">img</span><span class="p">,(</span><span class="n">x</span><span class="p">,</span><span class="n">y</span><span class="p">),(</span><span class="n">x</span><span class="o">+</span><span class="n">w</span><span class="p">,</span><span class="n">y</span><span class="o">+</span><span class="n">h</span><span class="p">),(</span><span class="mi">255</span><span class="p">,</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">),</span><span class="mi">2</span><span class="p">)</span>
    
<span class="c1"># convert BGR image to RGB for plotting</span>
<span class="n">cv_rgb</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">cvtColor</span><span class="p">(</span><span class="n">img</span><span class="p">,</span> <span class="n">cv2</span><span class="o">.</span><span class="n">COLOR_BGR2RGB</span><span class="p">)</span>

<span class="c1"># display the image, along with bounding box</span>
<span class="n">plt</span><span class="o">.</span><span class="n">imshow</span><span class="p">(</span><span class="n">cv_rgb</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Number of faces detected: 1
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAQsAAAD8CAYAAABgtYFHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMS4wLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvpW3flQAAIABJREFUeJzsvdmTJFl23vc79153jz232qu7unu6ZzBLYzbMgmVAgYQwJGAghg8ktJkRNAM5euE750+ADHqhmcxknAeaSJNJBAEIIkwPEiFQEM20AEMsHBEDzNZ7dXWtucXmfpejh+sRGZmd1V3VtUz1dHxmaZkRGRHpGeH383PP+c53RFVZY4011ng3mB/0AayxxhrvD6zJYo011rgnrMlijTXWuCesyWKNNda4J6zJYo011rgnrMlijTXWuCc8MrIQkb8hIt8Wke+JyNce1d9ZY401Hg/kUegsRMQC3wF+DngD+Abwn6nqtx76H1tjjTUeCx5VZPEF4Huq+pKqNsC/AL7yiP7WGmus8RjgHtHrXgZeX7n9BvDFuz1YRNYy0jXWePS4papn3+uTHxVZyCn3HSMEEfkq8NVH9PfXWGONt+PVB3nyoyKLN4CnV24/Bby5+gBV/TrwdVhHFmus8X7Ao8pZfAP4sIg8JyIl8J8Cv/uI/tYaa6zxGPBIIgtVDSLyD4H/DbDAP1XVP38Uf2uNNdZ4PHgkpdP7Poj1NmSNNR4H/lhVP/den7xWcK6xxhr3hDVZ/JBCJBekjDn6iFd/XmON+8X67PkhxWJ7qZqW9y12eyL5a4017gePqnS6xhOC1ZRUSvq2+9ZY416xJosfUiwih6JwGGMIIaCqqCopHT1mNcJI6e2v8ziO8TSsCe3JwxNBFtZaRqPBD/owfmiQUsIYgzGGXq9HURTEGIkx0jQNTdOgqojI8guOti6PC/IObPEkVOl+2LC7u/9Az38iyAKU9Lgvaz/kCCHgXI4qqqoixkgIgRgjwPL9Xl2w77R4HwXWZPH+whNCFo//RP1hhjFmSQbW2iVpAFRVRQgBEVkuyB9UZPFOWJ8PTx6eGLJY4+3QE+vlpHTtbsuprmuKosAYg3MOjBCCRyyoJFQSGF0mBpKm5bbk7cgkIyJETicTs3L34hhXX0lEUDIZLf4nVV0+1hiDiJBSWpLcusz75GH9ibxPcK8aVyUvtEVEYa1FFDQlQgjLrUiMkZTSfUUT5i4PTe8SBCwSq6oKbUXGWrv83eI4RGSZa1njycM6sngf4G5E8U7LfBFVLK7amoTU5ivgKMw/9l31xGu+fdGeRhjvRBZLMlqJWowxFEVBE48iiZMJ13UO68nDmiyeYLzXjhlr7TKkn8/nFEWRr9ri0FQfy1GsRhZG5PjWpv2VqpI0rVROzPE8hySStDsbyce9eNW0IAFY5klE82OMMafmTVJK65zFE4g1WTzBWCyX++UMESHGSF3XxBiXIX9KCSW+bYEuF+bJLYkk9JSw4bSE6N22KIvHrlZfUkp470+tyMBxElnjycGaLN4HEN5OGItE4WnRx2oeoAl+GRGoRoqiuDtZcJwActSgoObYFmGZnGwfa1bW+snjcc6R2nzJIicBLEu4q39/TRBPNtZk8T7EapVkEfavIqGIbbcKIaEagbzIYwhHz1UFjvIUVsxKdCErDJUQsSukklCV5TbGmLtvGZxzS6IAjkU5J0lqcd96C/JkYk0W7zPcSznVOdNWO5R8ITd5S7PoRD3xjMWit06Iy8SitjmMlbJmzFGANYZk216TJJjTciDtoi/LEoCmaUgpEWNcvt5qRQSOyqXrCOPJxJos3gdYLJ2TRLGKk78y5ihKUE1obMukKeGK8tjV25qchAyNx61GCUnIUYWQVHHWgBpQsAoWAyaTRt6e5CNJwrFti4jkEu4Kqayjh/cf1mTxPsFJojhWamxvZ52V4psGKzkisCKAIMaiqhSFQ2NCUvsaqdVAAKUVCptPiaSyzHskBAMYsSiLfMhKviMpIkclVEObZxGIISx7VU4e+xrvL6zJ4gnGyYhitTAhxmBSW+5MirQ5BKtCryzzNiREiAkjgkWxxlDgGHYGVEWBc47COpxzOCv4+RxpcwwhRlKCqO3WwRaEqARNy7Ksb4VdwVqSKpGs0FQgkQOb8XicyWFFpQlrOff7EWuyeMJxGlHAYrHlqGDxK4ugKGE+wxlLZQy2JYTKFThj6VYV5zY3EYVQN4QQMElxxlLaEgUChigCFoImguSopEZxgBpHIuEQIpGaLAU3qiTJx7wgj7uRwjq6eP9hTRZPME4jCmVFf7FIKCrYBNpuSWyCfrdDp6zoFCVVUVIVltI6NEQKFUTBGUe0WbkpCVKKpNhWKlQRY3PEEgMhKg4hKUQiksAlMBj84uAkH1tc1V+024+0ksQ8KQZb4/2BNVm8j7C6vDJJtF8pf1tUPLa3thgNhnTLCmcFJ2b5ZSvD/GCMUSicpWgFXN57rICmCCEnNQ0JSQl8zIRkXa6oxoS2vWgGyQnUlICjyCKXZBUxR9WW1YTnqs5ijfcH1mTxGKDt2yy0fRDS7ulbmTTkhbeICqS9PW+Th8aCE4NITi6G6NGkDIsCEwKEQBdh1OnR63TZ2RhRVVVuVddASgEWCxtA4vIK36SIxggidJyh8WCc4GMgRiWmiE8x5y4kkTC5IGJAxOWF38yIkoiqpDZvkWShnWijoXbLEReeoEaOs99DwGrbPRyVYNfbnYeDNVk8Jhxr2da8VhKZFO7WiGWQLK7SmJvAJF/xS+OwVom+oWMKRht9NnsDhlWX0rpcClXQFEAVQy5dWjE0TUNhLAbBoAgCbVnTiGCMQnx7E9dSLKV5m5K3FRE1NkcSulB8sqyuwPGf4Tg/yNsKvg8fa6J4eFiTxWPAIqI4LqBKGFg2YJ1EEhCTk4a58SqhSbEmRxkpBAa2ZHM44Pxoi41eD6dCChGHokTiYnsigklgDRRiwIJoNsgxkhMNTgxGNLeIq8GoA1WsCK6VjUMbDaUc4SQBYsp/rfWqSByVYpMq+hgIYYF1HuTRYk0WjwUpby04IoxFeVHaTs3Yyq5VjsJziQFNSqUGq2ASFAqFUS5feIqd4YCOK7AxQhOQFDEK0QectRRklaQriqyWTEqtkRggpYDhSHqdomeu7WJHSPGoDKq5ZZSZb3JIZAziDCllX4xcPckkEclbkZzBUIyxd31XHvXiXkcVDxdrsngckITqCZG1ZvJQsdmBauFaZTSTiggExSJYVUwIFGIYFRUb/R7nRhv0CotTwVryNgBFVDFVh5QCKQkWoRCT8xUCDgEDFttuLSzERFAI2s4ZabUQcRElqOawJOZKh6C5NKqJqAk1hsQikgA1ucKCkUdCCO9Ujl39eU0WDxdrsngMyAm+lLOCx3DitiQWcmkLFNagMVFZS+W69IuC7cGAzcGQrhiKBE4UKyBGSMkQU6RXFcRoaBadnqrQGvaKQGEdaiQnVUWImp21TFJSq+iMmvMScRHoGItYg2oitAnP1DZ/RaNLoljmX0zOSCyyH+tptu9/rMniMWCRl0iSMCsEkWCZ+VRpl9XKFdEZIfpIUTi2+wM2ez02un36VYVGj41Au2hFQVAKZ0khIkYorM1OWTY3lunSxNdlaz0FiYmUFklLg4+KjwnvYyYKa9BW+k1rBBxiJLY5CzFyZHSzQhQ/yMEf69zFo8GaLB4LlCTHr7SoaXMB2ZZysc6klWaL5JxFZQ1bgxFnNzfZ7A2oxEDwaCuiMuTEp0gr/W49IxKavSRgqaMIrRHOvKnb7YWgMRHConfDEFKkCZ550yClw6gwa2rUGqJphxS1Sk3JfzTft2K6sVisuWLyaLYCq2XSVbOck0Sx9sp4eFiTxWPAqufE8pRtxUuaEixatlGczWVNTQmahtHGBme3NulYh8SItVDYgpBqED26gC9KlDGBywShLXHEmIgp5xdSVGLKDlgpxTaiaCMfc7Socjk0b0d0IeFevEZKSz2FaQuwJ907YbGgH+17u4pVY+B1vuLhY00WjwF2EZ8vcxZmKeUOKeGMoQRcVGyMlEYojOXKxUtsjzbYLLqkxmPnDR4IKdLrdknSKiol5qpKuzJDVJqQ6DjA5MJtFMEWJbVvqH048uQ0gmn9L6bNlFmoaYInEkkxi6py8jLhkxIV1NiletRHJUk6kqAbWSZTs/T74b+fdxNbvZvz1xoPhjVZPAas6ij0RFKzsBaNAZeUQoUSGJYVo16fi6NtyqLAtUYxpbNoSkR/fFFYKfLtdNRzURQFiZzzWE4ia70qmhiynqIN5Q1C3XiaFI+2GDYnS0PUvAWJaanENFmokXtI0DZFkbcnizzu0m/rnUw4HgJObkfgeISxxsPDmiweA8xKRJFl3lkUpZKwYoiApETHOjY7HXY2N9gajNioiqy+VMWJtElMk7UL2RFvWf40ConcAGacpSwt3nuaGBAsxmQJ98IeT5MQJOJ9xNrEvKmZp0Bcai3yVqYOEaOWgKA2q0Wy6EqXik2j5P+h/S8XzW0JRbi7zuK94l4ii0Ur/Lol/uFhTRaPAbbNaiZpZd5tclNabYQTQymWYbfHha1tzoxGVEVBmTwaI4VmMtDVYTwIUY4bytAqK0lCYSpCmJFSoixLLEqY5UQnmhOgvvHM5w1lWeK9Z+prjLMYY7OIK+YFZozBikGNyTmMNorIgu2ctpXUirjaSCUutJuPcI2+GwGsI4uHiwciCxF5BTgkX1iCqn5ORLaB3wCeBV4BfllVdx/sMN/fWCkUnECWbReFpRLDsNtha2PEoNsnNQ0SE7HxqEmIyVEGIuiiXNm+qFGWmgcNkZlvcM5R1x6M0nUOIyBzYT6fk8iLvq49s9ls2QUaQqB0FuMMtigoNBJVcFUJMVd0sg7jSPRkRfDp6L9breo8jsW6+ncWx7QmiUeDhxFZ/FVVvbVy+2vA76vqr4nI19rb/+gh/J0nBu/ohblyni4e1rgcFotVos/5ggIwSQlNTSeWPHv2AmdGm/S0QOYRFwRfR8Awi4GyslDkzlPn8hYDDEazQU3SSDKQnLRt5x7nHLN5w3TagDHEoJjCMZ4f0gSPFkLtmrzYLdRVQzmoqHWGtQ21zIg24GdKt9uja3vMg0ITScaSTNZgWDEkJCs5jaAYlNj2noRj74kuSpmYBxqipKrEGI/muXK05VjNV6y3Hw8Pj2Ib8hXgZ9qf/xnwB/yQkMW75epOnvxLsZK2fefatpubLMNO3lPa7GR17uxZhlUFtSeFSL/TxcdWD9EuAtc2gS1mmYpYNKzOLBWctVSFYzatsUWZxwQ2DWoUW1kmB2Oa6JnMZ4g1YISqKrBFRWm7bJ/ZQkTwKXJwcICf1zRNwBqDMVC5Au0aojhCTDQxt79Lm8Vd9LrAYqHePa56UJw0BV4liTVhPHw8KFko8K9FRIF/oqpfB86r6jUAVb0mIudOe6KIfBX4avvzAx7G48Vpk8IXWDReHWs7b/ULNiYKEcTnBda3hu3BiHObmwzKkjSbQSuQmk0jlbVL6/wY8oK11qAxZgPdNrGYW8sttp2cfufOjZyorGuSQOM9TWrwyeM10mjNaHvAxvYWm1s7bO2c5emnn0Yl8b1XX2a0uQEWdnd3OTw8JPlEM/fs3drPxBGUugl5JKFCCJGIQUhtL23MjXOynIO8eOfa9+jBBh+fJIXFWIG1hd+jxYOSxU+p6pstIfyeiPzlvT6xJZavAzhn3xebzNV28qWyWY//fpUoFr0SprXLt7lEQPINvaJiZzjkwuY2O4MRxntSzHJtUYi+gSrP3HDGHk0aV5ZJyxBSJq62ZOq9X84bDSHSNA1eIUo2t2miJ1nlzLmzPHXlac5duIBYR1l02Dq7xWg04pvf/hbd1GPQH1J2O8hsirMFVbeLswV17bl9a5fx+BBrHWXlmMQ5qCDELM9S0yo7pSXWlYWqpr1pWNGzvmcstiOrtxcq1nUJ9eHigSheVd9sv98Afgf4AnBdRC4CtN9vPOhBPklYjRiMshzyu7i9wIIoVLI7VDaOyfLsyho2ul0u7exwZjikBCox9MqS0tg8k0PM8sRf7MmlvV+UbG3XzgIxmjUWxKMhPmqEst/FlIa6aahTQ6MRHxs+9MJzfOgjz/PUs08xGPXxBA4mBySByWxGHTwUFikcyQimUyKFZbA14tyFs/T6HWL0LTksBGExd6wu/v/2in86HjyyOPl3YoxrYnjEeM+fmoj0RWS4+Bn4MvAfgN8FfqV92K8A/+pBD/L9gLeNEFzIuQVC8lgrEAMOGHU6bA8GnB1t0DUW4wMmZeWmaZ0ujGEpplJVdGHrD1gRQtNgNDt6w3Eh0iJn4KoSRKhTgyfShJqpn3HxymVsp2AWGuaxhkKIBm7t7eI6ZRZhWUFLC5WjM+zT3RxhCsfmzhZnz59hc2dIp1/gU0PehWZiMKLL/EVeuCvl3Qckibvh2P+uR3Ne18TxcPEg25DzwO+0e0EH/A+q+r+KyDeAfykivwq8BvydBz/MJw9G304QC5y8WzQrKoMqDqVfddjo9RiUHcJ4gmiCmDtPjeQkZUqJ+XwOgBPyFsMYNBZoTJAUW+ToI7akEltttVhLbDx+NuNwMqb2Df1+hUa4ePEpnn3hea7fvMHB5JCZbxgMN6h6FRjDuUsX6Y4GdAZD5inRrRs2trbpVR3emLzMYHPAuXSB8WzCZDJhMn8TMYDm9npan4ylzd4jEFqsmv+eTGie/FrnKh4e3jNZqOpLwKdOuf828LMPclBPMo5tNVYaxBadnqq5MUxElipH23aKmpgYDnvsDEd0jMFPJjjNqktLbiQzxhDkSAy1yEVsbm6SYmR/fx8nho2NDeraY8uizV+ErNYUQVzWRuzu7TFralxZ0nhPZ9Dn4598kfNPXaIa9rl5+xaHkykHB2MGYqjrmsvPXmEePMYWFFWXsxcvsTkakkJg+/xZxvMZIXk+8alPcOfWTfYP7zALc3COWZOb10SEEDxlWWYf0BYPqy5yspN0aQZ8wjF8TRQPF48mLvwhxclkJhyVCaOm5VCdxaDgbIormBRRHxh2u2wPhgy7HbquzNuOpIjGvOdPR9O+YowUZUlRlseukAvDmqZpckk0xOUs0UVFICEcHB4ynk4w1hI1MWnm9IcDnvnQc8x9w9a5Mzz7wgtcePppeqMNksB4OqMoO7iiQo3gyoJ+v4+KIUXo9nscTicko1y+cplnXniWnQtnSFl3jnFuORf1dHFUOvH94eJkKXX1a40Hx1rufR84Ji5iqYZeOloLcjT7s72GOhGGpsRPay6fu8DTZ84zcgVFSnSNRUpBEbz3pBSIrRRbBYqyQEQ4mE2OLbzCOurZnBiVWmrUC3XTEEJCjbC7u0eICYyj6JRMpp7zT1/iV//Lf8CLn/kEv/9//QGXnr5C1ekhtqIabhBCYjTcoq4DsVGSgY3+FmfPnuXWzet4lKo/onOlYjjsU3ZLDm9N6Gz0aFLEhwCuYuprEIt1xdL1+9hSbTtUH0U24Z1IYZ2/eHCsyeI+sGyUWnxfrQi2D8jaK2VRDBYBq3mSV7/sUJpcGpWkJBKlGNQZfMrlRmsstpVzL+z1clgfSDEb5DZNs4wmYozM5w2z+Rw1lqIoqMou0ddII4wnM5roOXv2HJ/89Kdoouf8pctcuHiZg8MJh9MZmqDq9uhXBddv36GwJUVVsjXaYnu0RZg2fP/N79CphHPnzqBG+f5LL/HGm69TdsqcxNWUm1oXcnTJ/4Nhdbt2lMPIjfMPN7BdE8KjxZos3iNOjhZMmhun8rbiyLVKREiTOZXNjWIOgyybviKp9a80rVRarEGMyaa3Kb+uaeXdqR1E7JOn0+kgkh22QwiEEMCCcy67YqWYzWmMobQlVadDrzvg2hsvM6/b3xuLGIsrqzy2MCQun7vI1s421lrG4zGvfPv7/Nmf/SmT8ZiP/MiziMLu7TtcvXqVxjeMNnKVhJAw1lIUhoTLepMQj9VCjn9f4/2GNVncB04OBEqy4ttgTHararcji8cbzT6X/W6fXqebr7QrQ3yitsM9zFHSLmpCUp5MnmLM9nhNThSWZbl8fgghL/qFjV1KuXt0OiVaS0rQ6/coTC4nzn2DMYa9vT1m3/ke1hY4V4IpuXHjFhvVJpfPX6DxkauvXuWtt95ib28PrQPbww32b92htJZoAleefpqiU1CHBlcUpFlzREBi8lAkWJrgPMlYb1/uDWuyuE8YXclVrN7fmtlqK8BajCNMmj0rep0OlSuIIWBiwhqDCPnxtCesZsu7pPl+hUwWJnteWGspbUEKOZqYzWriwm07RnwK1E2TtyfkcmvP9lELMWYiOxiPmU7nvPbmNcqqx7PPfojhcIubN+5wcHDAtatvcePWTd58802cc1y8cIFPfPRjHBzscXB4m8Ggj62Esl8hTnjt9VdxzqGqeXtkS4xtT6sfsHHvvWJNFveGNVncB+42ZjAJxPYKXxqwRjA+kHzAIkgJ/X4XGyLdZBkUFU6Fpq4pqoqgiXkKZGsbm4VWArNJjbWGsjCkTpGdtVNCnCMlwavPIz5CxCSlSLmjNRYd5ge7nBl2Kaxy2EzpuQT1DPUNYgz9wYii08HHmBvJHLx1401efuv79EcbXHjuIs8+82F2zlwmNJa3rt1Bb98m6Zzaj9m/cYeQDjncP2C40+VgPmU612z+GyOlzWVTwecRBwKKBSmIalEsyWZ5OppLxEYEoymLutQDuiIXN0tbwqUT+kPAaU1oa5yONVk8RGibe4i+QVQoigJtAjubW/S7PZxzuLSY0QG2MG2p1eBM+1Fovk+AwlhE2tbrlRJtCglrXH4dk6eBGYmQcmdoxFCWZe5STdlcJ/jEZDLh7NmzvL57m56xDDY2MOKYTqdMJhNijHQ6Hc6fP8/HPvoJzp65RFLHndtTqo5l7g8ZT3ap612m89tgZhyO7wAGYwyVMzQIJpmlkrIwZIFWzn7m+SKaxysaTblzts3x/KCwJol7w5os7gMnT6lFDiN7SmgeSqyaOy1jotMp2Bht8JGnLvM//uEf/SAO+Qivwz/5vR/sIbwfsLW1+YM+hCcWa1HWQ4JRKJxDY6BjCwqBUiw729t0bfGDPrw11nhgrCOLB0JrY932dECudBjnKIuSYbfH1mBAudJ9+bWf/hmIoW0313boT4MTlxOFKZF8IEWIyaOqzGNNEgUxhKjUITKb1tRNXFYdrBWqIr8GxtI0DYU1uMrR6VXUqWH70gX+9n/xn/Ctay/z+vVruG7FaHsL4yy3b99GJweI7dKp+nR6fTa3dojRU/Ud129cZTy9QUoN/W511Kuiwm/89/+Wq9duYE2FdRWqrZFFCljjs4s4bfs++fhUDLVv0CStifCRH4VqBFmRievivX73nMVpycqTPSQnH7e7u3e/H/wHEmuyuB+szCs95gil2UYuNp6y7QPpdvvsbIyorKPwfvkSmgLGGohpqc1YnMwx5sWvMWZT3ZQQJwSfaEKDVyUhNCExaxpizJ6YRtNSQB1Soup2iL6hdBWldThjUVMwOxzzW7/xLxldOcfgzAbb584y2h5xMBlzdXYIzZRbt2+ytXWWs65gMjkkmcjeZIzSgDTsH9wmNF2sLZhOGm7duM10PMNExVohzOd4H3DOUpWO0uR8RpI87yQGT/CehGJdmUmQlEcGiOU0KfhqD859f2R3cQC/G9bNZ3fHmizuFycGHC8sXIxCDIHCWtJ0Rnfo2ByMsJqozNHbvPCnUJsbxDCteAtZ9oQYbRdYAiuWZKBJiUYjSYWEpSZixIGRdpBP67ydlLLtNXHOYQ0QEyLKbDJmd3rA5pWzjPo99ndv8ub11zHO4JxQdCt6fc9oc8iZczsAVL2S2VyomwOq7iYiSrfsEmrhcO82hwdzmsksWwaiCAlnYWs0ZGdrgzM7I1SVEALT+YzxdM68bvAxMZnVBGldy40sZ4y8jRfUrGg/H45pzhr3jzVZPAQYwFlH7UO29e/1GPX6VNbgEkjwxx7vnMsLu2myq3aKmFZolbvPE04MTYoUYmlSZBYampha+/9EMhYfAhoTzmRfT+dc3hrg2dwa4FyujoTYEFBMadAQslXem28y8TNcVTDcGKDRowQuX77E01ee4+y5S2ANBwd3ODj07O8fcubskE5Rc+v6Hp1qSKcYYbRH9JFUQ9VzXDhzlu3tbS5cOMeZnW2sBubzOfOmZjKbcTCecHt3l8PJFO8N4iOe1syHI0Pf08aNvFOEcdLZ+6Q35/1idfbIGhlrsnhI0LYa4lB6RcGgU1FZCyHizPEzP7QzRqMmDLnvIzTZyTsP6DFIiExjwKoynteMm4YmKYvrt/cR9dlOxiCtTX8CEiEmyn4/y74bjwo0KVLPIvv1hI39fc5cPsdgc8jET9pZIpHB5gjnOjTNnPH4AKzhzp07uS8lwSvffx1fB5pZIswbDnen3HprF6tw8fw2zzz3HM88e4WdnR0qZ0nRMxkfYCRbCpZGqCx0nCUUhlAWWfYeszt5Dh3aIUhqchS3xCJfcfr7/05bh9NyFov738m3c43jWJPFe8YJK/uoOBUGZYdnL1zk4sYGHbFghTidLR+WUOZNs2xF9z7P76jnHuOKbNhplISyW9cosDebMQ8B37pgpQT13NOzBV1rcdZgLRiJFEYIoebgYI+iqIgKk9mcaeNJzhCM5d9/8y/48+9+l4uXL/ChD3+IS09dBBkxrac899zTHI4n+DDDmQ57e3tcv36Tb37zm7z8nZcoxRE9SJKlNuRXf+VXeOaZpym7JbP5hKapmU/H7O9PscFjg6dIEaxAr4M1yqhfcntvxqGdccgM0wheBSUdRRf64MW6k4v+XiKNNVGcjjVZ3Bfu7vyUW9MT/W6PYb+LM4bUNFSuwJZHpdPY9nt474ne40yxrCrU3uPb3pCEMA2JRGSWIo0mAtpOP4fYjhg0TrLrtySsKAZLWTmcOA6nE4xkm398Yu9gDJ2C8WyOTgCxlJ0eIhbnDFoKL730MnXTMNzcwhjD1avX+Pa3v8uffuNbDLt95iExm0wZDQZ84hMf58WPf4znnrlCt1fRhBqSR9RjJFKatpITPSl6SPkYC2dAHVVhqQtHpyyJKUBKhGwa9p5wMko46dW5eMzJmahv+5RlURwsAAAgAElEQVTXIwROxZosHgJEj0LafqdL6XL/hoSItXZpuLvAsmM1go8ejTniaEJgHiJ1DHgSswRBA9Pg8eRti0KrBMuzOowxGJuD9Gx7I4gaprM583mNsZC8MvMRnwSLY7S5QzLK7d199r/550wPp1y8dJ7O1ogQ7zAaDYDE9es3+c53vsOf/ek3GQ6H7L11yPbWBp988ZN87IUX+NBzV9ja2qLf7eKbGT7MSMGDepxAWeZKjEERzeVlK1Bag1HbDgjKX2Vh0SBtE11qFZ/3Vwk56aC1fL/vYrH3blHGujJyHGuyeEjQmBvIiqLIcz9DamdnSC6VtkgpIWahLQjMpzWoEnykiQEfI/PoCVGZA1Ej8xiJKRFNS0oGCizGZV1F4QSXsnlvYYQmJWazGa7ooK19f8KwuX0GqUpuz/ep/Ry1hlFvk8lkzh/94R+zdek8SRr6/S5Vr2I6nfPKK29Q1xDmY55++gof/8hH+NSLn+DDz19he9THGDjcHxOtII3mZGpooPW3MO0kkfa/z8OVjCFZEM23rRiMUYwBkaOu3eV7uySMd9+W3G3x38+iX0cWp2NNFg8JeU5o7tdYZNEXNnerkYWPAYtdlklzcjELrUJM1MFTh4CPAa0qYsqu2Gkxp7w1vXGSI5aicBTOUCRDoZHCCo1P9Ho9VBzJFHSNo3IVxbDP1AdG5Sb9YY+bd27y5ptvURQWIfHm7i6dnqXxkQh0OjCdgHMw7G7yN3/xK3zswy+wtTHAEQihxkge8GOCAAknYJzD+5qUQuu10eQkKbkVP2k4tWqxiNDezfLiblf8d4oSVh+/zkm8N3wgycIllsOATnaSyooN3EJ1CPlxZVDECrXmJFxhLaSIRE+HwE6/ZKcLwyJQGEtlhMIp89395eublPAh4n3Ep0idAjHBQQrMRJlZZSZCY4W5TSARaQIOpVClTEKhiW5VMnCO0uRFajsOI44mNBRhg2JQcDhrsJ0uojDzniYI0hmwtdHj5Zdf5s7+mF5vBx8axuMxVW+TWFsqm23+6t2GrX6P7a0NPvfZT/Plv/JjBF8jqaZwlvk0cTgeU1hBYoNLUGpJDAFCbn6z1mLLgo7NW4wmeExUSmOoTIIKGh8wvkFsFm0lcajY/Nmoad22UnZB5+5X/LuRyML4ePGYd3qNd/vdBxkfSLJ4zzDSdpZaaEVUlnZBqFKYXJkQkbwV0UhIxydmzX1D4wMhpKzM9PkxXiNBlQDtFdhkgRZKIYbCyLLfxIphczDEAVsbIyQ1zA738SnS71YUmyNu7e1x5tJFRts77E/nNNev0wgMel3EWgajEZN6yqyeoxoZboxIKkwnEyDRrTo8+/QVfvTFj/MjLzzPC88/R6/XYz5T5pMxk/GY6D1FUUAKLEubK/kBay1lWS5dxzV6DJJjJBHKsoOJysx5jAmIpKVADRYGydl+717yFqdFD4v7TuYnTuoyTr7OOvp4Oz6QZHHXWv1dzo+ldR6LkDlP8TYJJCWMRoadiq3+kH7ZwaaI+qyLICnij164qT1Tn3MSSYVQWLzCbBaZpMA8RWqNhJTAOhClYwwdga4xlEAhhsrn6MXUgW6nQ2fkiN4jAjdpOPPR53nq2eexVcVbf/lt2Bhw8fw5Ot0+k2bO5Nob7E4PsVbolBVSOur9CR/7kY/ymU/9KD/xxS/y0Rc+TOEM08MDNAXqyRQ0j040IjRNO7jZx3ZRZtVHiguzHcG5km6pzGlIETQ1aFBiigwGA0JUJrXHzRqsKJaAplwiPnrX0rEsxr0s45ML/p20Fnd7/hrH8YEki/cKFRCxtFZWR6MEm0DV69AtHCZFUl2jPrTjBrOPwwLzxlP7XPUIgA+JOiUmvqERiGKy54Pk55qUcEYZFCWDoqBjDE4FJ8K5s+fyNHSxjEYjmmbOwcEBg4vn2X76Kf7vP/tjXKfHX/8bv8DHP/Up/uzf/3/8xm/9JteuXWMyOcQWBaVz1L5m3tR89hM/yld/9e/zoStP0+1U2AQxNHSLEl8n5j6gmonBFQViTHbH0qz9qKo81NkYgzQm53GKDoIF45YkC/NsPNz6b3Q6HUb9iHUeHxK+Dq0L+P3pLFaHD8HpkcZpuZI17g0fWLK4m+vV3U6dbE5tljohUTJhoBTWsNkbMKi6mJSt8RZEIauJD2DeBKbeM/Men5QohnnIWoocSeSGKlUwUTFJsZqQFLFqcRgKEbY2cs/FcDikKDs0MWA6PZ67eJk3+o4/+da3cL0O//nf/bs889yH+H/+8Bv83r/5N1y/cYPdvT1Gw34ejZgCH/3ox/mpn/hxPv/ip/j0iz9KVTrwgRiyr2Yd81YohYgrsqFw1JD7OZwlhdAmcktMSwoiFmtzYtPaAuwRWaR29MF0WiPO0e12UVui0ymHsznS+FM+gXvHadPKVn+3+pi7NZqttyFvxweWLOA9+EwbIYRE6QrQCN7jTCaKnY0NRp0O+Agh5agAIWlOaC7gk1LHyDwlGrKFfiOKF0FQokobwQg2KVaEyjpKFRxQmpxY9aGhHIyY+UCwAdepiAJ35lO++fobvPjJT/F3/vYvs3P2Ir/5m7/Nb/327zCdTvE+b1v83HNmZ4vPfvazfOknfpwXX3yRc6MtSJHD/QMkRgoMJikOwRQlw34fV5ZEDTTBo8HjY0LEINZhTA4xTErYlBBrKaNC01Bi0CSEqBQBUjT4lLtV85yRVixlji/g+/mM7hYpnOwZWf3+Tq8Fa9JYxQeSLE6LKlbzFSddvJfPwxBjgy0qlERqAkVVMux2GJQdKmsIsxnEiNrszu29Zzw/8mZoUiIoeBECwqSpCSiBXJqRth/CkKselXX0q5J+KfTLgmG3R6esmM0bpCpQA7FyTKPnrRu32D884HaR+Ju/+EuIK/j1X/91/t2/+xP29g6IjacoSna2tnnuyjN88Quf5yd//Ce4dOlCvrr7Bj+pkSRUrqRyjljPCUmp53NEDaSEInS7fUpVmIwJIS4rDiEEjLE4V6CqFFUkkZWrNiWKGHHOE2MiIjTBkxDqEGm8z9GOkK342g7fkzmmu+WWVsniXvMSazK4d3wgyeJueMctSAtrLaSEhERpLP2qw7DqUlmTRwkqmFZfEULCh5QTnS0mdcNcYB4TsxhIVohkuffiGBbHUYmlX1R0nKF0ll6vR7fbwxQOVzhujPcp+gMOxge89NrrTJua8xcv8bM/+XlCCPzPv/0/8X/83v9Op9Njsz9kv95jVPX4Wz//S/z1n/tZXvjQ83mgsm8okmHWRJwrc6QQA9qSQFEUxNAQfcQVBWXpMNaiKT8eV5Jaosi1Z4uSiCSMLTA2ISYb2tQxvx/J5G5a7yOz2mOso+xUuKpE6iZv5cRgncW3jXfGtJWmeHoFI6W01LacViJdJZL7Mehdi7QyPrBksXqanIwqVrGshAiQAkYMEgJWE8NOxfmNIRc2N3AxUqiiKRFi3l7UTaD2DRNXLl9vLwRqo8xFaZyhTiEPIZas/ygUKuOorGGUDEZgONyg1y+RwjIxEEm8cecmY2O59car1KqMNrb42Ic/yQsf+TA/cuV5/vF/9V9z9bWrnBtuMugN+fxnP8+nP/0ZvvBjX+TZK89R1zW+rqlsQTkYZfWpWJr5lKb21HVDMELHOWxZgW+YHwSkiGx1N7BFyXg6pVNA6mexmYsRrWuadrvhU+RgPmE2r5lMZty8eZNbt26xt7fH/v4+bx3eydsOTBauWcd0VmeVa7swffKoygoBB8q7JD4X4xhOiuJOyr0XvSF5dMPbpeEno5OTW5cPajTygSWL9wpnJEcQKVLZDr2iomMLTGjy1TTkReJDykKoxjNeef40eiKGZG07jSzPNi2QVlMhdIyhMpZu1aF0lmQEtQ7b7VDHwN50zEGIvLF3m42dHS6eu0C332O0ucFgMODqq69y89pbjHp9nr3yHJ/73Bf4+S//AtvbOzhxTA4m9Pt9Rv0RKSXquib4QFGUhKZBxWbXKiMEQKMiJs8G0ZT1EUVR4ZsIEYIk8J4mzPAx4UnZGSsmbty+ze3dXfb3D7l+/ToHBwfM53MODw+ZpfnSpTzGSKQh+LZ13+Zqi7Tak6VQTvVtIeBiES8W/2LBL0hjoflYXfx3E3CdjETWUcURPpBkcdp1YfVUkLs1l8aEWkMKHmsc3U5Jt1NSOIP6mEuqtOVVAxhLspbJ/Ci7n0QIxhBEUWPbTyDlxCCGAqEAKlU6ZYErC8pOAaVjEiOHsyk3D8fcPDzg7OXL9AZDBqMh/X6fwhoO9nb5P/+Xf832aIOf/tJ/xF/7mZ/lhRc+wuZwE02t+5Yp8D6gCraosEWHqA0pNMxnNd7nhKwYAyaXd8VZTFvtAIM1Bc4UBMn5mblvqH1DHTw+RA4m2eTmj/7kT7lz5w6Hkwnj8RRoRywmpVN0WgLKjuhKwhmLVcGnhBibx0DGBJqby06ODFhdxIuI5GTuQkSyZWH7+0VkARz7efU1F2RzklQ+qFEFfEDJ4m44uQU5CRHFGhBVnDF0qw4dmw1crBhE8skVYqJuy6NNiO0AoYxkLAElSv6urtVqxJCrCCKUmqXdVbdDSgFTlsx84Ob+LnfGh0xDoNrYZPPMWbwPzGYzUlNz560GX8+xYvhbv/QVPvuZz/HCcy/Q7w+YTCYUrgMYOlWfJiTqmLIICogKhSuPrsY2t9ZbFIlZodnp9hFj8E2kcBGDQaPSaB6jmGL+3w8nY1557TVefvU1XnntjVYlmlWqqMmiK2PpdPKUeINdzhlJSI50ag/krt2oCVWTiYO7RwXLz7HNbZxsSz8ZUdxNvfluFZMPajfqmizuA7YVHCFC5YosrS5dzmUgoHms4Nx7prVn0jTU3lPL0dscJBvb+NazIiXNJIQstRmVy4lNYwwhKQezCXvTMTf27lCrUg4GXLryDP/hL/+Sc2fOsj0acfPWLcJ8xs7WNl/43Of58pe/zJmdcySfCCHQ6XQwUhBCYn98iBiHdSWBgIjNIwdTg7W5imGsYp1DUyCqoiTKTkUKkbpuKF25vPrO5nMOx2Pu7O9x8/YtXr/6Bt956WVev3qVw9kkLy5bYFyZqx1GKMuKK089RVmW2be0ndNazz139ve4cfN2jgSszUOSlKyGXfk8Ti5Ya+3y/tV+kEU3cAhhOQhqYZD8TjmLk7dPJkY/aISxJov7wCJ55oCizDmFTlnhfENK2dwlxsXc0fw9KtTxaBuSW83bBBuKDwFn21ohijNQWkenLAjJIyLs7u9z+3CfJnkGW9tsnjvHWzduIORJ5zqvqZzlxY9/gp/8whf5zCc/x2AwoJ7NcDYnVxf79hASrihQMWANhSsJKTJvaur5eLmgRPLCi5rwsVWjWovGvKhzdSILrebzOXfu3OG1q2/w8quv8NJrr3Przm1mdd1GBrpcsEVVsrm5yZmdszx/6fyScLz31HXNfNYAsL9/SN00R/mGcORgfrcAcLXjF443kC22IfezrVglhw8aMZyGdyULEfmnwC8CN1T1xfa+beA3gGeBV4BfVtVdye/oPwZ+AZgCf09V/+TRHHrGg7C8ALY9t5LkgceLblQ9+TgFZyzSBDaN44wrGCpUscE5YWw9M/XckAZvlLm11KZkHgONHImyapdIkjAKlYduUpxXSgy2LKl7PQ6HfZpuBxOUg4MDbtzZo6hKts+do9PpMN7bZ7q/z1anw3Q64cLzL/ClL/0VPvPJT3Hp0iW6ZkDdwHA4oKyqfBUVxRSRbrdkXk+JMWKNxRoHGknSsK8NUx1jJbYNbYJxUHYSvm6IIeFD9t/YO5i1g55r9m5e49VXXuG7r77Ka29d59qdmxxMJzQxQPI45+hUjn6/w/nzFzh//jyDwYhhTMS6wdcNLihdsYwFZlWJKRxN9K2hj835ipRzD9KOfTz2Wdqsx5CFd4jkdv7FtiWkSNK2+qFZMHfXBGd7ThnJ9gKnNaN9EHMX9xJZ/HfAfwP885X7vgb8vqr+moh8rb39j4CfBz7cfn0R+G/b748M74UkFmYq99SQxFEuwwqQEjtbO5zbOUO3KvF1nYVVGpj5hsl0Rh2hDkrdJJqYaGQ1oeayq5UkbAJr8tZj0B9QVSXGWSbNnP3pGE2G2WxC0e1y7vxZrM3DgA4ODuj1OvyDv/f3efHjn+Dy5csUxpFSoqoqRAr6/SznnswmzOsp8/mcpmmYTCbs7+8TY6RXdRgM8gzWGCOzxuNM7pYtHIxGQ7qdDgBFUbB/uMd8OqPxNb6e40PNZDLhj77xDb7z0stcvXmTw9mMOiZUoBCh3+vTKR2dsqIqOrg6Mrlxh8mNPa77SfbZsC5XVVq1a4iRJAkRlibEIrKyJTndV/Nureim7eA9lgxFT81hL15D2zK4cvpWZPHaHyS8K1mo6r8VkWdP3P0V4Gfan/8Z8AdksvgK8M81v5v/r4hsishFVb32sA54FasnwEnN/7uassq727WtEsWiFwSNdLtdulWJUZYO2kHytqMJiTpBHZWa7CcZTvtDbZNJjB5hcaXMPROzpmZe54ljxsLOcJvJdMatmzewCM898ww/+eM/wc//3JepipIQYuu25ZmNJwRNvPTSIddv3eT27dvs7e1x685tdnd3c2XAe6y1DIdDdra26Ha7bQJQOXd2J9vclTlqqHsDkg8YDOPxmKap8c2cyeSQ6WzMwd4es3oOJm8XDOSJ7kVBp1MiIULyaACSRc2cJuQ8yu2DG5Akb+eKEld1EGMJmiiKAhfymIQQW7ctyUIvcKiuLtYjgribcvPU5jLh7a5cq+fNSpRx2uuffN4PO3m815zF+QUBqOo1ETnX3n8ZeH3lcW+09z1UsjitGei9hoXv1FC2ShQCiEaMtXSrAmeEFAOp7fsIIeFjrjDUSalVsoxblHjsJMpXLtFESooThzWSNQ0p4lPAh1xdqCWwM9pi3tRE7+l0Onz0+Q/z0z/1U/zHf+1n6VddZrMZ2i6+69evc/XqVb7/xiuMZ2N2d3eZTCbUdc14MmE8HuO9p1NVOGfo9XrcGI3oVR2stXQqx/7+BoNen62trWysG6Gua5xxS7Jo/JzZ9JDDwwN29+9wMBkzredYaxkMBvRiXjzWQMeVbAz7jEYj+r0hnU6HGBMHkzF79QHz6Yw4mzKZzjFugi1Kks0y8KiBkBJJ03KgEshyxtDRAs0OpAvfkOPnRGqJxR6LDpafszl+AqwKwhYir+Vj36E68kHAw05wnvZunvpOishXga+2P9/bi59oFCqKYnl7kZi7lw9uMfn8nqILPSIOg1AVhk5V4oxBm5qU8gnaLOzwklKr0iSyUzdkPUUL1exxoSoYVZzLprY+RkiBEGMuFRph1B8y2Bjyyre/y5mdLb742R/jr/70X+HHPvNZzuzs4OsZ88mUa9eu8fLLr3D16lX29/e5Pb5FCIHxeMx4Nm0t7vJ+3VmhKARjshlNPZuQQo2I4GtLv1cSC0cznzI9HEOE6CPWFEync2azCT7MaZo5TfB475nHerlQC+sImhO9EhKbO1s8dfki25t5pmrTBG7f2WW8f5At/12BbzxNPUNroSw9UpTt6+VoB5XlSXTy810SA8cvIotIafWUPLmVuJfS6N2SoavK0LedMz+kPSfvlSyuL7YXInIRuNHe/wbw9MrjngLePO0FVPXrwNcBnLPv+s6eFNvAUals8fv7+YAWhLE8nhO/N3qcKBY/V8ZR2nwixkX1QxPBR0LKsy+8Kl7AIyRR4qruR7MeI3tt5atd1KyiVMk+FkjK5rUmMjncZTjo8OJHf4Qvfu7TfOTDz7E96pPqmreuXeOtt27wvZe+z6uvvM6t3Tt5+pc/oGlye/mCRItORdVGFFXb5GWMoSotzuX3sSoMw36XbrcCoJ7NKV0HZ0usLXC2RHWKJsG0ysvsqZnLwVETIURSyCTYrSqef/55Lpw/S1EU7B3sszc+5Pb+HncO9rntJ3nIUErEEBDjcnk0RHKLe44k1ASMcXk4ombx2iKPcfz8WH2jE6wkMXOJ+t7yDifPs7vhh5EQ3gnvlSx+F/gV4Nfa7/9q5f5/KCL/gpzY3H+Y+YrTNPoPuk+8m1hzgQVRAEjS1s7eIKQs746RJgQCeeZoEkNUIZpWR6Esbe1XXpXsYg2qko1tNWKtwRT5pBcRUjPncD7nS5//cX7mSz/Nh557BkdifHhAM5vz3e99m2/9xV9w7cbNvI3oFzSpYVj1uHlzghXBVUVrMFPR6/XY2NgAcr7HGZsJpMiLrFtYBM1jDBw4V1KVXaqqS+E6SMqGNnMDPkDTzAHDbFYzmU5pmgDGUhYl/V6PQa/7/7P3JjGWZel93+9M9943RERGZEZWZmXW1F3d7Ca7WwJlWga8EG3BOwMCF4atjQFbsLyQ4Y1X9kYGBO08bAwYkGHD8MIytDQMAQYMCSJIiBApkqJIkeyhuqYcKjPmN9zpDF585973IjIyu7obqq7MrAMkMoYXL268d893vuE/MLuxSzKa48U5Hz98yJOnT7lYLlmtV6z7buu9leZlHyJd24DSUiIkjc5BdfyHGlsJ25nF5ZM+Xtn0l5ufw71zXaYy3huvWTD4SevzjE7/PtLMvKWU+hT420iQ+AdKqb8BfAz8B/nh/xAZm/4QGZ3+Jz/vBV7X3d4OEgP2YZsH8HmyjOuyimeo0Fceb3Lg0AbatiFkY2NPou09bUziR4oIvEg4kQxk++/RWkOUIBEzNiARCKHHaYdzBlKk1ImydPzqX/g2d27fYFZanIXV4piHDx/zu7/7O6zqNbMdgXyjDQfeU58dMSkdk8mE3Rs3KCt3qWQbsCClla8boyXYWEPfBybVhPl8j/lkxqSYMKlm7O0esDvbxRjNk6ceSBRFRYqwWEkvJCrRtjKFo5rP2Nndow2epw8e8PT4CZ8dHbNsGnwQsZ+dPTEyWq8b1us1ne8oy5KUIAzerykKTyUq+jgonMdnDokhs9jcB5ZtA2XtrJSeVw6Yq89ztQR50aj0amB5XgB6VdbnmYb89ed8669e89gE/K2f96K213Vv5vb/w8c/TYZxtXEJLx6jDo8vjGVWVPiuxXcdMXb0MbDqW5Y+sEqKOih6BV7kKEnPSWmjkoyjCS3KJEpjJIOJPakVENedW1N+9Vd/lb/8F79L8oF6ccqP/uyP+Zd//MesVjXvfP19vvWdv8KdN+8SEZxBWZZ0T0/4wQc/Yr1e8/TpU06OT2hb6SsUhePOnTtMnLikaQXzasJkMsFay5t372GMo6qmzGd7WFPhfeL27dukpDBW0XUdxyefEbzCe7g4W1A3HbaqSFqjq4rpjRvs3b7FP/vjP+Lk9JjJbMpbX3uXH/z4A85Ozwgx8a17b/P222/z4PFjfvTBByyXS5qmFYPnIK+Z05oQA73vQBm0NWxnDUoltBiUoLUZuR7PZJ/KklM5ORVSGj+99F7nEi3FlAP79Zv/6jj1VZ+EwEuG4HxRxL6uHn3uY1/w7edNRwB0UJTOjZlAJOGJMiJVokuBivnGlaaIUfKYrT9Crk+J/WCM0rHvfKQ04Kyhso7KWb777W/y3lv3MSnS9C2ffvop3//hDzg5PeJr73+Tf+ff/Svs7O3jQ6TpWjofWS9XXJyfsVgs+OSTT/j04QOUUsxmM6y17OzsMp1OKYoCcpajrIwri+xFYq3DWktROMqyJHg5zZ0tKMtyzFJkUylSiBnLkHDWUFQlIUVOLha0fYd1BXv7BxwcHLD75Ijj43NiDITeU5Ylk0nFdFKRYuDC92I8ZGXTW2vpiaguEXQi4UnpckDYvLTb7/3Qv5CSJeUpx6VehVKo52A2InKSXD2Uth939Wee9/mrsr70weK6cdewfp6I/rP8lIoJqx0RuSkDiS4GPELL7pOgHsXeQuDbSYmU/eUl47zBdMcYS+zWJG0ojOXm3i6HNw/4xte/xv037wKRvm/57Olj6rrmna+9x/e+9z12d3epmwbvg+hith1HR0d8+sGH/OBHP+T0VPgVh3feYGdnh5QS8/mcmCHUg1R/kQPgALs2xmAUKCJGJ8pJgSKgiFitMRqIieA9MQTJOJSh7T2uBGdLVnXL2cWSe/feoq5r1uslH/7oQ9YXK0wEa0oqa2jXK55+9oizsxOqqqKwmnq15PDGASkpXFVKM9pqQkq0fZcnJYpEQmHzuHOwIhhKCPLnY3Pjc8G3r47jn1d+XL0vX9UAsb2+9MECnp9R/KzNqKu9iOdlE2OrLE9OrLYUNhsZa40nGxQrhU9SIUvWkANZCjnd3T6FpKWalFgTphSwtkQFsEYzqQreOLzFN7/2Hjs7O+zt7ZEULNcr+j5w8/Yh3/3ud7n/9lvU65a2lSZhCInjJ094+OkjfvzRhzRdx8Gt2+zu7rK3f4Ou62jbmtOzM0IIzGczyrJkPp8zm81QMaEMdF1HWRUCgIotfS+3SIyi9dn7lhB66bfESIxeUJUKkhdOSYwxi9gE/r2/+huslyt+7/d+j0cPHlBiOJjs0vc9i4sT0qc956dHhL6lV4IeNQpmU6GvlxPRFlVOAnO3qCFs9RIQJuuQJQ3v7nhvDFmI3vRrtu+X+IJgoJRkTc9bz8s6XtWg8aUPFv86X/ifREm/upxz2YpQExCRmy54AV6llCX8jYxGlRpHLYrLwB7p3udfrqURaq1ld3eXN2/f4p237vH+e19jPpff1XWei9Waajbl9htvcOfuPSaTGcuLFaH31Muap0+PefDJpxwdHXG+WPDOe++SUqKuaz59+IDT01NAAFZaw3w6lCU73LhxA2sMN6oZ850ZRemYVhMgkejxXrxSus7TdWJKhBK2rFIKnU2ADJKdXJxd0HQtBwf73Lt7n7Ze8dnHn0IbODs5pcCy8AsW52fUbY01mtm0ZN3UKCLznQm3DvZQSmOLgp6IXRua0LNuVvj+ss96IlxCwSqlBMQFxEHT9ArAangvrq7hfhuh41f6EtdlG69qcLi6vvTB4kXrair405QlP018zdAAACAASURBVG2gGFZKKvt3imRe27Z4JSmyT/L9RBrTYGLakJvYOrXkM6wVBSprLTdv7nPv3j3u3X2TN27fZr7jhNPhe7z3zHd2eOONu5RlKdTwdcN6seT4+JQHnzzk8cNHnJ8v2LmzT9N0PDn6jLquAXjw6BHrtYjP7MxmLKYLvPdMqwkHBwc457i9cwNtZEojkG8xXo6pYzKZ0XcbnobWEiCG/s/A6uy6jrpp6YPnzp07/JN/9I/xfc+Djz7EKEtsA4Uy7FQzqDqi0iglvQmjNLYqKLXl8PBw7KfUfQdWYfuOxXpJU68/94Z93ga/DrczPM+2II66hm8yfPy85vvw/K/aeqmDxYtm5C9aUelcelw5afJ4VD4Rr86w9ZS99dShpugr2qWmax0pQBd7ApGIJ5g+n7YGokZFg7WXf08KkYT4feqQIAb292e8eesWb9+7y+03blJOHCYFysISk6JwU5HCm+8R+shydU7frnly8pQPPvyQTx58RtP22GlBi+XTTx7y5MkRF8sFMUZWyxqlZdOcLY/Z391lWjja+pSLiwus0Zwe3MXu7JJcyWynY3c3YnuPJhA7i0FDaNC6w9lAoCWqhnI+oV0swUf6eok2jmnluDj7jB//ODIpHUo39G3HfAoajbUz2jRl3a7pQ0dRaqamwDnHjd0dbt0sIWmKomC5VqR2SaUMYTKhDee0Ao0lYLGlYEFi9BgDKQW8bzcbXwHI9GdAsg5NWu/9pfcGLYF//FScVoFESnEL33EZs/EikNersl7qYPGzrs/jm3ndajo5MaMTtGIg0SNmv56sRTngP6TZPnqADGs2mdJ1XXZPzwEp9NzcP+Ab3/gG3/rWN9mbTTEKiqLEaYUykfv37+NcCWiapmN1cc4HH3zAJw8f8eTpEat1Q9MGmtMTLn78IUU15ezsjLfuv8N7773Hw4cP+YM/+ANijPzyr/wSd24f0rcNT5885vT4iK5vWCx69uYTLIF5VeKM5mD3BrPZPF+zIEILY6mqiklZURYFk8mEEBPGtfjIqFlx9+4bHN7aQ6VA8p5CG1SApq7pmjajPicoq7CFTGKm00pKo709+qYlJIXVEP0uddsQu44nZYlvOwJJAmDOaCCSrIgIjSe/VmhlMNaOzvXbWp3PW0PDV8fLuItNNhte+Uzi6notg8VPWs/zQu36ni7IIDRZDUGTggJt8b4lakEdJvRmjq+4VCvv7++zWq1YrRcZHCWYitlsQlUU441cVhXOynO3fct0Os/9Enm+i4sLVqsVdV2zWq04O1+wqhv6LvDO+9/i137t1/j9f/FHtG3L7u4up6enUu4Yw+HhIffv3ycFz3w24dbBTbzviFFzcnREZQ37Ozvs7+zQT2YkH0haOC0qT1IKaynLchzJKpXl7MaUPZBSxFhFaUqUdwKdD4nCGMx8F1RAWYMrLbYwDNaIRSlZVSBBCuIgr6BLER17Cmep215O+axelvQGixsZvFITOgmcni1z6us2/9W1KbWub3C+DtOPq+u1DBZDZvG8oPC81cdE03s8kaAQVmlizDJSkskISRLXiEaRLqW6rjCYVlzWY99hjCIpYYAao+TELArczlw2oDGSMlvR/+77npQS3svJl3ygXq1ZnJ8T0UxnU77x/vv8+q//On0f+K3f+i0+/ugjnnz2Gc5anDbszOaUzrFY13SNiNPszuYoa/j4ww9ommZkX8rv8mh6tLZCiS9LmqJiPp2yN9/BWj1uPGsNGknv27bFKs3u7i6VNZiIBB4v5YFTEZ+i4FEKgzICpbdWE70Hrem8R8WAJWBSxBrFZFKyaluCF58QbZQEaqXIaQVGOZEDVArUZTFfeH4vY1tNS2st7+BWqbF5/KuPq7i6XstgMazr0JtXA8j2WFVpTRc8fRID4z4m2ujpk4ik8AwHRBCcekuD88mTJ/i2Gze9RpMMVEUx1tHDWDKQsKagLCegzbhxY0hMp1POz8+5uLjAe2lIGif8j+Pjpzz49FNIAWMUi7Nz6uWKvfkOisjF6Rmxazk9Oebp06cQPJPJhJs3b/LeO+9y/+4dDm/ewmrxMfXekwLM5yXOTUgp0XUd02rCfD4XV3WtKaxDGY0gSxQx9DRNTdcUVNMZhRNvkGTEjGlSOLq+xyePMwICs048RPp1gw6JvoPkvWQlJCbWMilKDEoylxTH7E0ZjcpZnCQdgmrVSrIWnQPAkOlt0wTG9+vKph+mItuPuw7W/TpwSl7rYPGT1lX8RdKKru9FbFdDQ6CLguRM2oyPH5W48udmi6J+enQsp6rVWKNJKVBY4TFEHwQ3QMYDpIjRHjeZkZS4ltlCAkZRTYhRbtLZfIorCyIarS2PHnzCb/7jf8RqtWI+m9C2LZOqwBoRBn744BOqoqTrW3SKzHZ22NvZFVvDd97i1s19duc7o0mPNYbgRQpQuCuOoiioqoppNWOaexc+yIb1UVgx3nu6tmW1WIDvSZOpeKwohTOOSVmKSlfy2KLAukwYY1PuWCWq3jZfR1WWGFtLP2hrShFCxBrxYBk3bu4XRSXBa9TDyLydpJ49HC5NQpQaMTLPjl5fzYDwovVaBgshOG+W4tm3/jqglg+JuutpfEAlEeXtgzBOxdB389jhJpRMYVMvDyNCY+Tx0QdcaQm9p2lrfNejpkitnDUnTVIobTBGU+afqaqe9957TzKMswvW2ZNUrt1xcX7CarViOp0RfcfOrCT0hrZtmU0n7ExnMj1Qmv2DPfb397lzeIf5dMLOzg77+/sU1uK9z0FndzxhNWCVxhiLc26EgCd6lNICNvNSInVNS6MTNonOqHLi3xqdQusJBIhhA5aKuXGofMIoocEbPUDQJeOyNn/dBBntWo0ngNEbSYEcJBKglYbwbGYwlBrba5A9eLbsuJxlvKLJwwvXaxksftZlnMX3nlXX4LQRWrqSVDeSiEmSZTmMBvjx5RuuKApS9KjML5lOK7RW+E5Gi30vgjLeeyauQmvpU6gESlv6PjNGywnvv/8+h4eHnJ2ec7a4YLlcs25qIpq6rmmbNdbA3nzKrKpkAkNkPplSliWFE4r63nyH+XzO3s4NDg/3mU5KqmpCYQ0pCP/DGIfWVrxNgcnEszNt6JuW3Z0ZR0eG9XpNiIP/R6Sua7yfU7o5ZSkaGSELBEUf6MoJKGlQeh/xXnAcMQqsHIQc5pyj8z0Kg+8lAxs2ex89Vkmm08eItXlDZ+SsvP4Ckruq7n2dwdC2Buf2uorleVGweFUnI69lsLja377ufR9AW5cyjMyneHp+JpyKwqF1Rdc0IycBNiVIHH9sU4YE35F8YHdvj8PbN3FWavLQe/q2JvmeFLzQ391Gxj/GSAy9oCj7wLSasHOzYm9nj3t3RL26rluW6zXnF8eklFitVnLyRrZOxARBTueqqtiZzdndE8i301P29naELt/1dG1LUVTs7e6hlMEkjTVShjgnOIgY4f4bdzk/Oef89IKua7FlQQqwXCxYXVQsCkdlHbvVlNlkjtUalTQhSR/IuBKV0qipWpaW9UIEfOqupWlkbJtSGuUHx78lc3QwGmvJhLYeQkRrQ0q5fDBKnM+yTB+AQmHV5YDhQydTEE3mvejLrx1D4Hj9UovXMlgM67q3e7vXAJeRnjHJaeZDD30/ovsSG/j2dSXNpd+ZhPZcVo69nTlKJ4g9Sm/Qg1dPN6M1ShuIEnicK4U1GgMx611aWzCZaEgal5Fl88kUIJ/Y0tArioLCXu47VFVFURQYVWJtISVSEej7EmNczgo0vhc5QJWGCYAi+MRsWnFjd4ed2YSu64i9BwWlK0ZUp+9j7rEYnC3EXUwltDVop0cMxPA3ex8JIaG2HOhjjLnBK0rgISlSjOgQUEqjnd00I0fY9sahDDYj0RHWrZ4tQ4b+xPDYbV3O4TmG63md1msZLH7aken4c8MGzjqTsRPtyme1PPWVn9v8QiGkyXhR+hcR4ww6tNLgHDv1Hu+FJKbcRNisSW7egZ+S0sB7sDgrsndaWXZ2J5Kit924CTeiQSKq64xFaxG9kR6AA1QWwlEY5VBKNo6xhZzSsQej0dZiojBWrS2wSjPJWUq9bll1DSlEVGHxPowlRh+kORu0zT2YhFHyenQZlzIEBGHmXhbgVUpGqxJQDVpD2jJsslqPDWLJNxQKO75HaIVOG0ZpjFFGq1trgN8Pv5f0LMt04KC8buu1DBY/aT3PGHm8iYwmIak/kGX2rvw80nyPXF/Deu9xRhzJJ1VBszjF+07AUd4TvRVH86Sg70jGCdgLPZ52TmvKcpJPQJtPOoU1sunctBiv2RmbKeiB2WSeT1s9BgytxexYG/C+p+nlOqwptvQrNUoZrC1QKlGVIppDSlilmU9n1Dsd/XlgsVoSl55pZVFh2HDCCk1JrIOslpNfqYRVZM1N0ClitMZoTdLI40g4o7BOk3RuTloD1oJxJLMhkmlN7h9lVipqLCdQG3PlF6E4r2Irth87lCEv6k28iuPT1zJYXJdZfB4IuFKGqIbadVCPljXQ2HV6tiey3Uiz1kKuf+fzOfP5jPms5MivRxzF5qYUCvj2SWdMFsqNicIMJUuWwc/QaKUkGIlZs86TAwsEptMS54qRmTlMFqRXUKINNE0NREIecYrtoaf34mZubRAglpWSoijE1Ghvr8PHRBc866am6xp8N4gGS4pvTSG/UzuUauSUz9lUYayoZsSIRrKOlAOZlGkRnRJ9H+i9JyFjVawR5GxKKJ0nHNsNyZhIw/dzljEoYV1d4QrS8yfBwl+n9VoGi+vW57IFyBusD91oqqNg7M4/K3Ij62qwCH2P1pqdnR0O9m8wm5Wszo62JOE2vYvh5McYjC1wTrAJ0QdBRRpDSiJ1F3TmPBDxXT82VodgkRJYZVBR5fLC5B6FAL6MMYiyuM6/J49iM3gpBAFTeS94jpRkPLkzndHt9/gIPiaatmW5XAIx62i0oz+qMloc2rUR6n7wxJgh2iRQkZRBaVprrEoYpUQ/M5coA7fGK4MrUg4MihgCZmskqhQQXjzmvJodhBAu9S2el0G8jvHjtQwWz8P7X1rp2Y3fZ8/SYVOnGMeaFgaPVH3pOTTkkWV+jujpfYMyO9y6dYuvf+09dOw5/+wzFIl13XO26tAu5RO4onTSMzDGUBUFZTWl7/txrKiUYlLJ32SMoe0aZvMd2rana32uzQuK6c64kQaVrKoqR86JLUq6pkYbSPRoJady8D2x68UnxVh88tBZ6CKVqrizf4+JnjJ3U3aco9QBowJPjo84Xq45OluR1BOMLqlchbOa+XROEypC7wmxF8KcztB4lWhDT9N1oA0+GXpVkhQ0fUfjRUXclSXFpCQaaH2PVpYYpHwxTqDa2CgG1MGPzcyIZCC2cM8iNo0ZG9RKa7zJRtHD9zNJjfDTSSK8Cuu1DBZf9Lqkg5BRhSEEptMpu7u7NMtFhlbn0zcJHiPmhuZ2hmGczU24IWPI1GsiVksAcGVB13mSagipRcVIUVTjVMMZlacqjjIL+iilBEfSZq2IrA0afMAHj+8zcStp2UzKYAtLGRNlUVFUU2YxsGprdusbnK/WnJyfyTQkeC6WC54cPWV3d858Ps0jaY0ymsIW0sxMcqoPUPgYpVwIIQlwK0VCiAQ/jErza2EcgQ6Fy/IAMmkZX/UECgNJlNkHLY4hW9pel5CaaotPMvBF8s8lLmclL5J/fFXWV8HiC1iXUIDKkJQdwVd78x1U8Ozs7LC8OGe1WLOcLLh5cICOl3sYm/RaJinOlYLBCKB0wjqHdQWFm+FKD6bEWMGAWDtIAlqsyo/XBucsNpcr0mPoCX1H6FvR2Yye5APBZ8aH0RhXUJQTQJCl2llcWVAEGelOJtL4NMaMo+cueE4XFxydPGU2n2AKS1UUeaJi8X1L34uKl/cetEUpT4yiSBZCkMlKH2n7DpJGaYsy2WFdWaKSsW4kYZKIJ8skKm2CQNJoZdFaEWP77OY2wpwdSpBxjJ2/PeJutILwrIbFZur06gWPr4LFF7CupqpKKeq65cGDRyilqcopt27dptCGoydPWC1r1os1flCqigltpE+glUUpjbUGZwUVOUwHBuxE1ArlSqa6xJVTwTdky0SjobQOrRI6K3olH4jRs1qciaNZs8Z3Q5YTGaq2qprKv3JKMZlIlqFysMgZirMlk4nAyWeTOXA8jikvVks+efwQZQ3RwNtv3INcXgWfN1nSWzqZihgTwSd8lIyiD5HOBxhIazEKb0Yr+k7KPacN2srrRRJB4ascvzg2qa/pR2hFUkJv5wrrFBhp+M8LCK8qC/WrYPEFrG1UsUwtEl3X84Mf/IDFasXOZMK0rAizGUeIPH3TNEBB24cxEAhEWzZlCCmDhUwOHhbnCrR19ClhjMOVFuMqiAnfR0Lfo1QSAJYGUiT5nraraduW9XIhMoHdVkNSqVHfsigqXDnBVRXOlkQULoEtK3TTCCIzX2tVVcxmMzA6Ty4sPnS0TxvJBErL/TfeJCWZnvgMyEpaAlBKnpgSnY/0QTKKzge61tOHhHUiauNlWgwMuIirviHCTt0GZo0bOY+ct9fIGVF51LoFxU3yw5fG5NcFhats1FclcHwVLL6AtT0N8d5jtEJHy0efPOCjjz7he7/8beFcJOF0VK7g4nyBcQfjhh2k+4d0OuYRpVJxHEWSxOlMacFDaGUEIaoVqEBK5GzCQAoQZWrS1Q31ek3X1LTreuwZKJWfSwvwS8admt5HtEk4Z3HlhN0be2KYHIOMkLXNeAzphXR9T8hj4Lrt+OwIJvMpIQTxV4nDJjXoPPpU2gI9KQWCT3Q+0PaBuuuEdm4tyjpg8GHRWGdFjXsLRBWQ72kEbPaMBN5VfogWAeJBAyP4dFmmYADhRUbYOHD5OXm1gsSwvgoWX/CKMVK4EmNguVzyu7/7z7l/5y7aivnw0FvzfT/aDIYgyM4QgsjHJYUrK/ouABGtLMlmL5NMOFPakmIQ1mUyQvO2QBB9CkKXXdRr1us19WpJ14q/RwxhBGkpJze91dIb8N6TvGQ0tiwoi5KdvT1OT4+BzWYZdCyDj3TeQwpoDZ33nC8XHJ+d4UOgKAoUCm0GgZo09mQwmqTEQ7YPia73wvglX9vAAlUyuRj2bkpJhIe06IUopbLKl0GpAUsRr1X8BkaBZQWkJMJFSSuRZc3Nzm1Q/6UG9is8IfkqWHwBK/pNx90UpbClUwRl+Se/+Vvs7+7xH/7GX+PeHVHuvjg75+jJYzxP6LqOW7cOx4mITCkEMTqZ7EigyKdYCAGnNSk4tNGYwXVcW4xRFM7RNy06tPQh0K5W1KsF9WpJ3zWslhd0bStCNsWUyUTKDaXkpO/qhs50uLIkBJcbkpqu69DOsrO7m/HsBnN6zKrt6IM0K43N/QVEgHi1rPn440/Zv7HLjd1dXKHwXp4vJOlv9D4RlMajWPUdT88XnF4s0EWJcVZ6OElc7GVaAcYN5YbUJ8YYQowYvfE+FWKeIoRnCWFDoBgqEG3NOB2KKkrmkglt2ppR7/N1AG99FSy+iKUup6sxprEkWNUNf/b9H2LLiomzfO3r3+Dk+CmTyYTHjz5ivVxSr5ZYpSmM8DAGFulsuiOewSER8cSkSMkKIEsZKQeMIeVxn1YSUEwe3cpEpsWHThCauU+xPa6V8gBC7JnM5iRliCGwrpfCvwg9i+U5db1GWUM5mbBsatZNzcVygQ8J7QygidGjkiifq6g4Pz/FGkVZGFQq8MFveCBGEzopX7oYWCzXnC8X9HlkrKz8s1m6MCLj1etOdSkDNSpdpqkPpc/2kkwjbrgjAzfEalSQhmtMKRPhuITOuk4t61UKIF8Fi1/QSgqImqIq+eiTjwUeXSd2dneoqoq9vT3OzySzWC6XGKUpiwJn9ch7CLHHgLBegyJohdcdoRd3duM0CYXvO1IU0FPXNWiT6HtpYg5lTt93Y3ayTakfTsy+6znrj4lkN/OUcQ6FY7Fa0DQN3guy8uLigqfHx5xenNMFLyWM98IQ1aIDqjF0bUtdr1mvC1QMhNgLryMHrD4G1k1L53va6OliIig2WRZgjRnh7TF5EgaTW5ApPxalICoR9FcKZZz0cp733mxlCZ3vcWYDiU9akYIEDMPzy40XNT5f1jLlq2DxBaxtGLnccBkJqAXxeXx6xvd/8CO+/u47TELElQV79oA7d+7w5PFnrBbLrFFZjFwOjaJvGmIRBXCkDSlC6BVGVaQQiUqmDL6XxmNpB68MEdcJUWwI+76j6WravqNwjslkMhoZLZen1OuW09NTTs/PsaZgOp8xn8+ZzMUCsemkKdo0DafnJzx8/IjHTz7jYrGQksv7PL5UlNYxLSqqoiKEQFs3LJdLUmhJGZRljJHrDoHOi6K6CO8q/JZ+pvBfpLcxvLZWwVBaaDZfH0BU46ZPSXQ7roKyrAU1NJEjtH1WB0emSt5DjKLIJYSVz12CvOxNz6+CxS9gKeQ0zB00lNH89m//NvfevMN6rZnPxOX8zu1D2npNXa8onZgmO21GGbsQe0wwYLOFoBJuhdUKfI8PEZ+RkMNJ7JwjNG2+kKEcaWVk6j0HBwfM53OIitPTUx4+fMjR0xM++ugjjLGUE9G/mM/n7N24we7uLnZS0HUNF4szHn32mI8ffMxnR09Z1WuiMpDHweIVWzItK2aFaG2EEGjXKzQlRoE3GuccQsFPdL6nzmPZaJS4vVubm5MenZSUVSplQ+dthbJBvDehlEOpy+SwIau6urY39EBZ3240azIKFEVUiRQvlyIvCggva1YBXwWLX8gaTjoNoBWFrvj9f/GHfO+7v8I3vv41cTonsbu7y8HBAQ8++YTVaiXpt4GUdqmqSpCWxmCDIhpGX48YekIWmlHaYrQGlYT+HgI+9qDEoCeqgSuRqKYTbty4QVVVNGsJHk3T0LRrDg4OuH//PkVR0PYddV3TtQ3LBWhvOT0/5/FnD/n04QOeHD0V31JrcLjciFQUxlC6itJVTIpJ9voK9H1Ct2C1IhLpOkOPpemll7JuG5pO0JYxiZuYsZY2+PH1HDxLtCYreG1UvofXRTZq2upHPLupYxYb3nYu816QpAOt3wwyvldMk68LBFe/9lVm8dV64XreDZOAkDUoTk/O+Rd/9EfcfeM2SimapqEwhtlsRgiBuq5HsFPhZLNW0w5l7BZXwhFMwCVD0gZttEC5M8W863t83xF9t2nM5RO5LMuxvLCmwPdxtAcQ3VDF3bt3mc/neO85uxDbw67rODu54OjoiEePHnF0dERd12K6XExYdwHnSnRSODRlVukSnooAsbz30EaCVnS+QynFeesJyo7O9CEEfDai3i4lhnJhkNhLKaHZKFtd5XBcfV8GEt2wjDGjs7ogSjPlXUuwMEoLPyQE0qDzsZVNvIow72F9FSx+ivUMhX0gVV1aW47p+eOY3Oa7ijwdiUQlIzlPxLjI7/zLf843v/dtbr1zj8ODAyoKbs+m/OjjD4m9Z7Fe0DRr2r2GGHom5QQTNdo6rHFEp0kq0qpjZtN9YvB0jZfxZu4phNjjY0NMXvQtE8TpnHL3BtNyh2j36JXBzWfcmd3h8K1A7OV692ZTUgo09ZrDWyLU03Udf/jnf0hd19y6eZuqqnjj9i3atmFVrzk+OyVE0cPUtsiQ9IpoPIu+gz4T4npRL48h0NUNPnmULuhixLcd6+WCZi1CyZ2RoFOYDVdGAyFzQZLe6A0MOAuVdTJEQUvKNRIMalzD8j5PZDCggjwmbCYoIUV6HzaiwlmweVAUB2Ejmy3B5iGTHD5/WddXweIXuTIUedBMWK1q/vz7P+Tg4IDqO99hMi0wZUnrA5OqRIVI6D3aGi6WC3b3arR1FKkixohBaO199NkWUY9sSR88MXU5TRc2acwktSFjqcopylhSVGgjo9ciQSwiKQSBYcdIzBgEgVInqtKxM5tTWEM83JfGaL3i7OIcrTWL1VquzzhcUeCsUMNXPmQUp8aa7CjvPU3X5Owhbkoe32fnty1zIJV7E4MvqdUoNiNfgEHSUGXMReLqWPNy1rHtXJZIl8hiA7hr+/PEph80YC5gg954eUPDs+snBgul1P8G/PvAk5TSd/LX/lvgPwOe5of9Nymlf5i/918DfwPpH/+XKaX/91/Ddb9U63r9DHEvMcYSgkdpTd97/uz7PwBgvWr43i+9BzHxwccf8+79+2IMFAR3EDs/9jHSTFFoBVGjc9ocQp83imygED0xhtzzGBCMUDpH4SpKV2JdCcpkn1CGiEDI0aHpWohCzIoJ+iDwbR0SlTU4M6UoLNoZ6rpmWlU0TUPpLui9Z5DkiyBaG70gUlNKuMIwKROkSNv3TKxFaZUh3u3oMRu3ew5ZqIckI1GjN8FifO3VIH4cxgxjWCmJePKl92qL2ZuSwOS3BX4TW/2PdLnEiVm2WUyNrsdavMwIz8+TWfzvwP8E/B9Xvv4/ppT+u+0vKKV+GfiPgF8B3gT+P6XUN9PVXO81XlfVw2129zbGEZPms8dPWS1rHj18yg///C4GxZ/+qz/BuZJ7d++gjKLz0pFfrJdgNK4qKSiI9ISUcGaysUfUNm8oT6LPehB9/p2GsiwoXEVRVELdtoU0CgEyA1RwjrKxUlT0QQyWoiCWsEbhjMZEcNYwnUyZVRPK0nF6eopKSkR7QwA0TSt8lC5EMW1qGpHpu7FL6SxoI0hKJbL/Xb5e2IxAlRFJPW2zi1lKDCXg9oYcs5CwpfKdkjQnQ3zm6B/8ShQIPkOJ4lZM8VJTVOuNcdH2U1wdo77MZcfV9RODRUrpN5VS737O5/trwP+VUmqBHyulfgj8m8A//Zmv8BVcm96HHqX8tTK4qiDFyNliwWKx5IMP/lQwFTHy9vEJ+zdvsjOp6GMUJ/G+wzRrZv0M4ww2ObQelLl8rt1FwyFETwwtkUTb1oDO+pmFUM6LkpAMRZbv3yAdDYaA9wlrLG3o6UKL73u0NVSzKbNJb0NqIAAAIABJREFUSfSdeIZow7QqsYWjrBzOWKzS9CnQt56IIniP7zx9DDRtx8ViyaAdsb+3g9GWspzQe7/hx8RIUjKHUCZLDbJhk4ofyLPw7ZSG1/eKLeGYQVy/mYdNbrazihwIrpMcGDQvknzhmet4FdbP07P4L5RS/zHwe8B/lVI6Be4Bv7P1mE/z155ZSqm/CfzN/PHPcRlf/qWfkfDdLO+96HrGJPaEVYXzgYuLC3rtUSownxQ8fPKUvRs30HfewMfA4a2baGvoQseqWRGjF3yCmhFDT1mWmOSICkKGc/vQicVAaFFkhawkhYpKoK3Cx158PnKjTysFCnH6Qohexmh0VWCzGndVVTRNTQh+NO0JvadZC/W96zr6pmO9rkV7IsrfvVyvWa8bUfVKYpJ0Y3fOfDZjNpuxXK2BLe6F5BXYjLPwMZBCECBVXlmCIsOxN+xTg9n0GVIag83VnoUx5pkMYih7Lpco1wvcjKxTozayi69I3PhZg8X/DPwdJHz+HeC/B/5Trr7ysq59qVJKfw/4ewDWmlfk5fzp1zC+61pP8GIWZIsys0cNKURChMdHR9y6dYvDw0PZLMYKnDumDKjqKK3DWk3wPc6ZrAKeR459Q99nH5KURrjzMJZUyhOS8EXEdtBjbUHpsumQUrRNQ4oRZRVOieBu13Xifp7p6CkF0cZYr3ly9JSnT49oO9GgqNsO34s/7MnJGSerxdiotFrQpYWruHHjgMm0oO16zKgrkf8pRIVcazrfjpMQY6T5qpRsZqOH8arckjrpz1USDGPZsdGZ1KVMZFjC8A3Dm5j5N2nMLEaGKowGVMBoqfgyrp8pWKSUPhs+Vkr9L8D/kz/9FHhr66H3gYc/89W9Ius6k+Xxe1H+aSsakau6BgR2HHUQRqkrWTU9f/L976ON4S987zucXCyYvnGIy9lAjKI7uWpWTIodTs+OcFvK3UNWoKzBaFHC7ru1SOf1Hq0tve7weUIhG6bD96JiVRUlZanwbU+zXnJ8fs56saRtW06PHokTWW4ihhB4enzEw0ePiEmGleeLC45Pzlk1dSa8CaEsIXB1pzUGTfQyTp5P56xXtZDmQpbD0xqVcRAhZz7kk98WDkK65L4GyATGOenhsAFjJcQe4CpFXduCFAIx9pAQ7k3OLIbXZcxWModGJP/8pa/FFKUMDJebnNvzl2006fD5l3n9TMFCKXU3pfQof/obwB/nj/9v4P9USv0PSIPzG8A/+7mv8iVfST2/DNHZtpB8Kg3w42Es573P0w3PYrXm6PSU09NT3K0DQoyU1lEWVijUMXt0uDAGCDCgEjHILIE8qhQRXIXXnuA8xjha1gxSc9YKn1OAThCi4uT4hIuzc87Pz6mXK7qmzQIxIaMcRYin6zoWiwXL5QqP4uTsgrOLBSnB3u4+2hqi0tSPHxGCHf9mjZDdhs039Ct8GJzXDMq4cWMy9i425LNtgZuNexvj1OVqeXH1lL/anExajXT0lEe1Q6KwDe0eMg+bM6HhHR+c3LdLkaQGkYGXa32e0enfB34duKWU+hT428CvK6X+IvI6fAj85wAppT9RSv0D4F8BHvhbX01CXryE4yCCLrA5EZVSo4WAuKiLfP1yueTHH37Mwd6NvMlKymICSTaYweB9h3MCgFIIpd0ajTaKpllnPkggBmlg9r3I6J/XJ+zv7zOdTikKaSb6XoBXTx9d8NGPP6ZerkhBJil6C0XZNN348eJiydnxGavFEqzj5s2bvPXOu0ymMxarmo8++ZTHT588s3ltIeC1rutYLJcs1yvqtqEPHh8VioTRItsXSGOp1Xl5nYY+gtZ6BFIN5cSlKcbWuq5ZOSwp0eT9GAh8lzglW9dvlR7Thu3nGJGmV4Bb1xXnX/a26OeZhvz1a778v77g8X8X+Ls/z0W9autFN8BQjw89hE1afJkhSQYQrddrHj9+TPftbxFCpI8DqMkBTWZsdkynU4yxwjjNY1JrBD25Wi1o29zEzJaEArtusFpjlCK2PYvFCUdHR5ydnbFarFmcLdAoppOJ+J1iCDFweiTQ7wHLcHFxwXrdULqKt99/n/nOHto5Vk3L6fmCvu8pjGUFdEGCjJzIkaYV9mmfes4WF6y7lj4G+qSxSkabQhPfQLpDCKMOhTEuB+AMI0cCSUgbnY7hdY8h8oySr86ao1FGpr7vcqNXj7t5DEJ58xvUJbDY88qJqKSsubpeFjbqVwjOL3glJfTmQVj2eTdJSgltspWfBpX0WGYAnJyc8O69OzkYgLIqK2IZ/IiAHE5+kNGkeHxcXFzQtjVd048pv/eBGAP1SnxD2rZltVqzWCxYr9f41lMYEQyOXRgbjzFGVqua0EcGlmfhHG+9eY+9vT1u3L6Nso5FXXN8csbibEGzriW7if2I4NRaE5WYBYXY04SW08UFbd8RFEStwBlMVYyvT4yy2TevYRrLkeExIYSNMVBen4cZOjY6wybjG6cyOYMxozjQZXLakCGkK8+ZLzHfB2y50X/5AwV8FSy+kHVtg3PoYwxM0a3yA3K9HGLu8OcbMzE+9pNPHvC9b39rQ51OJqfgFufsyJCUKYXYAIy4CSVuXSH0rFYrFosV6/Wai4szqmo6XofNXqnTssJOHLPJHKtshjzL97XWTCZTKaViEncx59jZ22M6n3G+WrKqG85PTjk7ORUJPi2NzEhCW0NZOspJhTYGHwM+9PS152K1oPV9xlVYirJktjOnqiq6rsM5I41hhrKtJQSZ0Jjs8aqUgZAh6plePr7GW5yNYYUhIOTmqbZ2xHkwTEiMZF+jpN7WqPXqW31dGBjHq7xcoK2vgsUvYF1lJEgAGKwR5eYfTulBVNZaAUwBLJcrHuepBUG69DFkY2atKW2Zm30Woy0xZiRmEA3Jsizp+4q2bQkhsF4vubi4QKXEG7cOmc1mo1+J9340N96d7Ik/SFa7MsZhlGZVLxGHdulvFKWV3xECKUiTtm1bmqZBIQbI0oAE5wqm0ynldIJWCu8bQuhZtw1120hzUxu0FSOjcjLJr08ipIjakv631uaAEdCuyHgMSyJANpgeMo9hqnF1GrLdRxnKvzGLQcqIgTcyNHVTJpZdChRf8snGz7Je2mBxtRH1ZV7ObzW80sZvE0BpTQBR5Ca3JhAQUVIVwXvWi4ieGGzh6IisQ4syJd//+GO+88vf4sHJU/Z35ty5dZOL1Rn7u/t0nccYhdGCf1BWicuX1lTzXaK29D6xblp2bwTKSYUtJty+fx+nRTPTaiP4hNws7OsuGx03rEPIxkVJ7AN7AX2F4Fm3a/q+p/M956sli9WSo7Nzzs5POD45oel6ptOC+exuPsHFrjGEwOqiZrGoWa1rehRBOTAFs9kuOzs7GGc5rxeklChMQfBiQpSS2EGWWsakngBWEfAE01O4aZ4YyQYPcZgYXbl3tCJ0fpzQOGMz92Qwh45jnyKSR8BZEHmwREwpYQYflNxrGuHnpJGfMvBMhpUy2vbLul6aYPEyE3DS1Sba51gD8lJpJUK9VmOzcrUOApR6+vQpi8VdJkVB3/e0XSdpfAZUScaRsFZGf4Nc3IhEtIZyMmVXa+AG0+mM3d1dea1jysQsAzFycnRM4Ry71RSVRNF7vV7Tti113rzjRvQdbXY67/qG5eqCs/MjLi7OadoVSluqwjDbv4FSiqbv6LJYsPRLOqIYBGCMpphMmM5m2LJAKSGdKUSDI8WIz2Az2IwoNYMqt+h+qiTaIZIgCInvumZk9OHy4RPTiHJNAxpzCDLxClFsq/lpks6RP4yP2cZovIzrpQgWVzOHl+0F377eYb6vtwhlz4MDx5QwSpFUxCdPSLmPYGBVrzk6Oebx48e8+87bdL7n7OyMG3s7Mm0oZGMoJaAnkzQpRtq2JVc6WGuZTCZMp1Ocs0znM6bVREoWLxs3eI/3icM3bnH0+AkXF2cwTFecZVZW+EVuknaRrl+zWkkPpG5bnhw/Ybla0/Yd852K3f0ZZXYr64xMYlbrNUenUqaEEDHaYVXCk9BFyWQ2pawKUpJ+hC3spimakniOBORv0xpnLElBCP3YI9FZAGjAXyhlZBx9JbPo23Yck8YYib0IDauYRt/WgQcykMlCimP2NdyrcQwkVzKHLcj58Fwvy/rSB4uX6cX8adbIfnzBms4qSal9h7MQo6GLgRQ7Quipu5qj0xNuH97CJE/0PfOdKSoyYjTQFrzH+yhq3l7sCxNgbEE1laBRliVlKdgMHQJBe6L3mViZaH3PbHdGOS3pGoFzn5+d0Dctte+yR2r+lzkhYnCcKCaOcl5iCifcEmepKkelC/oUCanAXIiBUd8FSe+VhhTFZb2Q6+qiOLqbKKl6FxtUVhkPuYcw8EZUQhS9g/R/ks59h5hQuTFLDgiX3peEPEbnBmZUqKTH7EKKhzSOe6OWvolAv8W7RMVNRnFp2pFE3vDae/oFwL0vy/rSB4tXYW3fHNc5YI2P43Ljc92u0QmMFb9Q73ucUThnePOtN7l16xbaGE7PT3DmFtNqwuJixe5sThc6wRyMICI/ksNCkvTbOScqVU7jigLrig1xymg0FoOgTLUGnCGEIKQyFYkEGqt4+Olj6mU9NkyJAr+2hWPmZthSlMmVAZ8EkVpNJpyvOhZ1g0YEeJTSUrq0nmQNnoRJG9EaiDgn9HWl9Ii1sNaiVRKaekr4TsoSay3zapLRlJJxRCVZkdOGgKKP/aX3wCotVgoq5pLDYHL5EXOPhvwvxI3PidZ6HNEGwjMlx2Uy3LP3xcuwvgoWX/C6Wru+6IZpmjVWaWxZyibViv2DA+4c3uKbv/QNqlLhm4ajkxNu7O5hnOVitWRaVjkwiNepBKi0Sa1j5okY6QmYrIpljJz8Ohm0lvGhU4qUM496tSYCriyYkEgKjLMc3r7NarrMdopC2hr+vrJyaCcw7Eig61pR6C4KfEzil5JZrn0M9CHm5q8mRJn4tG1LGz1BRSazqcDCUaQ8HtZJGsUxZxQ+ZPxGBrZpoPeCt9D58cIITc9kd13bispYLiNMtOP7dFXkN8aYx8uSJW4fA2KVmK4pOaRf8jKulzpYvCyR2WxTqLeuWUaFopI1SM5vf382ETzBrcMDvvbO29y/d5eDg30R8Y09Tz97wMPHj1AhcvPmTe7du8d0t2RZr+ljYjJJFDYDiIwVnkQwhNBv2fQl4VgoqNuAUZtaOw4AEaXo+gS2oDAF0UFUDUWyJN1ycEtzcAshgg2jSWRkWtdr+r4lJg8BnHHYlEax2xhF8ev8/Jym7cUQWUNI4hbWNB3rx5+BUaRMTrZFNf491siItDDFCKRSIaJCxDctyrnMTBVGbdd1WO3yqLd/pl+0Pl+g1BBE4qVgsb0kGCjC1Y0/BErNCIaTn99+0CZgjM97pQ139TD5MoC3Xupg8bKs7XTUGPGxGoVmc9rfdt3YnR/Kg9V6weHhIf/2v/WXefPuXebzKSF46mZF37cY5yiqkovTMxarNcpo9vb3uXhynGv4iDGRypXYbDCklZZeQm70AZuNg2hvppSykEweCyqNsyW+y9BxwLgJ1XSXGCNtt8ooUC+WgyHgO+mPQG7yJZ0zFzVmN4K96GRqk4StKvJ5aZTPQ4nE/wAESypSX6y2Xj87NiwHfIjONHCtNZpEYSydF4yHisKLkZIpjfob40oBsrivThGlN9oVl9mhmaT3zJstXxcf1asZhCKNQeJKsLg6Rv0SHoRf+mDxZYioP++6ehNcxyEoy3Izi8906H/jL/0l7t+/z9fee0+MgOp15nD4jdCtdTRty/lyQUiKopqys59YnJ1TVTIebTuR0xO+iGFde+g1yQoRSxsjfYh+0xjVhgzsMmM6P8CaVVIiwZc3ad1cjCI3nVkLXT1GdK8ZjkyjFFo7IoY+tMQQaZuepu7ovMj0+SgmxynraiqlUFo2ZkwJouhBOGtHPIJKEH0ipZ6L/hznHE4PjcuIzQ5nSfcopehanyc3HtAkt1FeBzLGBDFBRn63UkP5OL6jWwFjS4FrvE1DnoIMP/DsiPbSff05mptfhj3wpQ8W8GzAeNkwFyOlGkYl6m0xFa019XoNSnHz5k3effdd3nzzTe7e3sd7z+//7u9xdPSEalLy9tv3OTi8JV6gweNjpPOetunofWBdN9x54zbHxyes1nXGKgi4aqC7F0Uxjv8gorKmhrOGummkaejK7AwWc2mfqMoJsjmGOl2u33QFRiesCnRbBj/agHOWGAMG+Xu99yLN10b6qGi9p2572q6nD/ncHYhb4zLoNOhvJiJ63IdK20sISxVFlCYGwW30RDF2LwIpqrGXY5RAo65mFkOmt+kr5Y28LZyaFbYEYDf0MfQlj5LL7NatPsWV0enwNcafvaxxsfn6L369FMECnn3BvgyR9vOuPmyChTQTNy7lQzq+s7PDG3fucHh4yGQyYVWv+ae//aecnZ0R2oa6XlFNStq25vDsjPfef48Y2Rgbh0jrA+t1gzo07N24wfHREW3bcuvgJtpp6rqWTV9Vcl19T5MnGEopzDw3OLUoXqVBcEaB0YaqqhCGqgj3xphyKl+QTCIaP24EozQ4R4wOTSTl/of3Ae8DTdPS9Z6uD6zWDeumxsckLNCU/VtBdD5ySWSyZmbycnIrI2VGZHOqpyCq3yomDEk0MJRCJY/WYAqLtWKi1HWeGC5PQ0Lvc/mTqe3DNy4JUgyqW2ELcTlkBxuuyvjwrcbmNqpzKEW2JyqDJuuXcb00weJlXlfl2Ib/h3JjNpuxvy9ZxMOHDzeHWL3k4vSMwkm3fVJWvHF4m/tvvzWCjZLStH1gtRbgU9KKp8en3HvrbapqytMnjzk6OWY2mTIphlInO6P3/RjIjDas1xcy4lQp+47I1KIoKoF+ay1ZRlQ525Ab3ufNOwRAqxXRaUwytF3edCoSg2hVtHVH1/SsVx2LZcNivaZpOrwxoAwhRqxAEhi22YDGVGgxQ1ZSkoidYPZBzb2YlAKohLOWonAURUFZFpTlRNzRlGG1qlksVvj+cgmwIfTl92srSKgRRTdkGxquQLRVpumnrQi23ZcY1Lrkd+S+it68dgNxcLs/8mUpxb8KFl/Aum7eDohnZsZBdF0HSgRv6rah73tuTcoMmJLO/8HBAfv7+1RVxbJejs/X9z3n5+f8/+y92Y9le5bf9fkNezpjzJFz3qH63q6u7rLbqO320HYLZJCNhCUk4AWEEdgv8IDEAxZ/gZ+Q/ICQWuIBIySMhCXTwjJGNNBY8uw2Xa66dW9V3SHHiIzhzHv+/X48rN85EZlV1a7utruyqmtLqYyMjDhx4py9117ru75DuanRJmFTlbgQOLlzitWGsxfPWK/X6CF417PZrHcnoTGi3AwhsKnWoIY7YhNqe8U6wESCmMf1cpF6D33nKVcVSnsC/U6B6b0jBGFAOtftvraPAKh3MF+tWS5X1HVNHzwhaPyNx1SkaQfwCh9igpgDrQIxrCC6fst3iCuW4AhaCXejKHJGgyHHxynD4ZjEZmhtaZqWzVr8Nc52JpG37vKxsdn6bCqlpECF77HyjgVjWzJ2fIrAax3JDrBVW5Me2ObXbouF69/eEfv3abG4PU9+b3Dp+1nh7fwTgzzObQqwUmpno7brIBSYW0QcHe+Kzjka1zIcFqBhtrqk6zo8mjTNyEY5Y5WjTMakSPnSe4957733KIZDLldzJknBq82CrvY0ZcOFe8XZsy94dPeE4fEJ33rxDOUD0/GE9//gV+mblvnlFavlgs1igetbEq1EIZqku/Fodr1iOBwyGozF4q6VlSNJT+9q8cQMcucMfYgU6iWu83RtTd/W9GVFWcmGRBlD33Wsq1JS3ZWnNo6Fr/j81ZKLeY1TI7JMUTUNASF0OdeRpIFhUaCCo6lLfBc3J9qI5sVk+AhwJllO8IHOOYwJeBVItCIfaoqxJh9DUCVtqMnMmPHegPF0CuZ1zML3QnpzrcP5DmskslG2RNFPRPldYZL3WVih/tZ5sANg3zDolQKd3hTqW4Y8sna+Oe9ue2jcDjr6YR2/T4vFP//4fhZncrO4OcFu26X5W5ZqSim2ePrt1CtJ5dKy/dAFm82KYlgwKka0bYsyCdPpHpPJhDshZbWc83MffInpZEhdVmyqil4FVqslXfBRKKWp65rrxZymbcm9F+1FVbNYLOjbjr3JiOPTU/I8pVqtqPqOLkSz2VSwhtRm0UOzZxXW6Gi7b23KIPNYle4Mhl0vM79rO5xvabuapmkIrqftO1mLtg02SajahrKS7sEFz6aU57XZrGRzokDH1e6Nx0NkWqYGqwzWKJoSmqrGJAkh9MJsbV282DxaK2wwaBNQOmaoKr2LBdBakyQZg2KA62E+n7NYLF57f5Mk2fmiKm0ZpKlI0UNPH7EMucABdLQWUPE9VjfErTiOfPeZdLPufdO5a+v49SbA+bYcv0+LxQ/AoAsa9UZ3EW51JLep2bfNbfztu0gsEm13A6KdnJyQplZOSiM0au8d2iqG4xHD4Ri0tPyDTc9kPOQP/cGf5+zlM87Pz6m6hnRQsFyvaXSgrmsZS5Yd19dzyqZm0HXkWYYaFHjvWa7Fym4yGpClOSd37zKf56yXc6q6oek7IYXFbUEb6dJaa4ospyiG9J0ns7FY9MLh6DvpOpTucV0nkYnOy2P0XZSKBzZVSet6kiwFD3XXMlsu4uglXAatxTLPeWFZaKWwWpMnKXmWgOspNQTv6GF3Zzb0BCPAplcQgviZBtfjeuLo1NP3gFHkuSFNU+abFWdnZ1xezl97j7eFZ/dvIxsTYwq03gLK8THDjQx9O77cjBDqtRvHrgAEIngcXisKgl91O9Dz9vETzOJH4XjTW+C3GCW3b+hO+6GV0JLjSb09Do4OKTJJArORBm2MxiRxxWkTurZHB3BdzcO7D/jwgw9oqzWL2Yy6rqGXVeR6vaJpGorhmLquma+WVE1L1TYMwzCqSZNI2lozm83Ym0w43t+jGAxYjUbMZjM2yxVlXeO7/rWT3hojYCaaLBUl6nYDI0XDCVfKd3S+23Et6rqSAqkUZV3RdD1oRds5rhdznr14zrMXzwnaY7Nk556dKL2T2HuvyIuUosgYFBlWK9JELuTr5ZrEatLUisW/2m5mXLxDi1weJZumrE1wbcBmBuUVvuupNhvm19eUq/L1tzxeyNuU9dQarM0YDofkhaS1NZ0oZFerVdxEfbcn9Q7UVjejigDL0Pc3q/PbnUWIEYlvnldvy/GTYvG7OLa1fts6b7sKAchu5tEsK5hfy9euViv6NmU4HJKR0DQ94/EIawzrzYaqaug6IV0Vq4YkSdifTDncP2D26pLZ1TWLusJbS7Wp6HtHMSiYGS2A4WrFtOtidKEizTKK4RitLXVZcRULznQ8YjTdJy0KrpJLrq6uaNp6xwExxmA6R9P2LJdL8jynyAYopaPpzQ0T02goyw3r9Xqn8/BeFKPL9YagoO47Lq9nfP7kCWevLijLEpMVmFQ2IDoRk56203jfkVjNsEgYFJnEIWpFogNaBZquJ0TbvNoovBMg0miNx8kmIwTiHhIVwFoJgFYRRG6aRjCiN3NDIjN06/1hVCAxiP9GnuMVFD7FDQckiYlmQB1N1+0yV0IIBBWB0e9xhwm43dNT/vaIqna08LepSGyP35/F4vZ48dtyJoq7cvXG2p0bYEuCcPRr4JW7dec5P38pKH2Wk2aW4TBnvRHmYdu2bNYVZSniqsfZhDsnp7RNjatbgu+pyzVnF5fY0YBluRYDm0GB87Bar5mv1jzUMk40xlEUBcPxiCzLsGkKWvH8yTMuY8LZ3mTM5OCQfDRmfXnBYrGg6xvapsPfsu4rioLxUMYVEyXess30bFZLqqqSSAEtArCqqqjblldXV9Eir+VyPuN6tsCHwORgny7qNoKCoIR16UKP0kFsBNOENDMYE82GswSlhqyrGtBUTUtiLFUfk9gTyUNRbAXicVxBYXVCYi0aI6te/72NaPI8x1i1KypdW2EN4oulAyaGNXkdSO0N+zMoBdxQ9r1jtzLm1nPZblVujyE37FDRw7ytx+/PYnH7+OdYmd0+naQ+fO9Nyq51tzZKqG+o21W12X1d24o1XV1t0BrWazk50zQVULASvCBJUg4ODviZD3+acrVmtVrRNW30W3D4vqfelCTDYjfP1nXL5ZWY4lZ1i7EisvLKoIwl9Z6DNGO92rBeLXl5ccm6rNnbmzAeDjFHByhrKMtS1plNi6fGh8DVfMZqtdoVitsZoH3d7FiqOrE0dcdsMWe9XvP84hWrTUUXNR82S8kSwWwGA+F9+KDog6dre7qukZHDGrLUUqQJidWYyEUoMstyvYFYXPTEElbgnKhkQ/DiuYlHBUWIAUh9JzwPryTseKu/eRMLODzaj3d4KXj9Mj6f1DLIpbg1XYurOrq+IUQJfZ5uX49Ix9+eGrfPrVg4tLIEddt270fj+LEtFtt0rNtvSAgheiPcqugxMHd3fA+V3259tTu5bnCJ21+TWIuxYr7rnL/RgNxCw73vBQsIniTJ4lwta8xEKyZHB5wen/Duu+/zqJhgrOLy4pzF/Jrz85eA54Of/hBvNVcfN/Ra0XuHtQmzxZKPPvmYn/7Zr7A3PcAYS9N2aJMwHE8wiVjt3X/vPfpGbPGWixlfvDyjrWoKHXj33XfZOzne/X/XNoQQqDYl+J62Fhv/uq6pmg06wKYsd52Fj+NJ2bSUVYVOE6aDAfmgwKMp4/fbNGF6MGaz2dB7eV/qqsX3DeV6QZZm7E0GHB3vY5RG4SkiwWpdNnRONj69h3ywoO88y02J91ZGHBRGJzRVwxqFO5rSlD0q8+STgslEsTc9oKx7uLUQOTk5om1lRBkNMmbdhkBPVa5IrOLRO4/F+Gc5Zz6/JssK0qygKNLd9sMYQ9n3aG1ey051ztH1beRXbM874aPI9uXt9d+EH+NicVviexuN3lFvg7Srt78uhCCp4bxOujFzmTSrAAAgAElEQVQSMxUJQzfoNz5mRChJGVd4+v52voRkaehbM8tisfzBfoH/K/793/z2fu+/93flz4/D8Y2P/8U91ne++MG+znuH1aATg9aGe/fuUFUVxhgGo4LhsGAymbAuN3zx9JlI3pOEEOxrfhfbc24rxtu6m+eDYkfKgi0LduuypXmbA/x+rIvF7bXW9vitEqMIARO7EQmniTLi+HjbLmSbLbHVD2glqd1yskQqbxCjFWsNWaKY/cv+hX9y/As5gutQKmCNrHOD1kz39zg6OuLBgwccHh4yHI9QRvPRx59EGwAxD/YeFJqm72ibFu9lrIKEJDGMRoPINn39BgVvJ6D55vF29z2/i+P2i/8mv35r4S4y4pvcidsaDsPN7nyLkN+MLh7C6y7Q8uNEQJUmhmKQsbc/4c7dE9595x3+rX/zX/u9+LV/cvwujj/8r/wcINsdjQPvGE8n7O/vc3Jywt27d9k/PODLX/4yf/JP/kkGgwHOddR1vQN3jY0mvr4hyxMGw1yo48qTpDemwVsB4G578iOAX/zYdxa3P96ZzWCRccLFz28ZgNvNxa3kKnXjYxBa8UTYApjy8W1U3WOs6DhGxYDj40NOTk74ys/8NPP5nH//3/u3yQcFz58/56NPPsb7nkeP7/PlL3/IIBMl6OnxHb785Z/h/fffx1+tGBY5f/2v/Q/cuXPC/Qd3uVrMWdcNLy4v+X/+4T9mNl9itaFcbZhfz8izjPvvvst/8hf+AtmgYDAck+aZ8Doymav7eNdTRDJQF3NPnaPabMTGrqqp61KS0nu5Qz64cyKGwNHDs3ct6/UaV7c4F9PPPbgAXd/T9D19FE61veSIOOduaNG+o6k7mq6lLCs2mw1XlzO++OILfuqD9/nKV77Cwd4evWu5urri8tU5ZVkyGu2htMF5GE33SIoBKM31bMXVxSUvXpwxu7qmrctdMtl4PGZvb0+o7JMxaMv19TUXF7IBmkxHKLUnmpKt/WDvyIoBzns2VU3bdxwVQx49eoe79x137twRIDgGPYlQLcH1nrxvefDgLoeHhxIKdXbGarXCJhLxIExY//oWTb3pqPV2HT+2xeLN4/abskXS8exmRBXUjQN0xCa2uOQWckishbjx4FaR8IhK0/W90Hy9I+QZRVFwdHjIIM/49vkrzi+v2KwrNtUa1zaUTcl8PufTTz/lD/zcVzDG8PL8RczjqHk8PWKQizDs/sN7VF1FsGAyw6YtCcqTphYVNME7CB7XtqzmC8rNhjzP0UrtnKMg6g8SjeoNru8Jwe3WvKHrKIZD8sEAP+6py4rVakVdblAqcHZxgbkApQOJ0aSZ0JaDcxiTyKZDGXxQooptJae0944s5LhIOuq88Ei6qowK1kCX9KRJTpZlGGMYDsZy5w6e9aoUoVxdoYxQ5VGapu3JiwKbZYRITR9Nxhx3Dt87rp0jOAdoyrLGmA1121HWDcoY1us1ddsQosHuVgCnlMFEHd26FNLWyDlsmrN3cMBoMtnZB0qim2hmxmO127DcvXfMO+8+4O7d+5L2pj3hRU9ZNfIztBcpviKqTuF7kDffquPHtli8aZaz/bd0FoZoxhR9El+3ONMBdOwejLpRBGaZ5IBucys8UVvhWjabJlrOKVonm4SqXFNVG+qyoqpLXjx9RucdAUgzi8lGVNWGZ88qvvqzP4O1lqZZce2usNby8OFDXr06Y7I/QScWemE69n2DR0RTXdeho4eCQdF3Hcvlkvl8zniyt7t77WL2FGRZIlb7yqOdnAIqSCixSaxQp73HJJIrYq3GFQW+q7i+vuLy5RlluWZ/f58H9+9SJDn5cECeDTCJpXeBsqmxVc2q3EQA2GISi3O98Be8o+w6QioKVuc8wUkymdaaPJcYhNVqxWqxoK5rjJHZfzAYyJYnkdc/iWSmNBU6Ovuyfej7nnK9JjhPXTe46I2RFnmMV5R173A4ZDDISdJbHhpIvGKaSmSkxDnKebLVkzRNA8pIpGPsKJVS5HnO48cPefz4IXt7e0DPnTsnDIcFv/m1r2PMDbgJMsKKlkgK29t6vDXF4s3AnW1jv9tmxK8JQZyStNaYWz6Gt/n5QBwnxMO+94EQV1rByBvqeo/DEUIXtxWyEtU4lFaMhgXDUcGoGJDG4tDGIBnnOpQyKB9oak9dK5zJMFZaY+c65suSb332hFfXCz794lX0gVQcTI8i668hSwxVU1OWPfPrhqODESfTu9y7c5df/Pk/yqhu+N9+/e/yla/+AhfLJdlgwGpVc70oGeZj/HpDOZuDMjRNR+2dvHD1hidPPufw+IAkNwTVM7Bjmr6J62SLTix5bLedc4QoPqvbjo5OJOEqI81SUiAEz3J2wdGoYHrvhPnVJS9fPOMffePrvHv/Poccs59lFDbHKU+ejCjGY8zK7FidBIXz0HeB0XBMeiIirdVyjdeGul9QNY6gUmbXa9rqKeVmzXhYkKVDEtUxLsZYMrxOwPRUmxpjUorhkCKXdHe84+7pHRKlef70OWVZ0gbFuqpJkoTQNLi2QxEwRvHowV2KgXh2hOiytXXQWq1WpGnKcr3iYjYjf/Gcr3/7O5yfn/P1zz5lkOVMDvdJjIbQopUiTeFnP/gSR0cH3H9wl+vzJxzup/yJP/Yn8N2aJ09fcnl5hcWCFsp6zBEg6O99Saq3oO14a4rF9ztuc+dhC1bKJsK7m83GmwYzKhJ0lJJfcXuHFVdIwSR8cFHAZMmylDy1OyR8OByQp9u7hfzsRJtYmJzYvMU7ZppCVXaRVxHBUqV3NvavXp1xuLdPUQiBShynFEErqqbGWstqteH0+ES0HkXBcrlkdn7BarWiqirSNKWuWvneRTSZsSkETe/8jrqsrKGqGxaLBavVinwwwKaZaCgiL0QMbtQNVqMUXm0NbbaF10SsRsa0vpcs0c1qiQ7I+nA13hG46rqmLGu6ztF3Loq6Al71gpdYGw18lQQeNT1OO4hZoSCRiJvNRkhrZUWWJq8xYZMsi6NJDFXWCcG73R1/K4az1go4OR5zfHzE9fWMxfmr6DUqNn+djwY5QfQozkmhkVH15v3rXY9znqbr8ChmiyXL5ZL1puLe6T2yLCOxmq5pacoKjGIwGGBtynpd8s++9g2++OILPPDo4WO+9FMfslrXbNY1VdvFUfcGSO9/gln8zo/bHYPzN0YkXgVM/P/b24pd2rWRQBwVvAiVtLTfw2EhBiyd0KeHgwGjwYDxeMhoWOBct2MKys93O0MXpQTp9krLnZcb1qa1FtN2EqdnTUyvEsamNenuJGqrGmMMnQt0dYs1CUmScHFxwbsPH9B1HScnRyRG8fLlSzarNU1ZMdofs2o3KEO0lQu7i7BvO7wTvYZCTvKLiwuurq4YjsckWY5NEjCid9gWLa00WlspqjrgtMzrygRMXAt7r0WUFUlOW2JbYnOKoiBPsx3OIExJMfLpg4wBdVeKriQf3oQaGSN0aGR74L3EElZlI9qZqC3RWpPkecQBHDbJhIodJHowKI3yNy7pSolDuGwcxAR5Op3ifeDZ+asoP5eiJFkj7MyPfTTRMVqyVFAKnEZrQ1VVLFcbLq5m5PlTFst1BLmlo+uaQNs0QmzLU6xNuX/vAevNis+fXpEVQ+q65tmzF0z3jtjb2+fyYkHVrHYFuu8dQYE2P6F7/46PrahJaY1vYq7kljux7ToU0ZnoZgWltUbp7SZDBEjWKNLEYIMj9JpEZzy4c8pgKDNsZmOB0dL2Od/hHDtmnUZs7LxPcH0vd0ot/hZpZum6BBd6jNEoLW7YWmu0Fa2GNUYuWDRpmrP1kfS+5+XzF8zfe5fpeMJoNKLvJU/DOaEd20KKSllXhKBwrSOxGWma44OmTT1d5Binacp8Pufq6oqDoxOK4Yg0y0hUgosGLsYYbMze2CaEK1Kc1ygt8/lWAbrthur1kiTJMMrTNhV4xXg85s6deyQ2AzRdH4OAe8FTri+vAEjSnNFoxP7+EUVR0LWOVd0KHuLCThpfR+q4NlIA8izFRmk4SkamJM2wWoM2uOBpoxblO599znpV0tS15LtG4hxIYTXG0Md1pU4s1hj6XgKcuz7FmD66hqnderN1Isdv2xbjRNG62VRRXq9vzjnnwHu6riD4Oa3zeBRd69jbOyDLMoajEUpZ+g6qpqPrJMDamGSXnep+lDsLpdRD4K8CdxAk8FdCCH9FKXUA/DXgHeBz4N8NIcyUzAV/BfizQAn8+RDCP/mdPsEt4cVYKyduH0B/dzScPFlAy6jhYiydMZICrpXCxD+jQcYwRurdOTm4cSEKnizmcbq+FZPZW2vVgCXg0CqjN4ZOOZEbo6JmQokuIUiLnyTyM5LU0LmWNB2SJjlN05EkGVluYutdsV7NePH8jMOfmYLvmV9fUW5WpFazmF/jcOwdHewMabbiNB0DirIso+k7vANjNJtNxWK+YrPZMG1bXCwQyopXRqINQSeRjryNLDQo3YsFnnforiOEiuCsFMNqQ1EUaDxtLYrY4+NjTk5OaJuetu0h5pIIqY0de/Hy8gUKzYNHHcdHp6KFWfZsypq2c6AMdS0sx213KF1eTppa+q6JUn+5ODNr8VphlKUtSxbLGV/72teiAY+8LnmSMxnJViUrcunAQh8Tz0T8pZSkuCdtgtFbNmWK0oHOO9JUOpu6rqmbjrbqb0yE43ZHFmqK0Hs265JqU/Hi+Rn37t/h+PSUq6tLRuMpjx494tmLc9AWrQ3WpmiTEHB4t+XtvL3krB+ks+iB/yKE8E+UUmPgHyul/g/gzwP/ZwjhLyul/hLwl4D/EvgzwE/FP38E+G/j3//c400l541r0hskq0BMdHjdrmx7Ucv3SQfSty1JapiORhwcHDAejxnaG58JE5fbSoVdcpg2CqNTjFG7ll9eiEgT14AOeC0hvmrrrBQA5+npSZRFpZLGba10OcUgR6mO5XqDD0q0IeidQvH502d8+N5jhsWAxGgWixl5nnJ9fU3jW7BE3CHevePzMuYGke+85JpWVcVisZD1YDTIUVoLqNn1dLrDmESKXMQFrE3R1uFdQEdh2JY05B3k+QDXt2jfkaWpdAqTKcPhEEIFaLR2uDhGJElCZjNCUCRJxcWrS66uZty5e5/33/8p0jRnNjsXP8yNrEf7vt+NK977aGGn8U4cp5xzZKmMWm3TE4yKAGrHZrWWLY5JcG0XHcwmKKWYTCbMZjPo5fXqvSN0YTeKdN6RBo8JkgVrQsxNSZLIzvQsliLo01qT2gTnPFobtNUYFF3EtPCBqqkJaKaTfdbrNYPBkHv37nM1W8dzL0Hpjq3b1hbv0vZHeAwJIbwEXsaPV0qpj4D7wJ8Dfjl+2X8P/N9IsfhzwF8Ncib/PaXUnlLqbnyc39YR4NYMGqRbUAHUVpr13QrQrdzXGEPwPRjYn4y5c3rKwYG0g2nfRtq2F5Wjtbt5VmzxAxiNw+LjXVewPiVOTkGo4AaF04EQxNF6F5+3a02F2LOpNmRJhjKGPDeMR1OcC6RphveBwWDEeGBpGwkXPtibUpVrZvMrlNZ0fc1i0dP5XohV2uB9H3UHsk5FK5ImEf6CFwet2WzGbDbj8PCQoih2hLFdfkfToOJsb61FaSPJ4NGwRfcGa0SG3bcNxkgAcV/3lJuKtmox+wZtEpLEY222SybzMUtUKUWiDZPJhOVixXe+/QXPn50zny/5hT/+xzDGsl5f8+rVK65m17ubQpYl2Ci2stbStRJ1qEL0wuwcddOImM95hsWALEsoy5qtJZ9zjvVaLs67d+9RlmvatkYbg3f9rih08WMXbpLQQsRBmqZiOBxydHTA4eEhl1dXtG0fDZKbOL7d3HxCvJncv3+fNE0j3RvKuqZqGj755BMWiyWr9Zq6bknTHKVCXNF6iUN4S4/fFmahlHoH+Hng7wOn2wIQQniplDqJX3YfeHrr257Fz/2WxeLNzMntoa2iaWQboGO83s4zgJt0L623u/U2ItSWPMuZ7o15//FjbNRu9HVJQifhc8YwnI7i3C4WbDqCgEopCJ40KjWVUqhe4RzgenrlMUaRovFOMxkNUErGCk9AWbPb0FhrccEzn8/Jc7H97zrHcrmiKHK08hzvH5PQc/fwANqWv/Nrv8aLl18wmU4xeYLXjqvrC7xWHBwcYPOELDdUbSknZd9hk4DqArSWpu158eKMwWDAaDTagZoKSJME7xydb3cBwCEEEURpjSPglUYnKYk22N7SonCNp2oqZpczvva1r3N1dcEv/uFfYG/vABO9HXxQ5JGP0vc9e3t7grnUCcPhmKOjI7717c/43//W3+b43iPu3bvHp995wmeffiEy8qgWLoqCIk9JtET+aQ2JkbFus9nI12QJyojTVlk33Dk54fPPP0d52Za1raNkzXg85A/9/B/g+vqSy8tLhqMBVd8KoU0pluWGJMuwWYLymuB7rLcYApPRABMBX200D+4eoZSh6064mi1ZrVasVxJl0NQ1Vd2Qpim/+jd/lV/6pV/i+PiQsqn44tkT5nOx8CuKnP39fZbLJd5DF0HhJNUoZb8n7XsL+P4wjx+4WCilRsD/AvznIYTlbyF8+V7/8V2/vVLqLwJ/MX78fR4p2sPHghCCF4FWBDO7tiPLUpQRxDrLE8ajPbIsYW88YTAUG3gtrow3+o0ImG47iRA7ke1KEWSLgQ+vvUnysyU+TwHBe2n7vdvd5VUca0JwqBjxJx2Ej1kfCYlOEDzM4b2QjCbjEWlwPLh/n+VixstnT7FJImSsxGITS+06XOeouxs3qslkhNYW59d4ZXE+pas7eieWcut1uRtHrLX4Qb7DBLabe9l6QK5SVGyDb2exohV916KsRSnN9XzGsxfPWc4XXF1es65KsjQnsxnGSDp7nudi/nvZYq1l05eRyCakpTTNub6e8+DBI/I8xzmJNAgx8/S1c8LfbMS6riExuXSXIRBCjwqWNLUUMQJyF86swmtdY2ItaTTc2Vodeu+xiXRmSmt0YnfbkC1xTVhTPUolEVMX3chkVJBZQ5FmzJYLuq4hwjacnZ1xdvaCu3dPuXv3LvP5nNn8GtdLp+r6lr7rMPH5KR0ERH1jDNm9Dm+B0OwHKhZKqQQpFP9jCOGvx0+fb8cLpdRd4FX8/DPg4a1vfwC8ePMxQwi/AvwKgLXm+/Zer9mhv/F/WWKxWmOtZjw8IBuIV2JiZEZNrSVLEhKlhF+hNam1WOV2BUCncvJgNNoKQUYpCScOIdBV3Q5E1BqUMgTEj8IYjdHgHFhrdidl37vXWlOjEwhy90hNBjkkiaEoMlzfkicFoyJnUqT81Hvv0lcNvutJi5x8UBDyhCTPaIFNM2O5XAIamyZMJpOdS1aaphI0FOndfe9Zr9dcXV1xeHhIkhiGt8xybt4LtTOi3QKH27Q0gOAVaZbTR8OW6+s5Zy9fsVrO+eLZc7705Q9RccNTFAUgxVYpacG11ngF1tywM621PH/5ki9/5SscHByRZRnL5RylFGkq+IuJvAilxLx3+9pmKSgrXAgftx3WGI6Ojhg8eSo+pURMZ5ss5ra+lzcf+1jskzwTd7PEkuU5iZUxzfduVzAF35LkAKUUzirquiWxoib18eckaytck77n6dOnHB0dobR0l6PhGGMyVsvN7vxyfY9SgneZ79M4iEbpR6BYxO3Gfwd8FEL4r2/91/8K/IfAX45//41bn//PlFL/EwJsLn4neMV3h8Xe3F1CXBEWqTz90XDEvft36J0T63hrGeQ5PqLyeZbJRgQxqNHxXem6jjyx0QrOy1otMhrTGJibZClt3ewAQOdCvNlEw1VjsCEmZVkFJqC8cDLkrhwEuOJmTedcR5YohoOUzaYjzSxFYjnY3+Nob8r1xSsGWY62MBiOua7WXK9Kzq8vubySVWSeFxweHjIaTZjN5/EOmcZid3PW1XXN4lqwi+GwEIqyl7la6xvr/RDkzpamqTAZI14QQiBoyUft24qyari4uma53rBabXj6/BnL9UoKRfBkSUZBIXyGSJcOIUgkY96KiXCWY9OMs7Nz1us1kyjwOj/3YnJTTHZErO17LuS3VNzCIg6CNhA8QcvzPz48FC5L24ogK/JufBCKuetkk9GHPjqv33hOoDUmTcgHBcYoXFnSOQFbk0Twk3g9SHdptGzM0PS95KkOBjlplglDt+94+fKctv37u23be+8VaJUTgtx0xEVLxqwQpAvqb532txnJt4WRP6zjB+ks/jjwHwBfU0r90/i5/wopEv+zUuo/Bp4A/078v7+JrE2/jaxO/6PfzRO8vQ1xXsaQ3RZAwWAw4M7pMdPRkPlqKfhnCKit8YhIK1HBC+FGKVQEorQRGnia5ZhEXgo5uT3rxZKr1YrpaIzrBLRLY+ewU5wqeaO996BvJVdtO5GYUk4MJ1aqpu9bqnINRSFzeWY52J9gLIwHBa7rqdYblHMU4ylOGT7+5Ds8ffmCi+srqqbFWEueZfzyn/pXOTw55PmLM0IQZmRqM1qrYksfaJrI5pwvqI8OaGK2qbmF/ajeSUZoCHR9C6QYpJgksUVvGnHMms1mnJ2d7cx5ry5nLOYrRsMJVVVF/Fk6szS1jMdj+uCjbsNjbLK7MK6vr5nNZkyn0x04HHzAGL1zOXPO4Y0mNbKVMErTx+2RMqCweAWuDwwGA4osZaHErQykM+2dE11ML12jDx5rrCgxvCbJUmyaYNMEE1mjpm0xfhvfmGKUltfUebxSsTgM6FpH3zeECKqmmZgxz2YL8HBxdiFAslKUq5LEDlgsVqzmK3TQZFkSOxxx8H2zKOw+fgvkqD/INuTv8P2Xv99l0hC3IP/p7/J5vfGYN2IoY6SFT63lcH/CdDplfzLGeU+WRDJR21IDg1ySwPu2IzH6Vmut0EaTpQUqMewfHnB4fBxTw2FvMuHzTz/j+bMXmKBjS3zzfN5Mkeq6RpiVbMHMsDPtlYsSaXEjCNi2LdYa9iZDUltweDChX6/Is4S2qXB9T55ltCbj6fOXfPvTJ5xfXVI1rZgFq57lsuL6es69ew+4uLhivS5Ba8bjMV3bUZayRtwWi8ViQbXZsFlJsI+0+GZHzlJKYawmOE9Hi3MmqmtfD8O5urri+csXLNdrsiRBGU3nt1sHg1ZW3L77Hly/44Qs1xuur69ZLBbMFis2VUXd9pRlKXfUuDLVJmE6nXLnzh1WyzldtOHzStN3XohskUpOBGwTY1AWdJqK4W7chGit6fpe/Cba5mY8cV5YqXHcygYFaZGTJpmwb5V0GVaB0QlWxwCk4HC+ly2YCzE6QUuRGg7onKeLrcHh4bGYGW9WeA9VVfHZZ09JbC7/LhtZVasU58XLk8A2V3l7LX1/PO+HcLy9Erd47O7gIaBRZFnGwd4ed+7c4cHdexwfHJIkCd71pFbuPoPBAK1FFViXFYnRqBCj9pzss4PS2DRDW8tkb4/7Dx9w9/490jwjyTIePnzIcDxitlzICBKBse2fqHTfzbM7GvTWsfpWR+Sd3Pm2XUnXtfTRi3FvMiRNE4yCyXBEvSnZLJckScK3v/0pX//6RwxHUw4PTygGQ7I0J7Ep1lhevjijqVuKfEBdNVRVTQjs5vxtcSxLATnn8znz+Xznl7ltwaULSF9L43K+361B+14u+qZtubi+4vr6mrbtyPOc6XQfay1lU8v4FlWay+WSs7MzglYkNqVtW1zw4vpd1zRNt6Nn13VN56Xb2d/f58MPP+SDDz5gf38/vmZbUFCeyzaPRQd246qxiixJRb5O3O5Y+b6tdqUuq51Piev6qKwVyXue57KWNkao3Lubi1j27/QnyoqWxQt2c315yXK+oG2EBCgU9YJHDx9z5/Qu+3tHFMUQpYyse+sW70BrAYuFGrDVLW21R2+nEc7bQ/cOcicQ81mROZs46yVJglGB4TDjvXceMRmPGOYFSZJSVRVJYsl1wcHREaenp0z397i+vOKjjz6iLktU3TAZjRkVA9brNcYFjAqUixV7x4cUWca7j99hPJ3w7Nkz/s6v/7985cMP+cU/8of5jX/0j2nrhnQ4xBhN0AglWhlhYQ4UyliarkVphc00ofYQZMNQt4GgO5SDpuspEkvXdHTOow567j84ZGxTwt4R0/EBn37+khfPL/jii5f8zX/4D1gul/ypP/XLzD97QlnNMSbbnbifPnnJvc+f8q//mT/Lr/7q3+D8/Iyrq0uK/B5G5bhWaNN9CFy/uuIzK7mmy/k1zjkme2IS6whYm2KxDNKMVN8S3zlxHtVGcfHqjE8++Sar1ZI0t5zcPeHxew+ZjAZoFEZ7ys1KWvRsQKoyjvfu4uucg0lPOdXQF6yXjrZ0lP2aptowGKa40JIOU+6/c58/+st/lNOTI3rdsq7muLplMB7RNQ3GKAaJET4EsUvEE1SC8zBfVHinQSWoJAUaTGqoqg1BidLYBY+yFmMsxXDIcLTHYDgmz0ZkNgMf0H1Lsy6p+zWqKEjTlDxJcVro4mme4YEXry5YzNegDYPRhMl0j5O793jvnQ+x1jKfz/nmN7/JetGikXHFh57W1RilsNrSa3F0R2uU1oTtFu6WyOz7dRlvqrX/ZR5vT7EgKke3YjFuCFZ934OG6f6UceQMmAjAyVydcHLvDn/g53+e09NTxtMJq9WKn/u5n6Mu1/za3/rbbDYbDCrqK0pxNAqy059MJpyennJycsIgL/j808/o+54PP/yQ5WzON/7Z1yMYWkT0/ea4ETGJpmC7tjMR+Vc+4FVcxTqPShVFUTAZFExH452Fvow6akeWevHixY6Q9vTpU66vr/Fxht6eOM45nj9/zh/5xV/g5OSEV6/OpdUOVXxuYSdSWpcl2XzOZrORApsVwlzsOrQ1pOnrgOKNcnd7pxMfh+vra/q+ZzQayAi4v89gMMAoHcOCietKw6avOD8/Z7laAmL0IphBvwMtm6YiBNHD5HnG6emp8GSShNPTU56N91i0lzv8xWqDs4Idpch2yz8AACAASURBVFlG7x2td1iT7GIahXV68ztsx5xtlKHWmjRPSLJUQMmoG5H1ud1hVF3X0dubrtHaFKUc0EfNTkNTx9Ew3ug2mw0vX77kN37jN7h37x7D4ZDxeEye57vRqe1bUqvJhwNxjK88XS9GPlXb3bjS3wotSsz35l/8Xh5vRbF4XX6udujx9k3quwatU6bTKXmekWiD8x2bzYbJZMLjx4+59+gB77zzDrD1skDWeL6nGA53AbxplpIGmY/7Hc3W7zwmtm25c47Dw0Pu37/PsydP5bnoG8/O7fPdrdWMzKuidI0qWA/O9yiTELZ8DScFKs9ztvF6fjhgfzqJF09N01bMZjNhm6YpZ2dnlGWJjryNEAImitOur69JkoQPP/yQL774XLwb2lY0MsrgI3DZti3L5ZKrqyuRvOe1EIFsDA4amUiVvykYt9O6lFLM50tmswVCn97j4OBgxw5NjLTnCkWSZ+RJjnOOs5cXNF3PvXv38EExn8/lok80VS3Pf7I/YTAocN6yvz+NVPGU0fEw6k4aVFAQNDbJCEpA1947nI+2+tbw/PnzXbQA3IwOShmSLEUnFr/xOy6DtVZ0I6nFGkViVCTvdbRNQ1OV+CzdnaM7Gzyks6mblrYX3xQhaomMve5avvnJR7x6dcZoNKKua2GOaiFgGc2OTWusJXGpsJUjB+jGJuBHbxvye3DIRejDjTfFloQVnCc1llG0YBdCVUAFxf7+Pu+++y4/9dMfEozi888/F/6/jp4Gwe0ujsFggDHCsHTO7fQHSinKsuTZs2csFguePXvG2dkZh9M9vvXJt5nNZoxGI9br9e5C3WEXKEzQOOWjojHsvBVVLELOOeiEzNV3PVWnyMZjsiyLBQjKas3poWwqtpbxKC9K2CzbmcFuZ3BRX0qep7GK8/OX3L9/j4cPH7Jczanq/sY8CIQSraBuGs7OLyjrljz+rDTJ46ai33UGsCUDaUS41eMjZ0N0JgX70z329/fZ3z8kzway/YlYwPY9lOds0K7n+PiQJEtZlUu++cnHLJcLUJ7Fckbv7jMZjynrDYPBAKUEm1IBGSmvrnj18ozNeoNSmiLPcSHQVg0YTTEY0vc9z5692G0etBbNzZafoBPZPKBFB7S1LCiyhMzKH03AdQ1tVdJVJa7r0NYSlKLtfXSyiuZKPfRe4Z3GBU/fS6EoEkk+67qGF2fP4xq/IM9T9idj6RAh+nSws/TDaJwGg9lFK5po2KS13r2uP8zjrQA4t6QTadNef0rOdwyHQpEej4akVnb+gzxjMpnwzjvvcHp6yvPnz/n1X/91Pv30UwCOjg744MMPefz4MW0v4blJkrwmPttW8cViwXe+9S1+8zd/k29961tkSUJd13z00Ue8Or/A2gQbNxnb0WeXicmNp4bVNxTv7QrRGEPXtLv22GrDdDplOhmhtaw4Ly9f0XUNi8WMst4wn892hQxkhblbJfput/bc/tyPP/6Ytm157733ODw8BDyd7/BKEri2XULbivHter3eAY1bF6u2bnYekDeFYtvtyXZhGwQ8HA53I8je3t7Oz2JLmy/LksV6Id1QIn4Z8+UM76VoHB0fUHcCiM7nMzabDVmW7Ipjnuesyg3Pnz/H+4CxCYv5kk1ZRsZsoCdg8hRbZLSu5+XZK15dXYrewxhMxF2k85OtTTEc7DrB4bDgYG8qdnpGtD14T7OpqMsS3/fYeI6IEZAS0Ziy+GCoG0ffBTENQtE5MSX2QQSJXnlMatjbm3Dv/h1O7xwzHBVSHIKjyNOdCVLnHZ4QJezq9S7m1jn2wz7eis5CKV67+MSMxKECFFnO0eE+B9OJ7PwBvEMbs3NVKsuSyWTCwcEBe3FTcni4z+npKVoJRrBarfDek+c5PTfzeFs3XF/OdoKj6XTK0b17PPv8CU1Z7fQUWZbRNy1a3xIMRamydLtimpInKa3tdxfPze+oGAwy9qdTjvb3UCqwXq5YugajhCNQVeJwfXl9hTYGo9wOA5GthIt7/wStRafSdR1nZ2ecn59zenrK/fv3ubj+nH7dxs2GOGB5Feg6h2pqrq+vGY/HtE2/E+ltZeVy6NdOzu3cv1gsICaBjcdjxqMpg8EAjBWVZ2Q3tl1H13W0bR29MxRX15dcz+a8evWKuqspBhnVfMNms+H6+pLh8CH7+6JgzfOc2WzGq7NXdE0r2EBs97N8hNcGnWiGwyFN1/Ls+Uu+89lnbMpSsCMPXm11JjJGTKdjTu+e8OryXDgzacpkKh1eYjQ6ena6tsN1HVZrgk3k8RRoY7FJhusVdbVhta7ovcZYMUX2XY13smFpXcd0OGA4GHBwuM90MqatG/IiIUuE+DUaj3AK1lUvhWwgRDVnO7mpeY+6lQy/Db/6YR5vRbEIQWa5NLXi2NT1KAWjQc7jRw94/OA+fdeSJQngcV1P01ZMpycUoyGj0YiD7oB/40//acqm3BGAtJK5frleYbQmHxTCuosz/K79cw69MUKm6edsViXVRkDQEE+iNE0xyB3adl0EOt1u7DDaYBIbsyQCvWdntT8aDmjKSiz125qLV2cY5UkTxXg0ILWKZblCOST1ajQiLwq+eP6Upql2IrA0TTg4kAu0aRouLs8JwTEcDthsNqSZ5YMPPuDscsPHH1+jPfjg4+rXCgjnPP/0//saeTGkGIx2XhjbYObhcLi7s+1cx5Smdz1PnjxBa82jR4/40pe+xKNHjziY7on5biMdSp7n2BjMrFSg8x2DJOf5yxecv3rJy5fnDIc577//DovfuEZrePnsOe+++5ivfvWr7O+LpPvjjz5htVrxtX/6NTarNSdHRxTpgOM79+lDy6rc8PTTT/nk29/iyZMndC7ggibPBrRthzaGDEuSWKqqwunAV776s9gs4ez5M7Iso0gTssSigqfebOi7jsxmpNrQYtA6QdmU3kFftaw3PfPlmvl8TVW3eJWS5Ibe99A7lA00fUdfex49POHo6IjpeIL2gTTJef/9x1y+OqdzUsibvqWsNugi5+D4iOF0j8qkzGLSvXduR3vfUs9/mMdbUSzgZiSw2shs6Hum0zGHh/uCM/Qdndki7SK8sVm6A6m6V2dsNiteXV1yenrK4eEhXddRVZVsETIBReWiuJn/9PYG6oNsTIzBakNmEwkEcEDQuP5WlADb7icK0MhjsTO7GZOup+lrvA/0cQYdFTldU5GojOGoYDIuGBQ5y+Wcq9kl09E+q3JDWuQSytu25GmK73tU8IwGQ/YmE0ajgThprWYMixwVAr5v6eqGw8NDDvanqMDugpfuIWHr3LVYLHjx4gUPHjwghEBZrZnujfGR2XkbYNuOOl3dMZvNOD4+5v7de7J1Gg7F3CYyI5WCtq1pqloozM5RNxV95xgOC4oiA8SBTDYUYGykOfeeuqyYKwl/ms/nPHnyjOvra/K84ODoGO/hajZn3Wx48eI5nz35jOvra6q2w+iEwWgIQTEdTuk6AcDpHYPhVFzW65LRaMDRkbh1HR+J8dF6tiJ4j1WyWnadJMd3nWxVNlVHWVaUm5q2k06ycyInd9E+0CsITkDXNM/iNB3EzXxrBKQ0J3eOeX72kt53FIMByXrDqpQOeRxp9VubRufDDSFO//C5F29HsQgB7zq0srRdS2I0g+GQ4WBAok0U4mwBM0tiLDboHQ4gbbLm6dOnrFYrmqZhNpvh2o71es3edMzFxcUORxiYJBrUhmh3F0cgJ/RvF6ALNzqArZCJ2FkISzFB64CYl3Rxbk8EyOx7qnoTDWpFIFQUBffv32WQpxitsNqjNHSuRcWK5YLMvXXbQDSP3d7dtdYMBjnj8ZDBYEBdl9gkGsTc8vIIwfHOO4/4+te/HoHSgDLbOVgKwPb1ubq6iqDxKI4ggeD9bk53zuG6nmCEBVlVFSeHBxwfH3NwcECaWinkbRe7K1FraiOvZY8nTyyLpqHrHVlqyXPhxkjBkPFOAnoynAusVnLhPH32gm9/6zscHR3x8N5DNmXL+fk53/j6N3Has1jNqesKYw2jdIzWliwdkKY5o9FEGKvVhq7v8bgdyD0ZjkjMDYGrrRspkhiUUbJBArRKCb7n/EJWxW3nYlJ7EkFjI2ZJPtD3NwrdgJjfbIvuFkMZRK/Sw5MjatfRuSA3jGbEpq1Zr9cMxxVFJMdZa0Vqj4yaRv3w4cW3o1jE7irRhrbvSPIBR4f77O9PxdC1dySJRVnBAWyS4JzGJAbwNF3NYjbnG9/4xi7fYZDlgk90sptXQR7fOYejI8Sgod5HJ6g0ee1OmqRmF85z+07b9y7qK6RQGGPIgqYPHhd9JPu2iW24ktl4JDP+weEeiRa/BE0PMZzIRIq4I9B0HXXXMiiG5GkWHafl5JuMxkzHE9mKuF44B127M9npu4a+63hw9x5H+3ucn1/QhkhuQ++2M94rLi4uePHiBXfvnWLMkbiK5/K7bdWzBI+xW7xiTr0pGT1+xMmJFIs8T2nbOoJx0VEs3BQv4VYo+r6lbbpdF1hVldwxlUYFEegVxZCm6egjo/PlyzPG0z3u3XtA2bR8/PHHbJYbSQDD4UJPXqQMhmOSXLCFJD7O/v4hxiiqasV6vabrRA+j8SRZQpJOYmRAwHVdFJ4FrLKRKwOt82yqlr5bRYMbg04sSSIKWhMtA53vcGxXtIIPiU/nhjwREHM0LhhHez+TJmzamrPzV9gk4eDggGVZUZcVruswcbOUJAnK32BJNjE/6SwAYuQwWotXRZHlHB8csjee4IOj6xrSVFpendjdRW3TqE3oOvHTvHMHYwx37tzhnUePyYuUT75ZYlCcHh1LtQ7guoY+eFQQUdHWRt8Yg0lFzNSpDq9uAZReUtGd8yglRQqIiVqe5XJJ1/UsFvOovVASlTcasT+dRAq6wvlOzICVR+NRWpFYMZ6VbBSND5DmBak1qCh6SpOU8WjAMPpRSHcihrQaBUG6gL7tGA4N9+/dYb1e0y9WO5D2ttfDer3m/Pyc1WoFyFglr4MjBHODxcStzOWrC9q2Ji9EKJWnQiIDMEZWiMF5fJAWXhJloeua3ajXtx3WCDaklFDT27bl8PCQyXAkj6UMTSNxiF/60ju0rePb3/mMi8trQjT2xSpsljMYDcgGBSb5/9t7sxjLsuw879vDme4cQ05RmVWZVVlV3a1mNdktNylTaHiAB/GF9pNpA7YMC5YfZNiG7QdKeiGgJxuWDRs2BNCQAMk2LKs9wDRgiaINiaNIsZtsdndVd2UNOY+RMdz5THtvP6x9bmQ1q4pFsVkZBccCLiLy5r0R+544Z5211/oH2dcXeY8sKxgO+8IcpeHxw4dSgaiTPkyWpKgA69ggD20QxZOgqErHYrFiNl8xm68xA4FlC48mASXub0FJItVOiylVAKUk6YdWiGtaSxN2MBySZhlBQd7LGE8mPNrfZ11X9AZDtkZj7j96RLla09MnehtN+KCeyvOOU5EsABSeuhKZ/GG/YDQakBcZy7mwG/M8x+gEoxOatqVuPTknknBbW1u89NJLPH36FK01o9GIt7//Ft///vfp9XqkNmE+n1P0ClTIqetaxnBtoHymEuhGVq7xWCsNptQIg7RpmojyE7GWtqxZLOVuN10sqKqKdVmilKJIU4b9HoNhnzRLsElU+zaCz/Be4dqGXi+Oz1wrIrlGAEedx0W3zTJWpjppmtK2J5obwEbIBSLLsqm59uJLUtKXDatyLQgBJVspYwxNIxgU4XkIdTwEt6FkC7JUtCJmsym3bt2KTVYp3zvhoLquydIUJ5AMdOsRZVJJGE1dA55EK+qmEoMmYDGbx/6OYW/vBYqih7bSjLx//yEXLlwgsRnvvXuDg4MDXHRJCyJ9RJ7nDIdjBqM+SfR30daSaEuaJxT9bXQCy9WCVbU8aQ76EPUzZe2u8dGfVOD469WK46MZ09mKdVXT74k7nTYWOi5H9Bmx1tA04mOzwd5Ixt9MMeTCT0AJa9prxc7F84yePmExX1L0B8JncZ7ZwRGZMpu/6Ql50vx+QaDnEKckWchBreuK3W0Zgfb7/Y2GQPeH7S7WTgF6Z2eHC1Fbc7Va8dprr3Hp0iXquub+vTt885vf5HD/KePhCGVESSlPU3QUI2m8i0zGIFiMzZTEkD8jwNJRpZ0L1K4V/89ITlqvZS/flYjdflPUoEQbwlrZSigdhCKvDar1BMxmTNZpIGAsHmgDDHo90pgwkth0xTkMCnyLRtwQVHD4piVY+VqtV5zb3eHqlcsCP370RMhKSncYJWGCzmY8ePCA4+Njzp07FyHJbiPL38Ggj4+Pefe9G4zGAyajEUUvQ6lAXTeU1Uo0QhBqvlcKvSnHHVVscIboZxKiifB8PseYhK2tLba3dlEYnAs8frzPu+++y5/+ya/xznvvc+feXRSasqowJmEw6LOqViRpHh3Ox6RFRsDR1JLcdWLIi4KRHzEcD5gtZDuXJekG8OeegX57RKVrMV8xn62Yz9esypqAwXmNiSNU59loTwQNrWvo9D67y9g7Q3Ceupam6GKxIC1yBrYXldhgNBmze/4cq2g+rQKkNmG1XLLI8xNN1Gdg9y4mjecZpyJZhBAo0pTgat544w0uXTiP8yKKamJzbjqdcnR0JGpQVcNgMMDcfJ97D+5vtBm//vWvszWeUNVr2krwFxrFermkidZ15Wq9YRoaa0isgLvE4FZMcNtWmJodCKnD6HuvqGMFkmUZw0GKjvTusFxiioK6rmJlII+AF40WHFonwmnRkFgoYpXknKNxFVnZYJOENC/wIdDv9ymKAqWCEOTGI+mpGCIwq0UpkRTsxGGccwIqq1tefeU63sNysebp4ZHIByaWtnVoa1islrz51lucO3eO3d1ttre3N0phSolgzfHxMb/8y/+A3/3d3+VrX/sab7zxBqPRSJJ3W21GpY1Gpj51hDbjqcsSg2LVNNSVYBjKsqStW9ERvfuEn/jxf5rz5y9SljU33nuXt99+mxf2rvCtb3+HmzdvQlAsVwvSNN/8bbK8x2Syxfb2LqOtAf1+D5RnNp+T5z3wgbxIGY0vUQwyJlsD7ty5wxe/+EX6RY+mEjOjuqwwGO7ff8xstmC1rHDBoEhQWtzQ61qOsZg6C2JWJyJkNJ9P6eU5O7tb9PIC3wah4R9OOXx6IF4rZcVqtZItCJ68KKjbmot7e9g04/GDx6RZ4KUrl3n/HUEgd0C3Xq8X8So1WZJ+AH7/POJUJAulNKuyISv6DId9alfG7rzHe81wMJG7eVWCgl5/RJrlZEHTN9Jkc85RGMPB40eb6iNEsFcwsA4Ny0pk3vq6R6hbkqDoF+JuReuwKJGlizoEVVPH9SkcgUIZepne0KDLugJXolVLkUuFgIueHo3cRY3SUpp6KaCNFUEeAUs5cGBIUFgSI9sRrVpCWJMpwyjPaXCMhj3SzLKuGoKHJOvhgkU5sf9LjCX4BhMc7bwG3xJaj3Et2tXQVihtCQSRAQyaIu/hasfB/lMO9g+5dhVIgLgfb9o1jx7f4cbbb7IuZwwGBdp46nqFUYrlciF3uyDH3weHTQ0hCAI2zQeYpMGaQGsrCIq6FoIWynPh0oTBMMP5igcPHvLgwQO0SXj55Vf5h7/8qxAS4ZHYaBBUN3jVkPeETDjoj+j3hiSJoGrTZEVVzuL2TASUiyxhb2+Pb966y717d7h27RVWZcV0UeJaw9HRlEeHi4jIFGCdUoEmOBwO72s0hswkJEZG9iYo8FAoRa41k17OaDyQREuOYsXBTAyW+v0+Rid4p9DBkuuAdjAseqgtj1vWPHr0BKOiSJIPtOuKBGnAqqDRsepSH5iIxKbqppn8x9/XOBXJops2nDt3DmP1RhOi82tQSuTuu+lC3u8J8zSJalQhZb1cyF3XGpJOi7LrP/BB75HO7DaLcnvOOXE6X683gijGGAqdo8yJyE3aQaDNCcLRx/U7J9RnAGXN5nc+O0np/k1HmAsKH124g9cb4pyJAsR5LqV2G5pNn0BEgS3rdRn5DydkuBBChEO3m3Jba70BXbU+cjYC0ahJY6Lu6NOnT5nNZhSFSO/lec5sNuPNN9/k7t27G+xKkiRysUdzIvndojUhbm7mA59XeisGk/RZzJeEIGPMqqnZ3t7ekPZu377NgwcPeONLPxZFY+S1eZ5uyvFGNZtRZFdJZbkocmkTmC7CZusoAkORsAes1xVPnx4yHG4RvGK1WlOWNcfTuWwv4t+ps4LoJlDeNSiVkxorep4BtAqkqcWogjzLyLOUPM1IrcE1A1aLJU0j4+bpdCr+qwcHmFT0Qq5evcpoNKJtZDu2XC4Z9sdRsIcTThEflNZ73nEqkgVEebyLF4HOK6QWWz1CVIcStGVa5AwGkizqusK2rYwelcYFcf+u18JJICaaJJZwdVtFGzw2dOWjg4MN47RDMGZZRhEBR2IpJ388SweMibgFnmHMGo1FEyKoqEtyHdVY2TgS8PJ5pHehyTI5uRfzNctyzXAwZjKZiNy9SphMxnjlyWOf4ESAh9iobDaQ7a5PALAql2A0o/GAvct7rOuG/YMjBJuuZRSoNb2I4pzNZszmx7xw+RJlKUnvyZMn3Lhxg7ZtOb8jPY22bUWotl9sSF/elfi289pQYGRy0FHq5fjWmx6BMtCsGvYu7QlzNorybG9vc/nyZW7cuHEi918UKKUkkce7aJIa0jQhyxPyPCXLUrSRflHp1qh4wSmlsCYlSxVZVnDwdArhNkmSslyuqUrHarVmg3KHTUXbHed+0aOXp2S5FUXuuqbFkWjF7s4k2hIWZInCe0Ovn9MfiGhx0zTMpguWi+gvYhJQnqOjKdvb2zjnePzgIet1w2gwEcBgs6JtkxOYt4YQPgi/f15xKpKFAnbPbTMajaKyUxWVqPvxpIOsKEhnc0aTMaPxWBpAqZCrOpMYm0hjqG7KKJUvd7zGtZvRYNu2aHdCYW6qOl5AJ+KySimyJEHHJpPxXkBaWkBL3oshjSSMsPFf1daSJwlNEx3DlDxE81KduHTT3TH0BhfSNA1+taLIpU8hTc+WrJeRZIJPUNZgvINw4kLWlHEL8AzfJShPG1o0CeOtLa6iWDcNtQ9M56uNA5lSIsufZXJyz2YzGUlH0Za33nqLx4/32d7e5trVlzdToPV6TWYTbNKBkSzWgtYiOYdWhCD8kE7FejqdMlvNN1VBVa3Z3t5msVhw48YNUJ4vfvEL1HXJrVu3cK4hLVLyviQot3YErVDWkCRWcDCJbBuMVSgjautVVUEI0RxJ0zSCtN3ZPs+7h+9z//4jesUA78E5T9t4lEowRkiMzQbKT+QOlTRJQmJlVJ1khiTNyBLL1lgmXWmaRmPqQJGKDUUHMqvLBhcaXCtTl7zf4/Bgxmol/ZyyrDfbizS1VHWgdTVNYz9wY/jIZBH0h4hb//HE6UgWWrO3t0eepzTNktVqxuXLl7l48aJ4SqBwbeDp4SFJlpFmcfS1EiCUtQnWCeW7wVO2YuDTlOLwBR8s51IjuhCJMZg835TwJs63N2IoEWrbwAk1vmPH6pgM4niraVrSeAHXtXBJOhNep1q8ESyJjSCrzoKRCLxJ05SglTQAW9G5UEaTFSn9fkHez0miqLBrT/wwxM4wnkgqGi3jyIpc9DuKhG2zw9WmIc36/N533sIHFcFSonbdbVU6ST1jDPfu3eOtt95Ca83Vl1/h+vXrsRsvlUkIgeCjUM5mi6VonZcqI6JjveuquDo2ZxUdDLooCm7fusuTJ4/Z23uBfr/P2+/cYFUuSfKUwaDPYNCPVUWIbF/ZntrMbmwh0dEESgdR8m715sZgVYo1GXk2wjstTeyQkGc9jDbUwZOmiUD6o+hyh7uRzwjB12QmZzAoKPKEvLAkRmO0mB8pRBLAaElSG+3XVmD+zku1aYyOidXia+mJKNVtqRLSzKJXsrVrXS0WEsAJyI2P+PenE6ciWVhr2d3dxVrFfLZktVqRZpbxZIiNbuPaGIKNwixaSze+rNBGKMFlhDCvViuBE8e9vNKB0WgUxVnk/f0kO+k5NC2hbaOLlcJGbH63b9UaUqXFQV2r2MgL6OCf6UOoCEM3seegEMJbTU2gKNINdFcrtQFIdRBhHY132h8AiCW9lDRY0jwVJGsQb4+6ESanjYhWImhno91oFc61tM7RtC1JnnHuwnmwGe/cvM1sugDAeU9Zy9asKPr0ix6LxYymcdy5c4fFYsGVK1e4fv06W+MJy/kUa9Ko15lho9N504jgbGgDTdOiCVL+W8/RckpVVRsVqqaRinFvb4/pVPAbg8GAqy+/zGq14O7du6xWC7Z2z7G1O2E8HhMOZZunvIw5k7j9sNZEpitxQiRYFO+IzuctaV6QZQXBa6zJ8G7Nai3ubYnNCDSgjMC0Y3Q9A6UDO1sTRqMRO9tjRqMBvdyitMe1wjJt2xrXCkxcawvBowgMBgPqupXKBbGGDF7Rlh6diYNeB0oDyIp8wwvpFNIwp2P70cWpSBZpmnLv3j2sVRQ5vHL9Gi9fv85oNOLJkydUTUue9RC8SiDLE2ymSJJdHjx4wK3bt5lOj/DeU/QK9i6cYzKZbA50mpgNz0NrTWhamrJivV6LhVxQBO2xWmNymdNjBNYLYXMiuUhB1kpho6qSpgPiQLUusdpwfntHsP6jXIRrEKSld45gLVZLMiIqb6VpjvOB4B1lBz1OLUE5jBUwl/fSl0hSSXrLhcCyu5l87VpWTYWuEwrVkPUzaB2z9RxVl+TFkJ3dXa5eu8bv/M63UZGNOpvN2N/f5/r1lyXJNi2z2ZwLFy7wM//av7ERHFqv1/TzAoITgWGTQPBUZROPR4YyUFeiHWKMJUmiU1tUXe8UvLa3t9ne3eHv/eIvc+WlF3n55ZeZLRf82q//OqtyTX884MWrL3Du3Dl0krIslwQd8EpIW8YG8jwjLyw2NRgbm6gmQWFo64q016NatswOnqKU5snjY4p8TNvXTOdz1rbFDgusSsEDAgAAIABJREFUFS0OEZwpcd6Bakmsot8fcOncLpPJmK3tIVlqaNo1bVNCaFChwrdRqNdmItSUZLx2/SqvfflLfOO3v8WNG+8yn60IQeNbaJrOYjOh18+jWpamKAqG4z6rldwspXdSS4Xju6r4DO5NZ2BbVSv+uX/2T/Hqa9cYTSb44BgMBoTlamMU05nVuuDZ3z9i/+AJq9WC4WS8kZNPenKXTpJE5uJRe9NElWibpmhr8ApyJz4ddTTnab3DxfQgU5jIISCQG5kElGW1wex3k4jOo9MYQ1vV5EkqQidW+hJKE4FdDqPixMecKG851xIIopvRttRRfTtJDUUuoihSnQj0eI1sr7z30gCOZDibJrQ4JuMhuiwptGW1rsl7BUkqJ2Wn4l2ul5Sl4uhIBGiaRvgbOzs7YiKdi1jMcrkkaRP0cEBwDaaDIUcZuKYuI5dEnMGc6zgy9Qa6DHK3d07wGzdv38IkCZ/73OdovON73/8+i9UShzRFd3a3GW1NNspXxipCFftJWUp/UEhV5QPBR6MfZdFojMmoljVP51OWi5JqLaZD1ib0en3KstoopnWWlc7JxEkwIrIlyFMR7qnqNTAUTpBvcG3LajUHX8cmbo7Wmslki0sXL7O1tcM6SXn1tTnHxzPK9X2qytE0tUz8jKasFsxmM7IsYTCcYK1YCnQgPa1Pts2dQtvzjlOTLLpm2N7eHi+++CKzxYKn+/uMhmPq1kUVphKPkJ2ePn3K4dGUoijY2t2hrmuOpscbtGe/X5zAgJU4WG1YnB60tZgsJXcFnoBp7cZKIDFGphqd0pTVMsb2Po62XEwa5Qck0FAiWBK0SN9txnG+xXAyAvSCA8R+yEhM6Tg+DZ4mNBv3tU4IRSY8etMo7C5E531stsq0Je/n0YbQomzKcDJmuRCUqHMNWgtZrK5rlss5B3Eq1DSOJDNkaUGSpniPbDl0Ql0taUqFrytC8BCbtt4YlHe4bjIUE5t3UNct3oOKIrsd9d8Yy+UXX6RuHe+89w6Hh4dkmfRgBqM+/eGQLEs3MPxnLxabnGy7tDZYbfHesTXeIkv6PLz3kJv37rD/6JC6dliTkoSkG2bLtiXeqbu/pXcOnVrGo2iU3TYbiYPRaMRisWA8HFBVa7zr+jaKNM3Jsx7j7S3Onb/AzoVdxqMJYd1y8fwFXnrxMovZgv0nR9gs4UtfeoPhqM+TJw94/+a7UTzaMBgMwMhovBt7e9+JH8FpELU7FckCiCV1nAzUjnK1IrMpd+/e5eHDx0IWSkQPoWpq9vf32d45x2g0oigK3r19U8q7XsFwPBSti84LI8jJ4X2LD54QkOmB0ZgsJcVhfSIz8zyXC7NtNhWF+FNI81ArpCopPyh91nrZq4qlYbSng9joq7BBqpVuP9ypaHUjsrquCc94jPrWYVIRgrVKy/pb6ZcohdCgI31+05+JzVmnPUWvJy5X2pIniqzIOTxacHB0QOMdNtjIiZC77OPHD6kjjF4rwTAobfG+3YgJEWHlXkmDEgyI899Gko8f2PsLu9SglcEmKVpbHtx/xM33b/OFL/84i9WSW3fuMF8u6A172FQg4OPJkMRmEUrvPoBX6TQzO/k/sZV0YtNQlTx5fMDDe09Yr0sMBp1qVDRFFrFcoekvFzPSLOOlFy9LBYNsEXSAxknD8srVq2iteP3VV/jSl36E3/hHv8pv/9ZvMhjmWKMZFEO2d3a4cuUK2zvnKIqCLM+x7Zrz53e5fv0689mS5XLNcrGmVyRcu3aF4SjjeHpA9Xi98W3pxKLlhnTSg+qIgM87TkWy6GT/29ZvaMwHh/vUdc3tmzf57W/+Lt57LlzcI+/3GI+HpDZhPBqQ51Lu19V6Qy/XWkyDhRQlCM0QROQXkK1G8DR4gtUYb7FKkRUFWZoJRLsxuLqhbRraELveQaoNZUVNOlhNMBZlWkLwsq3QKuohxOan8pv+RwgBHx+dY5YxBh/AWoePiFMAbRw2yr8bpUXmTSe0vkUFTS/LN+C1sq6gVPRcXyqWVOz4oosvRosU/v7+Pvfv32cwGNDLUlzbsFg0hOBYLOc8frQvFV7bRv9O8T9Jk4yyLDfHVtYsZLEQxKHeiW/k5uTegMSaNmp+VqRpjsKwv3/AdDqnKhvu3nsgXJ+4lRoMBmyf26bX623gzc+qdsm2RraVVll00BgStLYcHO5z9+5Dnjw8iNMpqYyaqmWUa7LU0lrNoFcIbb4uKYosaqVkBN9idWA8HFFkgkL98lf+KZbLOcPRCJv2+Pznvsiv/eqv8/T2Q169fpVef8TlK1fZe2GPJJOktVwvEQnAlO3tCXsvXGR/f5/1esmDh3e4fOUCk8mQF1/aI8nkMzfRL0cMuDUhNHSCyX9ghE+n6jgVyYIInkkSvRkldV4Pw+EQ37QczeY4F7hw8SIXzu0wHo/p5QVBIVLxqvO7kImBtRqTaLQVYo8OgWAEPutoaYLHxRMwWEEymjwVQJEWqbmyLHErJyhJpWhdC8QL3wgEvHEtq1q6/R6ovZPqA42NCSLJUrQRVGcn9huA1nk6CpKWGdwHRrxaiVu78tIwtCbgGidoSd/5qipcLSO/tMjpjwakhZXf1YnNmoT5csmDR4+YLua8tPcSF3Z3qMo1Vb2kqgVpeOPGDb7y1R8nYFHKkkYh3i5BuEamDp0wb8csDU6SaYiK423b4lq36essl2vKdU2SpUznC44OZ2xNdnn3/fe4dfcOrXMoIypR5y5eYHd3VzAHVfMBdKpGkrBWJyhbsQBMWK1Lvv/muzx+vM9iscaQUJUlzglTNs8t3jfgo3m2UTilKIpMPpPRZEmfLBnzyrVr7O5uc/vmLQ6OpgyGvWhgNOPCpSu8/vkf4Vd+9R9S9EYMhltMts7hlKGO/KOuX9a2LWlm2NnZ4uKlXY6OD1gsjzg63ufll6/y+uuvcuHSecq1MKCztOsndXq0zwhDP/+WxelIFiEEFosF5y9IEqiqCmtSUaoOovmYP3nK06NDfFRvqssKMxFil2trGXNGFF9n6HKCPwhR1VseHf6haqOhS8QKeCBYhbUJibFiT2gVbS3NRiIzVfuAahowmlYF6uBIg8IpucN28HQd1b3SbrTZVQ7mxDu0GyuGuE159q5sdULQTsatSqYvrRYxINe2G2CWrsVuL89z+sMBzjbUrawvIBfX0dERT5482ZCTRqMRvQu7BCru3L7Fo0cPyEyPe3cfcNEJSrXwYLOUoE1kkp5oQpyMfzVtewJi6rZZ3cM7sDYlzw1lXXHn9l1mswXXrr/Cm+/fYj6fkxUpWZoz2dlmb29PRt1J8oFk0Y2eVTQD9a0TzoYtUEEzPZxz/95j5vMlrvY0dUtVNWRJSi8vMFpRlRWtdyQGhsMe29vbfO4LnydPM1brBThPuV4ynR4x6GV413Dz5m0uXjwvOBuTEILipauvUnzjd8mLMTbts1xXzFZLUJ7t7Ylgg4KOzU/L1vaICxfO8fD+XeaLYw6P9nnJ7zHZGtIb9Dg6Omb/IPrERETvyfSjuwl+Shfjx8SpSBZpmvK1r/0zfPkrb3Dp4hjwXLhwgdVySVs7zu2cZzQYs3Uk0vO+8TRlxb07t1FGVKoSLfP7wWhIXhQkaRJHfIamlhO3rWvquqZshO5etw1JlqJ0pFdrAYh5rXDak/V7DCZjCEJhxsn4cr1qSKdzgrF4a8n6ItJbxN8HHqxCJRYdTZJCUOi63twRg5XXplEqsJutd5wSrTV1WUricwGHwypNnuQoHFW9YjAYsG5rlvVKRpORoWhzy6osyfMedeMo64p333+P926+T1VVXHz1Ar1+wd7FC/zIG5/n9q33+P5b3+W7336Pr3/96/zYV77C66+/zoWLewwnYzmJjcZEj7y2bQm+RhNIjN4oUXnnCDgSY8D6DRx9PB7z8PE+t27e5uDgiJdeusbWZIfF6i0mWzvoFF577TovvniFre0xo8kIgoCjqqqKsn0nKuPdxaSjC9xyUfLk8SGpyRn1LauwxKiE1GZMp0esF0usHrG1tcXe3h5JmjKdznnp5Wt89atf5caNG9x+/xhrDKF1vPmdb/Po/j36/R4P9mv6AxEverJ/xHrdoEzBtVc+z7p0PH5yyN2HD3j99VdBOd69+S6vf/51dibn4rjb0evlXN67wOHTF/jGN/8xN96B7Z0Bo/EWzsPBwRGLVUWaZ+JeVqQbt3u54floa3imZ8Fg2Oerf+oNzu1u07YNratRKsMmCUWvhzaQZpbMGoo0QQdFs25Y+nKjTaiDJtOavE0ofEpoDSpJhOxkpDFYa0VtoKWlCQ0i0+JIbRrdvxJMHHOqJNBQ0bhK6Oa5RiFq301T0mSBJvE462iN4C+8sYwGkfwWvTiddygtVYCxot5UeXHoxCoa4zEWahfwKoAHZS0aCwFUZvEKmqp6hrwWKN2adStmw3mSk6gUWyfYKkV50ZS0yuK1YTafcbB/RLlao3ygXxQMJ0O0lQro8kvXaFrPo8dH3Lt/i16ekmropSlWBcxoiEoSSFUkWzUYrchtInD6RvpNxmjSrKBpHG0jqFWdJazWFdP5jMNjMWw6f+k87793i3K9IM9ge7RNmjj6PU2vn2ANrFctCkuaFrhgaJzDmETczbN+VBRzWO2hrTncf4jRKbVXWNOjqZeEtqKXJphMsdcbcG5rm+3tEct2TeYDx7N7vP19xaWL51mue7QBwnCAbTKOyxkZFjvYYrZ2JHnKrVuPWUzfYX48ZTAYcFhX1M7iA1S1YjKe4KqHPLq1z+RHBwRVkSYO5R2DQcr58xPZli3WPHj0FG9Ej7QzsCoSTZJ6khRcWBEQAJ8IRut4IzrxdPm0i41TkSwSm2waWoPBAOcbUQ6aLZ4Rc3UbLIPWJ2rbz5a+3QgMEDcnOvWiIGNPRP4sOL+Ro0ttQhq3HVaLsrc2gG8BRVACigkqCFwXGUcGBzgfR5viFpamqfhoyDs3DcH1ei4Nyo3xUCKMWWPwdYvqEJvaxFGg3DkTJVsLX9YfKMVD8JjEQl1HglxL4zzzlfiYFkFm9W3borymXK1YzuYE58QAOULFOwUmYwy7u7t85Stf4Rd/8Zd4/PhhFO/JeVVrFqslk8mEPDPgm9iMdjRB9D07rEInCtxVSU0tSfTw8JBbt24xnU65/NJVZrMZ8/l808web4kV4mAwOLElMNLfeXbitNH5hM1ItW1bFsuZcH6MuIx530Ipjm472wN6hWFr0GcwHgkfJi2EXbte0SzXjIs+W8MRy6ZhVZUyJcsNtl+wt3WRtmpZLOa0rsGmFq8Cq2qNzRStbymrZXSuKzBJwny52GCCMIZWSfNy2BvE80HQxkku/BHnfGTXCk1dKRGa9MF16WLTw3iecSqShYrjrK6ZJpexNKbEy1Mg1N0JorWm9iVtZ4LbOoKLjEGj8SEw3t0WOnFEWAYnfiOuaaNOgGh/RndPAfe4gFcuIubChgtitEIHvdFZzI2M7hKTYG1KauRnJsaS5z1sNCJKjNwN2tFASvdW+g/GGLI8Jy16DOyWTC1iGDqymaKpKrIip6xFat5E4JUPsfFlNKpjxjrhk9SuJamhbRqMshibMZ/PmU6nm2NXFMIYLYp8o+qd9wqRsksMh4eHG+ZsmudcunRJqPEU2G68G3sSaWKpFtXG4BlO+CWdGE/bttStCBbt7u7y3rs3efLkCUmaiEZpdDZLi3yzxeiSXYdj2cgdumYDqS+KAt+0zGYzqqrEe9nbaw1FkTEcFAx7FnwlxynKCXrEEaypWvxiTXO8oDqeM69XlFXFeHvChfMXuX7tOs16m5s3b3Kw/5TGyzZr3azBazJj6emCYOB4MeNcvYUyisVCFOYTazcSAsCGMr8qK46PZyR5sVFU68Bv3oFWdtOnUNFHVZ0CHc5TkSw6i3mloHU1bVuTGplIuLbeNAOVOtEkBDn4OE+Is3wC1OuSpTEbh2qbaCyKxgd83dCWFZaTLJ1qQxrv5kZprLKRaxA1M7XGdC5kUchGY9BOeCXtuqJciYJ4rWvqskJlGYmJhr1K0+sNKcsSlYFVMk1J8pyi15PKQfEMIlQSWQB87KU4ZNxKBBOFgND103TzKCN8vSxLmHqUN7RZy3BoWMzmzKczQbA6v0kWvSKnrFYsl0vBfqSWq1evcu/2PabTI27edGS9gjQTWPV41IsEPHDKoeOoujP/baITWVO31FVD7VoOnh7x+PE+0+MZ4/EWTdOwWq1IspS0l21EjYuiiCNDh/dmU2J3VPMO2Zin6YbtCl4g+/M5nkDbNmhtGU8GTMaXOLc7wVVLnjy6x2y1pGhGjHo92SKWNbp0KFdz960bPHz6iFloWBpPpRTpsM/cl1wY9Rn0c9arDK1EfV4dadZVSVUFiiYnywzzcsHdR/dYz+esVzOOj4+ZjMfYyCzOE9ENHQ0nLFZPmM1mYv48GtHrCWGtXK1oW/FTVcoiVHkDQaNUh+J8fknjVCQLgbZC41qyvCAEmQ60rt6Al07EcFoMltRovAevNS7qJmitMWhC61jNhSylBNcIjUO7gGo9CkEYKiUsUKssiU6wRmOjTJ6KO0YVAsoJlNNHBe350TGz4ymL4wXz6YLlbC78jrLFGsOw16ctsk15nnrZGnnv8VGjIUkzQoDFYnmCwfBiBq3DiZ1jBx4LWuEjv6QTb+30PrvtxPx4yvHBIT2lUN7iikBqc9aLJW1Vg9Ib0Bgg0vZemI11LZYCV65cYXZ8zPRYZPTv3LnD9vY2xlr2Lp0D/AYPorzHOUkQbeNoG4d3XYPWRpGdEyGf8fYWR4dTpvMZZVlz/sIug9GQ4XAomqvWih4GbLadoj9yQtp71hlusVhwdHjEar0QNfVxwXi0xe72NlvjEYN+zuH+Q548DqzqioPDQ1DSa1kcHOKnc7RNaTKF8iXjrT42U+yXKw5mxxzMp1wdQC/XKOVofE2jHLqQ8XowjpKKohjQtA13H93HVSXKtTx9+pTxSBTdKicizoPBgPF4zOOnByxmC5raM1xXkrh7AzLbyRtoqS5wMv3ZUNSfb3VxKpJF5GpHTclOZUn2pxv0oA9yF25aQhqJXW0roKm6obA5SYRAq6Boy4oyYv6VDpvtivKBpqlp4jh0lS5ok/aDXXbYVBUdRl+pjj7ecnx0zHK+pCkbjNdYndBUDcEFVvPVprfgnLBWD2dz8jxnuZqjlPipdkIyaWo3I1AZ9/oT4FPXB9goO0f4ePxqjMEoRWotiTYsqzXr5YrhTj8muZPeTJamtBFz0MGYe70cm4q0P8DjRw+YbI25du0a3//eDblrHx1z48YNjFFcv/4i/Twj+IAJDhU8VdOio3Fwl/Da1ouYcdXwne98h4cPHrFz7jzndsXAOs9lejSaDJlMJjIB6PUwUdjYxy2QEO1OhGi686HT3GiahulUDJjbtubSC5d44YXLjEZD2rqkrldUzZoQGnbOnWe5XPL22+/QLNe00yXDAGb3PJNxRlANoTBgLApPVZfM1gvOn58wm2/x4PF9ZvM5rVYUk4yEFI/ohpShBhrWi6k0l1VgenwsxLzaMZ8uROJQJ/T7Q/q9AcezOet1hbIrmjrQlI7RaCTIXC2GVSB8JeDjR6fKfyrArD8wWSilrgB/C7iIEOl/PoTwXyulfg74d4H9+NK/FEL4v+N7/iLw5wAH/AchhF/8uN8RQhCyjhI1KB1HRamVPa3Rcocd9AoZDSaGqlyLcZCxGAsJmtwkWCOApExbfOOomwWrcomP5kBVVVI1ddxjK2zjSZIIPlL2A/gMYwyJ1ZteCrGHkaucKjRYr9EOjDfgIVUJOmh8I6jBxKQYk7I7HnN4eAiIpuR7+7fpFRnnz5/HlTV5llH0LY1rBUgUXPx9htoYiiTDKk2IehPWGHA1aItF088KkpHGNJ5BmmNaBXVLGyrKxRrlPEWWc3h4jFFWiHO1KEtneYrNUgrleeGFF/iNX/t1Ll+6zI/+2Bt859tvMp9PWb2z4OnTR3z+C6/x2vWrdBAAnVh08DK5UCoeRznJF6uSsqzZf/KUrZ1drr58nQcPHvDezVssl0t2zp3jtdde4/yFHSY7Mpr0Sn5OXde0rt4gcjulaw0MBgO0FguIqqrYPzxgWa7oDwa89vlr9Pt9nG9pXI1JHVmuGO+M+Bf++Z9md2uXr/8vf4e//3/9PXazPrWDB3cfcm58nVy3rKsKTMMgNegA0/sPufve96jXK5LMY9tA6Rta1bJqa7CG9XzOwf4TBmlKYgPWB6y2/MZv/AZvv/022+NtvvC5P8GVvcusVw2vXHuF+bJkubrJdL6gcWDVilXeI7OFKLWlnsTmKGoIdgP3/gCZrBO8+ZSEb+CTVRYt8J+EEH5HKTUEvqmU+qX4f/9VCOG/ePbFSqkvAD8D/AlgD/h/lFKvhRAcHxHS1a7pTGs6ll3H7y/yHrP5lDzPqUvpD0iJKvgKEk2aJHHMFEijmZD2IZoJicHNarGkXC1pkSqlyAoSI4YzOhiKKITjvd8I4XQTjW4/Lc2EyBtpHHXZsF6Ke3eW5BiTxGpAjGtEUbwiMSm9XspyLXobi/mKprzLqDdgPOwzzDK0F2i3IsTmFuBDFMyR3k7rIhLDC1pSB3HHCo1YA5SLJb1Rb9OfmB9PKbKCfl5wEI6AyE+pRcW7a0I2jSLNBT7+6NEjdnfPsffCRW7fuisTh8UC76UCa+tqAxRzMQnLxEL2NyI4JEIzFy/ucXHvEuuyZDqfsVjMUCaR6qrfo+j3RROjrVGGE7yJc2Jw3GmJGjkvOmm+5XJJHdmjAJOdCb1RgdIQygabAIgSN4j5cj/vc/Wll5lMtjh4/ISgc4w10hTOE0pfk2DJewNG1oJK+N5b36VsGx5PD1mowGG9kvF73PplRUKWakLE0GQ6QUXW7Wy64Ee+8CNsbW2hMPR6Cb3egPF4izx/zHJVgfO03d/ERTyPXAVobTHRRe95K3vDJ0gWIYSHwMP4/Vwp9T3ghY95y08DfzuEUAE3lVLvAl8F/tHH/Z6PEiXdcD0w+Lg16Lr6yjtQYSNTp7sx07PvF8rCiWtUkKmC0VpOrNARxcTIVyslDaVOp8ILcatrOsrP1Oig5GfKM5v+QQfX7SDriU25sneJF154gdbA06dPODo64s6tm9x6/ybr6Zx2NWLSExJVqg3aCq+jbVz87LKWxgeZ2oRAnqa0HnKbEJoWozQmxDXHNYlP6wlDtRO5fVZMV9YsIjLlasF4POboaErTNOSpjDFnsxlZT6jz3YWslcJp8Wft+iday+m0XEqj9enTp1SNAOEOD4+YTqfoRJL/s4pkQBQUOrl7ynrDyXFMEnBseljEnlOSJBSFTBW0Bq09QYu/qwonif7Rg4e8cu06u7u7XLi4h1+3WOdZr9Zk/R6TCyO2e5p14pk3NQ8fH3A8XbIebGN6GT60JHlKohMaJdwiH5w0vU2E77ctlQblRCphPByyNd6mn/di8hMNkmFP/GqXqzUuuqx16mhFUfD7exPdv59vwlB/GJ68Uuoq8CvAF4H/GPi3gRnwDaT6OFJK/bfAb4YQ/sf4nr8O/N0Qwv/6Az/rzwN/Pv7zdeAAePpH+CyfZuzy2VkrfLbW+1laK3y21vt6CGH4T/rmT9zgVEoNgP8N+I9CCDOl1F8D/gpyw/0rwF8F/h0+HDny+zJSCOHngZ9/5ud/I4TwJ/9wy38+8VlaK3y21vtZWit8ttarlPrGH+X9n6iFqpRKkETxP4UQ/neAEMLjEIILIXjgv0e2GgD3gCvPvP0y8OCPssizOIuzeP7xByYLJRvcvw58L4TwXz7z/KVnXvavAt+N3/8C8DNKqUwpdQ14FfjHP7wln8VZnMXziE+yDflJ4N8EvqOU+lZ87i8B/7pS6keRLcYt4N8DCCG8qZT6O8BbyCTlL3zcJOSZ+Pk/+CWnJj5La4XP1no/S2uFz9Z6/0hr/UM1OM/iLM7i/7/x/NkpZ3EWZ/GZiOeeLJRS/7JS6m2l1LtKqZ993uv5sFBK3VJKfUcp9a2uo6yU2lZK/ZJS6p34des5re1vKKWeKKW++8xzH7o2JfHfxGP9baXUl0/Jen9OKXU/Ht9vKaV+6pn/+4txvW8rpf6lT3mtV5RS/0Ap9T2l1JtKqf8wPn/qju/HrPWHd2yfVRD+tB+AAd4DXgZS4PeALzzPNX3EOm8Buz/w3H8O/Gz8/meB/+w5re1rwJeB7/5BawN+Cvi7yHj7J4DfOiXr/TngP/2Q134hnhMZcC2eK+ZTXOsl4Mvx+yFwI67p1B3fj1nrD+3YPu/K4qvAuyGE90MINfC3EQToZyF+Gvib8fu/Cfwrz2MRIYRfAQ5/4OmPWttPA38rSPwmMPmBqdYfe3zEej8qNmjgEMJNoEMDfyoRQngYQvid+P0c6NDLp+74fsxaPyr+0Mf2eSeLF4C7z/z7Hh//AZ9XBODvK6W+GZGnABeCQOGJX88/t9X9/viotZ3m4/3vx9L9bzyzpTs1643o5R8DfotTfnx/YK3wQzq2zztZfCK05ymInwwhfBn4M8BfUEp97Xkv6J8wTuvx/mvAK8CPIjykvxqfPxXr/UH08se99EOe+1TX+yFr/aEd2+edLD4TaM8QwoP49QnwfyDl2uOuxIxfnzy/Ff6++Ki1ncrjHU4xGvjD0Muc0uP7x420ft7J4reBV5VS15RSKUJt/4XnvKYPhFKqr4Saj1KqD/yLCFr1F4A/G1/2Z4H/8/ms8EPjo9b2C8C/Fbv2PwFMu3L6ecZpRQN/FHqZU3h8PxWk9afVrf2YLu5PIZ3b94C//LzX8yHrexnpGv8e8Ga3RmAH+H+Bd+LX7ee0vv8ZKS8b5G7x5z5qbUjp+d/FY/0d4E+ekvX+D3E9344n8aVnXv+X43rfBv7Mp7zWP42U5t8GvhUfP3Uaj+/HrPWHdmzPEJxncRZn8YnieW9DzuIszuIzEmfJ4izO4iw+UZwli7M4i7P4RHGWLM4joBm1AAAAMUlEQVTiLM7iE8VZsjiLsziLTxRnyeIszuIsPlGcJYuzOIuz+ERxlizO4izO4hPF/we3OBIyHE9wpwAAAABJRU5ErkJggg==
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
<p>Before using any of the face detectors, it is standard procedure to convert the images to grayscale.  The <code>detectMultiScale</code> function executes the classifier stored in <code>face_cascade</code> and takes the grayscale image as a parameter.</p>
<p>In the above code, <code>faces</code> is a numpy array of detected faces, where each row corresponds to a detected face.  Each detected face is a 1D array with four entries that specifies the bounding box of the detected face.  The first two entries in the array (extracted in the above code as <code>x</code> and <code>y</code>) specify the horizontal and vertical positions of the top left corner of the bounding box.  The last two entries in the array (extracted here as <code>w</code> and <code>h</code>) specify the width and height of the box.</p>
<h3 id="Write-a-Human-Face-Detector">Write a Human Face Detector<a class="anchor-link" href="#Write-a-Human-Face-Detector">&#182;</a></h3><p>We can use this procedure to write a function that returns <code>True</code> if a human face is detected in an image and <code>False</code> otherwise.  This function, aptly named <code>face_detector</code>, takes a string-valued file path to an image as input and appears in the code block below.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[18]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># returns &quot;True&quot; if face is detected in image stored at img_path</span>
<span class="k">def</span> <span class="nf">face_detector</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="n">img</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span>
    <span class="n">gray</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">cvtColor</span><span class="p">(</span><span class="n">img</span><span class="p">,</span> <span class="n">cv2</span><span class="o">.</span><span class="n">COLOR_BGR2GRAY</span><span class="p">)</span>
    <span class="n">faces</span> <span class="o">=</span> <span class="n">face_cascade</span><span class="o">.</span><span class="n">detectMultiScale</span><span class="p">(</span><span class="n">gray</span><span class="p">)</span>
    <span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="n">faces</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Assess-the-Human-Face-Detector">(IMPLEMENTATION) Assess the Human Face Detector<a class="anchor-link" href="#(IMPLEMENTATION)-Assess-the-Human-Face-Detector">&#182;</a></h3><p><strong>Question 1:</strong> Use the code cell below to test the performance of the <code>face_detector</code> function.</p>
<ul>
<li>What percentage of the first 100 images in <code>human_files</code> have a detected human face?  </li>
<li>What percentage of the first 100 images in <code>dog_files</code> have a detected human face? </li>
</ul>
<p>Ideally, we would like 100% of human images with a detected face and 0% of dog images with a detected face.  You will see that our algorithm falls short of this goal, but still gives acceptable performance.  We extract the file paths for the first 100 images from each of the datasets and store them in the numpy arrays <code>human_files_short</code> and <code>dog_files_short</code>.</p>
<p><strong>Answer:</strong>  100.0 % of the first 100 images in human_files have a detected human face
11.0 % of the first 100 images in dog_files have a detected human face</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[25]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">human_files_short</span> <span class="o">=</span> <span class="n">human_files</span><span class="p">[:</span><span class="mi">100</span><span class="p">]</span>
<span class="n">dog_files_short</span> <span class="o">=</span> <span class="n">train_files</span><span class="p">[:</span><span class="mi">100</span><span class="p">]</span>
<span class="c1"># Do NOT modify the code above this line.</span>

<span class="k">def</span> <span class="nf">calculate_percentage</span><span class="p">(</span><span class="n">file_short</span><span class="p">,</span><span class="n">func_name</span><span class="p">):</span>
    <span class="n">total_face_detected</span> <span class="o">=</span> <span class="mi">0</span>
    <span class="k">for</span> <span class="n">image</span> <span class="ow">in</span> <span class="n">file_short</span><span class="p">:</span>
        <span class="k">if</span> <span class="n">func_name</span><span class="p">(</span><span class="n">image</span><span class="p">):</span>
            <span class="n">total_face_detected</span> <span class="o">+=</span> <span class="mi">1</span>
        
    <span class="n">total_percent</span> <span class="o">=</span> <span class="p">(</span><span class="n">total_face_detected</span> <span class="o">/</span><span class="nb">len</span><span class="p">(</span><span class="n">file_short</span><span class="p">))</span><span class="o">*</span> <span class="mi">100</span>
    <span class="k">return</span> <span class="n">total_percent</span>

<span class="n">percent</span> <span class="o">=</span> <span class="n">calculate_percentage</span><span class="p">(</span><span class="n">human_files_short</span><span class="p">,</span><span class="n">face_detector</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">percent</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot; </span><span class="si">% o</span><span class="s2">f the first 100 images in human_files have a detected human face&quot;</span><span class="p">)</span>

<span class="n">percent</span> <span class="o">=</span> <span class="n">calculate_percentage</span><span class="p">(</span><span class="n">dog_files_short</span><span class="p">,</span><span class="n">face_detector</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">percent</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot; </span><span class="si">% o</span><span class="s2">f the first 100 images in dog_files have a detected human face&quot;</span><span class="p">)</span>
    
<span class="c1">## TODO: Test the performance of the face_detector algorithm </span>
<span class="c1">## on the images in human_files_short and dog_files_short.</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>100.0 % of the first 100 images in human_files have a detected human face
11.0 % of the first 100 images in dog_files have a detected human face
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
<p><strong>Question 2:</strong> This algorithmic choice necessitates that we communicate to the user that we accept human images only when they provide a clear view of a face (otherwise, we risk having unneccessarily frustrated users!). In your opinion, is this a reasonable expectation to pose on the user? If not, can you think of a way to detect humans in images that does not necessitate an image with a clearly presented face?</p>
<p><strong>Answer:</strong></p>
<p>We suggest the face detector from OpenCV as a potential way to detect human images in your algorithm, but you are free to explore other approaches, especially approaches that make use of deep learning :).  Please use the code cell below to design and test your own face detection algorithm.  If you decide to pursue this <em>optional</em> task, report performance on each of the datasets.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[&nbsp;]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">## (Optional) TODO: Report the performance of another  </span>
<span class="c1">## face detection algorithm on the LFW dataset</span>
<span class="c1">### Feel free to use as many code cells as needed.</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<p><a id='step2'></a></p>
<h2 id="Step-2:-Detect-Dogs">Step 2: Detect Dogs<a class="anchor-link" href="#Step-2:-Detect-Dogs">&#182;</a></h2><p>In this section, we use a pre-trained <a href="http://ethereon.github.io/netscope/#/gist/db945b393d40bfa26006">ResNet-50</a> model to detect dogs in images.  Our first line of code downloads the ResNet-50 model, along with weights that have been trained on <a href="http://www.image-net.org/">ImageNet</a>, a very large, very popular dataset used for image classification and other vision tasks.  ImageNet contains over 10 million URLs, each linking to an image containing an object from one of <a href="https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a">1000 categories</a>.  Given an image, this pre-trained ResNet-50 model returns a prediction (derived from the available categories in ImageNet) for the object that is contained in the image.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[20]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">keras.applications.resnet50</span> <span class="k">import</span> <span class="n">ResNet50</span>

<span class="c1"># define ResNet50 model</span>
<span class="n">ResNet50_model</span> <span class="o">=</span> <span class="n">ResNet50</span><span class="p">(</span><span class="n">weights</span><span class="o">=</span><span class="s1">&#39;imagenet&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Downloading data from https://github.com/fchollet/deep-learning-models/releases/download/v0.2/resnet50_weights_tf_dim_ordering_tf_kernels.h5
102858752/102853048 [==============================] - 2s 0us/step
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
<h3 id="Pre-process-the-Data">Pre-process the Data<a class="anchor-link" href="#Pre-process-the-Data">&#182;</a></h3><p>When using TensorFlow as backend, Keras CNNs require a 4D array (which we'll also refer to as a 4D tensor) as input, with shape</p>
<p>$$
(\text{nb_samples}, \text{rows}, \text{columns}, \text{channels}),
$$</p>
<p>where <code>nb_samples</code> corresponds to the total number of images (or samples), and <code>rows</code>, <code>columns</code>, and <code>channels</code> correspond to the number of rows, columns, and channels for each image, respectively.</p>
<p>The <code>path_to_tensor</code> function below takes a string-valued file path to a color image as input and returns a 4D tensor suitable for supplying to a Keras CNN.  The function first loads the image and resizes it to a square image that is $224 \times 224$ pixels.  Next, the image is converted to an array, which is then resized to a 4D tensor.  In this case, since we are working with color images, each image has three channels.  Likewise, since we are processing a single image (or sample), the returned tensor will always have shape</p>
<p>$$
(1, 224, 224, 3).
$$</p>
<p>The <code>paths_to_tensor</code> function takes a numpy array of string-valued image paths as input and returns a 4D tensor with shape</p>
<p>$$
(\text{nb_samples}, 224, 224, 3).
$$</p>
<p>Here, <code>nb_samples</code> is the number of samples, or number of images, in the supplied array of image paths.  It is best to think of <code>nb_samples</code> as the number of 3D tensors (where each 3D tensor corresponds to a different image) in your dataset!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[21]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">keras.preprocessing</span> <span class="k">import</span> <span class="n">image</span>                  
<span class="kn">from</span> <span class="nn">tqdm</span> <span class="k">import</span> <span class="n">tqdm</span>

<span class="k">def</span> <span class="nf">path_to_tensor</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="c1"># loads RGB image as PIL.Image.Image type</span>
    <span class="n">img</span> <span class="o">=</span> <span class="n">image</span><span class="o">.</span><span class="n">load_img</span><span class="p">(</span><span class="n">img_path</span><span class="p">,</span> <span class="n">target_size</span><span class="o">=</span><span class="p">(</span><span class="mi">224</span><span class="p">,</span> <span class="mi">224</span><span class="p">))</span>
    <span class="c1"># convert PIL.Image.Image type to 3D tensor with shape (224, 224, 3)</span>
    <span class="n">x</span> <span class="o">=</span> <span class="n">image</span><span class="o">.</span><span class="n">img_to_array</span><span class="p">(</span><span class="n">img</span><span class="p">)</span>
    <span class="c1"># convert 3D tensor to 4D tensor with shape (1, 224, 224, 3) and return 4D tensor</span>
    <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">expand_dims</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">paths_to_tensor</span><span class="p">(</span><span class="n">img_paths</span><span class="p">):</span>
    <span class="n">list_of_tensors</span> <span class="o">=</span> <span class="p">[</span><span class="n">path_to_tensor</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span> <span class="k">for</span> <span class="n">img_path</span> <span class="ow">in</span> <span class="n">tqdm</span><span class="p">(</span><span class="n">img_paths</span><span class="p">)]</span>
    <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">vstack</span><span class="p">(</span><span class="n">list_of_tensors</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Making-Predictions-with-ResNet-50">Making Predictions with ResNet-50<a class="anchor-link" href="#Making-Predictions-with-ResNet-50">&#182;</a></h3><p>Getting the 4D tensor ready for ResNet-50, and for any other pre-trained model in Keras, requires some additional processing.  First, the RGB image is converted to BGR by reordering the channels.  All pre-trained models have the additional normalization step that the mean pixel (expressed in RGB as $[103.939, 116.779, 123.68]$ and calculated from all pixels in all images in ImageNet) must be subtracted from every pixel in each image.  This is implemented in the imported function <code>preprocess_input</code>.  If you're curious, you can check the code for <code>preprocess_input</code> <a href="https://github.com/fchollet/keras/blob/master/keras/applications/imagenet_utils.py">here</a>.</p>
<p>Now that we have a way to format our image for supplying to ResNet-50, we are now ready to use the model to extract the predictions.  This is accomplished with the <code>predict</code> method, which returns an array whose $i$-th entry is the model's predicted probability that the image belongs to the $i$-th ImageNet category.  This is implemented in the <code>ResNet50_predict_labels</code> function below.</p>
<p>By taking the argmax of the predicted probability vector, we obtain an integer corresponding to the model's predicted object class, which we can identify with an object category through the use of this <a href="https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a">dictionary</a>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[23]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">keras.applications.resnet50</span> <span class="k">import</span> <span class="n">preprocess_input</span><span class="p">,</span> <span class="n">decode_predictions</span>

<span class="k">def</span> <span class="nf">ResNet50_predict_labels</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="c1"># returns prediction vector for image located at img_path</span>
    <span class="n">img</span> <span class="o">=</span> <span class="n">preprocess_input</span><span class="p">(</span><span class="n">path_to_tensor</span><span class="p">(</span><span class="n">img_path</span><span class="p">))</span>
    <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">ResNet50_model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">img</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Write-a-Dog-Detector">Write a Dog Detector<a class="anchor-link" href="#Write-a-Dog-Detector">&#182;</a></h3><p>While looking at the <a href="https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a">dictionary</a>, you will notice that the categories corresponding to dogs appear in an uninterrupted sequence and correspond to dictionary keys 151-268, inclusive, to include all categories from <code>'Chihuahua'</code> to <code>'Mexican hairless'</code>.  Thus, in order to check to see if an image is predicted to contain a dog by the pre-trained ResNet-50 model, we need only check if the <code>ResNet50_predict_labels</code> function above returns a value between 151 and 268 (inclusive).</p>
<p>We use these ideas to complete the <code>dog_detector</code> function below, which returns <code>True</code> if a dog is detected in an image (and <code>False</code> if not).</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### returns &quot;True&quot; if a dog is detected in the image stored at img_path</span>
<span class="k">def</span> <span class="nf">dog_detector</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="n">prediction</span> <span class="o">=</span> <span class="n">ResNet50_predict_labels</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span>
    <span class="k">return</span> <span class="p">((</span><span class="n">prediction</span> <span class="o">&lt;=</span> <span class="mi">268</span><span class="p">)</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">prediction</span> <span class="o">&gt;=</span> <span class="mi">151</span><span class="p">))</span> 
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Assess-the-Dog-Detector">(IMPLEMENTATION) Assess the Dog Detector<a class="anchor-link" href="#(IMPLEMENTATION)-Assess-the-Dog-Detector">&#182;</a></h3><p><strong>Question 3:</strong> Use the code cell below to test the performance of your <code>dog_detector</code> function.</p>
<ul>
<li>What percentage of the images in <code>human_files_short</code> have a detected dog?  </li>
<li>What percentage of the images in <code>dog_files_short</code> have a detected dog?</li>
</ul>
<p><strong>Answer:</strong>  0.0 % of the first 100 images in human_files have a detected dog
100.0 % of the first 100 images in dog_files have a detected dog</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[27]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Test the performance of the dog_detector function</span>
<span class="c1">### on the images in human_files_short and dog_files_short.</span>

<span class="n">percent</span> <span class="o">=</span> <span class="n">calculate_percentage</span><span class="p">(</span><span class="n">human_files_short</span><span class="p">,</span><span class="n">dog_detector</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">percent</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot; </span><span class="si">% o</span><span class="s2">f the first 100 images in human_files have a detected dog&quot;</span><span class="p">)</span>

<span class="n">percent</span> <span class="o">=</span> <span class="n">calculate_percentage</span><span class="p">(</span><span class="n">dog_files_short</span><span class="p">,</span><span class="n">dog_detector</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">percent</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot; </span><span class="si">% o</span><span class="s2">f the first 100 images in dog_files have a detected dog&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>0.0 % of the first 100 images in human_files have a detected dog
100.0 % of the first 100 images in dog_files have a detected dog
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
<hr>
<p><a id='step3'></a></p>
<h2 id="Step-3:-Create-a-CNN-to-Classify-Dog-Breeds-(from-Scratch)">Step 3: Create a CNN to Classify Dog Breeds (from Scratch)<a class="anchor-link" href="#Step-3:-Create-a-CNN-to-Classify-Dog-Breeds-(from-Scratch)">&#182;</a></h2><p>Now that we have functions for detecting humans and dogs in images, we need a way to predict breed from images.  In this step, you will create a CNN that classifies dog breeds.  You must create your CNN <em>from scratch</em> (so, you can't use transfer learning <em>yet</em>!), and you must attain a test accuracy of at least 1%.  In Step 5 of this notebook, you will have the opportunity to use transfer learning to create a CNN that attains greatly improved accuracy.</p>
<p>Be careful with adding too many trainable layers!  More parameters means longer training, which means you are more likely to need a GPU to accelerate the training process.  Thankfully, Keras provides a handy estimate of the time that each epoch is likely to take; you can extrapolate this estimate to figure out how long it will take for your algorithm to train.</p>
<p>We mention that the task of assigning breed to dogs from images is considered exceptionally challenging.  To see why, consider that <em>even a human</em> would have great difficulty in distinguishing between a Brittany and a Welsh Springer Spaniel.</p>
<table>
<thead><tr>
<th>Brittany</th>
<th>Welsh Springer Spaniel</th>
</tr>
</thead>
<tbody>
<tr>
<td><img src="images/Brittany_02625.jpg" width="100"></td>
<td><img src="images/Welsh_springer_spaniel_08203.jpg" width="200"></td>
</tr>
</tbody>
</table>
<p>It is not difficult to find other dog breed pairs with minimal inter-class variation (for instance, Curly-Coated Retrievers and American Water Spaniels).</p>
<table>
<thead><tr>
<th>Curly-Coated Retriever</th>
<th>American Water Spaniel</th>
</tr>
</thead>
<tbody>
<tr>
<td><img src="images/Curly-coated_retriever_03896.jpg" width="200"></td>
<td><img src="images/American_water_spaniel_00648.jpg" width="200"></td>
</tr>
</tbody>
</table>
<p>Likewise, recall that labradors come in yellow, chocolate, and black.  Your vision-based algorithm will have to conquer this high intra-class variation to determine how to classify all of these different shades as the same breed.</p>
<table>
<thead><tr>
<th>Yellow Labrador</th>
<th>Chocolate Labrador</th>
<th>Black Labrador</th>
</tr>
</thead>
<tbody>
<tr>
<td><img src="images/Labrador_retriever_06457.jpg" width="150"></td>
<td><img src="images/Labrador_retriever_06455.jpg" width="240"></td>
<td><img src="images/Labrador_retriever_06449.jpg" width="220"></td>
</tr>
</tbody>
</table>
<p>We also mention that random chance presents an exceptionally low bar: setting aside the fact that the classes are slightly imabalanced, a random guess will provide a correct answer roughly 1 in 133 times, which corresponds to an accuracy of less than 1%.</p>
<p>Remember that the practice is far ahead of the theory in deep learning.  Experiment with many different architectures, and trust your intuition.  And, of course, have fun!</p>
<h3 id="Pre-process-the-Data">Pre-process the Data<a class="anchor-link" href="#Pre-process-the-Data">&#182;</a></h3><p>We rescale the images by dividing every pixel in every image by 255.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[28]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">PIL</span> <span class="k">import</span> <span class="n">ImageFile</span>                            
<span class="n">ImageFile</span><span class="o">.</span><span class="n">LOAD_TRUNCATED_IMAGES</span> <span class="o">=</span> <span class="kc">True</span>                 

<span class="c1"># pre-process the data for Keras</span>
<span class="n">train_tensors</span> <span class="o">=</span> <span class="n">paths_to_tensor</span><span class="p">(</span><span class="n">train_files</span><span class="p">)</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="s1">&#39;float32&#39;</span><span class="p">)</span><span class="o">/</span><span class="mi">255</span>
<span class="n">valid_tensors</span> <span class="o">=</span> <span class="n">paths_to_tensor</span><span class="p">(</span><span class="n">valid_files</span><span class="p">)</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="s1">&#39;float32&#39;</span><span class="p">)</span><span class="o">/</span><span class="mi">255</span>
<span class="n">test_tensors</span> <span class="o">=</span> <span class="n">paths_to_tensor</span><span class="p">(</span><span class="n">test_files</span><span class="p">)</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="s1">&#39;float32&#39;</span><span class="p">)</span><span class="o">/</span><span class="mi">255</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stderr output_text">
<pre>100%|██████████| 6680/6680 [01:11&lt;00:00, 93.90it/s] 
100%|██████████| 835/835 [00:07&lt;00:00, 105.29it/s]
100%|██████████| 836/836 [00:07&lt;00:00, 105.86it/s]
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
<h3 id="(IMPLEMENTATION)-Model-Architecture">(IMPLEMENTATION) Model Architecture<a class="anchor-link" href="#(IMPLEMENTATION)-Model-Architecture">&#182;</a></h3><p>Create a CNN to classify dog breed.  At the end of your code cell block, summarize the layers of your model by executing the line:</p>

<pre><code>    model.summary()

</code></pre>
<p>We have imported some Python modules to get you started, but feel free to import as many modules as you need.  If you end up getting stuck, here's a hint that specifies a model that trains relatively fast on CPU and attains &gt;1% test accuracy in 5 epochs:</p>
<p><img src="images/sample_cnn.png" alt="Sample CNN"></p>
<p><strong>Question 4:</strong> Outline the steps you took to get to your final CNN architecture and your reasoning at each step.  If you chose to use the hinted architecture above, describe why you think that CNN architecture should work well for the image classification task.</p>
<p><strong>Answer:</strong>   The idea of CNN is to use multiple layers to extract different features from the images. In my model I used a simple stack of three convolution layers with a ReLU activation and followed by max-pooling layers. I tried adding fragment with more filter but it didnot improve the accuracy but reduced the epoch speed. Pooling layers simplify the information in the output from the convolutional layer. Max-pooling outputs the maximum value</p>
<p>These layers will help the model to extract complex features to understand the difference between different dog breads.  Next the GAP layer is used to reduce the spatial dimensions of a three-dimensional tensor which can help in preventing overfitting. The final layer of CNN is a dense layer with softmax activation is used to classify the output into 133 classes.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[42]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">keras.layers</span> <span class="k">import</span> <span class="n">Conv2D</span><span class="p">,</span> <span class="n">MaxPooling2D</span><span class="p">,</span> <span class="n">GlobalAveragePooling2D</span>
<span class="kn">from</span> <span class="nn">keras.layers</span> <span class="k">import</span> <span class="n">Dropout</span><span class="p">,</span> <span class="n">Flatten</span><span class="p">,</span> <span class="n">Dense</span>
<span class="kn">from</span> <span class="nn">keras.models</span> <span class="k">import</span> <span class="n">Sequential</span>

<span class="n">model</span> <span class="o">=</span> <span class="n">Sequential</span><span class="p">()</span>
<span class="n">num_classes</span><span class="o">=</span><span class="mi">133</span>

<span class="c1">### TODO: Define your architecture.</span>
<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Conv2D</span><span class="p">(</span><span class="mi">16</span><span class="p">,</span> <span class="n">kernel_size</span><span class="o">=</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">5</span><span class="p">),</span> <span class="n">strides</span><span class="o">=</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span> <span class="n">padding</span><span class="o">=</span><span class="s1">&#39;same&#39;</span><span class="p">,</span> <span class="n">activation</span><span class="o">=</span><span class="s1">&#39;relu&#39;</span><span class="p">,</span> <span class="n">input_shape</span><span class="o">=</span><span class="p">(</span><span class="mi">224</span><span class="p">,</span> <span class="mi">224</span><span class="p">,</span> <span class="mi">3</span><span class="p">),</span><span class="n">data_format</span><span class="o">=</span><span class="s2">&quot;channels_last&quot;</span><span class="p">))</span>
<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">MaxPooling2D</span><span class="p">(</span><span class="n">pool_size</span><span class="o">=</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">),</span> <span class="n">strides</span><span class="o">=</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Conv2D</span><span class="p">(</span><span class="mi">32</span><span class="p">,</span> <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="mi">3</span><span class="p">),</span><span class="n">padding</span><span class="o">=</span><span class="s1">&#39;same&#39;</span><span class="p">,</span> <span class="n">activation</span><span class="o">=</span><span class="s1">&#39;relu&#39;</span><span class="p">))</span>
<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">MaxPooling2D</span><span class="p">(</span><span class="n">pool_size</span><span class="o">=</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Conv2D</span><span class="p">(</span><span class="mi">64</span><span class="p">,</span> <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="mi">3</span><span class="p">),</span><span class="n">padding</span><span class="o">=</span><span class="s1">&#39;same&#39;</span><span class="p">,</span> <span class="n">activation</span><span class="o">=</span><span class="s1">&#39;relu&#39;</span><span class="p">))</span>
<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">MaxPooling2D</span><span class="p">(</span><span class="n">pool_size</span><span class="o">=</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>

<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">GlobalAveragePooling2D</span><span class="p">())</span>

<span class="n">model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Dense</span><span class="p">(</span><span class="n">num_classes</span><span class="p">,</span> <span class="n">activation</span><span class="o">=</span><span class="s1">&#39;softmax&#39;</span><span class="p">))</span>


<span class="n">model</span><span class="o">.</span><span class="n">summary</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_20 (Conv2D)           (None, 224, 224, 16)      1216      
_________________________________________________________________
max_pooling2d_21 (MaxPooling (None, 112, 112, 16)      0         
_________________________________________________________________
conv2d_21 (Conv2D)           (None, 112, 112, 32)      4640      
_________________________________________________________________
max_pooling2d_22 (MaxPooling (None, 56, 56, 32)        0         
_________________________________________________________________
conv2d_22 (Conv2D)           (None, 56, 56, 64)        18496     
_________________________________________________________________
max_pooling2d_23 (MaxPooling (None, 28, 28, 64)        0         
_________________________________________________________________
global_average_pooling2d_6 ( (None, 64)                0         
_________________________________________________________________
dense_10 (Dense)             (None, 133)               8645      
=================================================================
Total params: 32,997
Trainable params: 32,997
Non-trainable params: 0
_________________________________________________________________
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
<h3 id="Compile-the-Model">Compile the Model<a class="anchor-link" href="#Compile-the-Model">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[43]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">model</span><span class="o">.</span><span class="n">compile</span><span class="p">(</span><span class="n">optimizer</span><span class="o">=</span><span class="s1">&#39;rmsprop&#39;</span><span class="p">,</span> <span class="n">loss</span><span class="o">=</span><span class="s1">&#39;categorical_crossentropy&#39;</span><span class="p">,</span> <span class="n">metrics</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;accuracy&#39;</span><span class="p">])</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Train-the-Model">(IMPLEMENTATION) Train the Model<a class="anchor-link" href="#(IMPLEMENTATION)-Train-the-Model">&#182;</a></h3><p>Train your model in the code cell below.  Use model checkpointing to save the model that attains the best validation loss.</p>
<p>You are welcome to <a href="https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html">augment the training data</a>, but this is not a requirement.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[44]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">keras.callbacks</span> <span class="k">import</span> <span class="n">ModelCheckpoint</span>  

<span class="c1">### TODO: specify the number of epochs that you would like to use to train the model.</span>

<span class="n">epochs</span> <span class="o">=</span> <span class="mi">10</span>


<span class="c1">### Do NOT modify the code below this line.</span>

<span class="n">checkpointer</span> <span class="o">=</span> <span class="n">ModelCheckpoint</span><span class="p">(</span><span class="n">filepath</span><span class="o">=</span><span class="s1">&#39;saved_models/weights.best.from_scratch.hdf5&#39;</span><span class="p">,</span> 
                               <span class="n">verbose</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">save_best_only</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">train_tensors</span><span class="p">,</span> <span class="n">train_targets</span><span class="p">,</span> 
          <span class="n">validation_data</span><span class="o">=</span><span class="p">(</span><span class="n">valid_tensors</span><span class="p">,</span> <span class="n">valid_targets</span><span class="p">),</span>
          <span class="n">epochs</span><span class="o">=</span><span class="n">epochs</span><span class="p">,</span> <span class="n">batch_size</span><span class="o">=</span><span class="mi">20</span><span class="p">,</span> <span class="n">callbacks</span><span class="o">=</span><span class="p">[</span><span class="n">checkpointer</span><span class="p">],</span> <span class="n">verbose</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Train on 6680 samples, validate on 835 samples
Epoch 1/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.8854 - acc: 0.0084Epoch 00001: val_loss improved from inf to 4.87082, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 25s 4ms/step - loss: 4.8854 - acc: 0.0084 - val_loss: 4.8708 - val_acc: 0.0096
Epoch 2/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.8690 - acc: 0.0113Epoch 00002: val_loss improved from 4.87082 to 4.85077, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.8689 - acc: 0.0112 - val_loss: 4.8508 - val_acc: 0.0156
Epoch 3/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.8479 - acc: 0.0150Epoch 00003: val_loss improved from 4.85077 to 4.82285, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.8481 - acc: 0.0150 - val_loss: 4.8229 - val_acc: 0.0180
Epoch 4/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.8238 - acc: 0.0191Epoch 00004: val_loss improved from 4.82285 to 4.80168, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.8236 - acc: 0.0190 - val_loss: 4.8017 - val_acc: 0.0228
Epoch 5/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.7940 - acc: 0.0213Epoch 00005: val_loss improved from 4.80168 to 4.76351, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.7934 - acc: 0.0213 - val_loss: 4.7635 - val_acc: 0.0192
Epoch 6/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.7496 - acc: 0.0278Epoch 00006: val_loss improved from 4.76351 to 4.72846, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.7495 - acc: 0.0281 - val_loss: 4.7285 - val_acc: 0.0251
Epoch 7/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.7020 - acc: 0.0302Epoch 00007: val_loss did not improve
6680/6680 [==============================] - 24s 4ms/step - loss: 4.7024 - acc: 0.0301 - val_loss: 4.7528 - val_acc: 0.0251
Epoch 8/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.6578 - acc: 0.0314Epoch 00008: val_loss improved from 4.72846 to 4.68115, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.6576 - acc: 0.0316 - val_loss: 4.6811 - val_acc: 0.0287
Epoch 9/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.6057 - acc: 0.0390Epoch 00009: val_loss improved from 4.68115 to 4.67642, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.6063 - acc: 0.0389 - val_loss: 4.6764 - val_acc: 0.0371
Epoch 10/10
6660/6680 [============================&gt;.] - ETA: 0s - loss: 4.5580 - acc: 0.0446Epoch 00010: val_loss improved from 4.67642 to 4.56937, saving model to saved_models/weights.best.from_scratch.hdf5
6680/6680 [==============================] - 24s 4ms/step - loss: 4.5579 - acc: 0.0446 - val_loss: 4.5694 - val_acc: 0.0467
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt output_prompt">Out[44]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;keras.callbacks.History at 0x7f17f8542cf8&gt;</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Load-the-Model-with-the-Best-Validation-Loss">Load the Model with the Best Validation Loss<a class="anchor-link" href="#Load-the-Model-with-the-Best-Validation-Loss">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[45]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">model</span><span class="o">.</span><span class="n">load_weights</span><span class="p">(</span><span class="s1">&#39;saved_models/weights.best.from_scratch.hdf5&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Test-the-Model">Test the Model<a class="anchor-link" href="#Test-the-Model">&#182;</a></h3><p>Try out your model on the test dataset of dog images.  Ensure that your test accuracy is greater than 1%.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[46]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># get index of predicted dog breed for each image in test set</span>
<span class="n">dog_breed_predictions</span> <span class="o">=</span> <span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">expand_dims</span><span class="p">(</span><span class="n">tensor</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">0</span><span class="p">)))</span> <span class="k">for</span> <span class="n">tensor</span> <span class="ow">in</span> <span class="n">test_tensors</span><span class="p">]</span>

<span class="c1"># report test accuracy</span>
<span class="n">test_accuracy</span> <span class="o">=</span> <span class="mi">100</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="n">dog_breed_predictions</span><span class="p">)</span><span class="o">==</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">test_targets</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span><span class="o">/</span><span class="nb">len</span><span class="p">(</span><span class="n">dog_breed_predictions</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Test accuracy: </span><span class="si">%.4f%%</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">test_accuracy</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Test accuracy: 4.3062%
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
<hr>
<p><a id='step4'></a></p>
<h2 id="Step-4:-Use-a-CNN-to-Classify-Dog-Breeds">Step 4: Use a CNN to Classify Dog Breeds<a class="anchor-link" href="#Step-4:-Use-a-CNN-to-Classify-Dog-Breeds">&#182;</a></h2><p>To reduce training time without sacrificing accuracy, we show you how to train a CNN using transfer learning.  In the following step, you will get a chance to use transfer learning to train your own CNN.</p>
<h3 id="Obtain-Bottleneck-Features">Obtain Bottleneck Features<a class="anchor-link" href="#Obtain-Bottleneck-Features">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[47]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">bottleneck_features</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="s1">&#39;/data/bottleneck_features/DogVGG16Data.npz&#39;</span><span class="p">)</span>
<span class="n">train_VGG16</span> <span class="o">=</span> <span class="n">bottleneck_features</span><span class="p">[</span><span class="s1">&#39;train&#39;</span><span class="p">]</span>
<span class="n">valid_VGG16</span> <span class="o">=</span> <span class="n">bottleneck_features</span><span class="p">[</span><span class="s1">&#39;valid&#39;</span><span class="p">]</span>
<span class="n">test_VGG16</span> <span class="o">=</span> <span class="n">bottleneck_features</span><span class="p">[</span><span class="s1">&#39;test&#39;</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Model-Architecture">Model Architecture<a class="anchor-link" href="#Model-Architecture">&#182;</a></h3><p>The model uses the the pre-trained VGG-16 model as a fixed feature extractor, where the last convolutional output of VGG-16 is fed as input to our model.  We only add a global average pooling layer and a fully connected layer, where the latter contains one node for each dog category and is equipped with a softmax.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[48]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">VGG16_model</span> <span class="o">=</span> <span class="n">Sequential</span><span class="p">()</span>
<span class="n">VGG16_model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">GlobalAveragePooling2D</span><span class="p">(</span><span class="n">input_shape</span><span class="o">=</span><span class="n">train_VGG16</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">1</span><span class="p">:]))</span>
<span class="n">VGG16_model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Dense</span><span class="p">(</span><span class="mi">133</span><span class="p">,</span> <span class="n">activation</span><span class="o">=</span><span class="s1">&#39;softmax&#39;</span><span class="p">))</span>

<span class="n">VGG16_model</span><span class="o">.</span><span class="n">summary</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
global_average_pooling2d_7 ( (None, 512)               0         
_________________________________________________________________
dense_11 (Dense)             (None, 133)               68229     
=================================================================
Total params: 68,229
Trainable params: 68,229
Non-trainable params: 0
_________________________________________________________________
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
<h3 id="Compile-the-Model">Compile the Model<a class="anchor-link" href="#Compile-the-Model">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[49]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">VGG16_model</span><span class="o">.</span><span class="n">compile</span><span class="p">(</span><span class="n">loss</span><span class="o">=</span><span class="s1">&#39;categorical_crossentropy&#39;</span><span class="p">,</span> <span class="n">optimizer</span><span class="o">=</span><span class="s1">&#39;rmsprop&#39;</span><span class="p">,</span> <span class="n">metrics</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;accuracy&#39;</span><span class="p">])</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Train-the-Model">Train the Model<a class="anchor-link" href="#Train-the-Model">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[50]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">checkpointer</span> <span class="o">=</span> <span class="n">ModelCheckpoint</span><span class="p">(</span><span class="n">filepath</span><span class="o">=</span><span class="s1">&#39;saved_models/weights.best.VGG16.hdf5&#39;</span><span class="p">,</span> 
                               <span class="n">verbose</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">save_best_only</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="n">VGG16_model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">train_VGG16</span><span class="p">,</span> <span class="n">train_targets</span><span class="p">,</span> 
          <span class="n">validation_data</span><span class="o">=</span><span class="p">(</span><span class="n">valid_VGG16</span><span class="p">,</span> <span class="n">valid_targets</span><span class="p">),</span>
          <span class="n">epochs</span><span class="o">=</span><span class="mi">20</span><span class="p">,</span> <span class="n">batch_size</span><span class="o">=</span><span class="mi">20</span><span class="p">,</span> <span class="n">callbacks</span><span class="o">=</span><span class="p">[</span><span class="n">checkpointer</span><span class="p">],</span> <span class="n">verbose</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Train on 6680 samples, validate on 835 samples
Epoch 1/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 11.4752 - acc: 0.1406Epoch 00001: val_loss improved from inf to 9.28330, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 295us/step - loss: 11.3799 - acc: 0.1446 - val_loss: 9.2833 - val_acc: 0.2539
Epoch 2/20
6660/6680 [============================&gt;.] - ETA: 0s - loss: 8.3443 - acc: 0.3635Epoch 00002: val_loss improved from 9.28330 to 8.57971, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 240us/step - loss: 8.3378 - acc: 0.3639 - val_loss: 8.5797 - val_acc: 0.3533
Epoch 3/20
6440/6680 [===========================&gt;..] - ETA: 0s - loss: 7.7724 - acc: 0.4446Epoch 00003: val_loss improved from 8.57971 to 8.22671, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 241us/step - loss: 7.7729 - acc: 0.4452 - val_loss: 8.2267 - val_acc: 0.3952
Epoch 4/20
6480/6680 [============================&gt;.] - ETA: 0s - loss: 7.5551 - acc: 0.4787Epoch 00004: val_loss improved from 8.22671 to 8.02998, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 242us/step - loss: 7.5468 - acc: 0.4795 - val_loss: 8.0300 - val_acc: 0.4216
Epoch 5/20
6480/6680 [============================&gt;.] - ETA: 0s - loss: 7.4418 - acc: 0.5037Epoch 00005: val_loss improved from 8.02998 to 7.97091, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 240us/step - loss: 7.4192 - acc: 0.5042 - val_loss: 7.9709 - val_acc: 0.4156
Epoch 6/20
6440/6680 [===========================&gt;..] - ETA: 0s - loss: 7.2516 - acc: 0.5172Epoch 00006: val_loss improved from 7.97091 to 7.83021, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 242us/step - loss: 7.2435 - acc: 0.5175 - val_loss: 7.8302 - val_acc: 0.4455
Epoch 7/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 7.1595 - acc: 0.5320Epoch 00007: val_loss did not improve
6680/6680 [==============================] - 2s 240us/step - loss: 7.1548 - acc: 0.5331 - val_loss: 7.8552 - val_acc: 0.4395
Epoch 8/20
6440/6680 [===========================&gt;..] - ETA: 0s - loss: 7.0974 - acc: 0.5390Epoch 00008: val_loss improved from 7.83021 to 7.78890, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 241us/step - loss: 7.0819 - acc: 0.5397 - val_loss: 7.7889 - val_acc: 0.4467
Epoch 9/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 7.0103 - acc: 0.5497Epoch 00009: val_loss improved from 7.78890 to 7.69336, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 243us/step - loss: 6.9949 - acc: 0.5509 - val_loss: 7.6934 - val_acc: 0.4515
Epoch 10/20
6440/6680 [===========================&gt;..] - ETA: 0s - loss: 6.9237 - acc: 0.5570Epoch 00010: val_loss improved from 7.69336 to 7.63339, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 242us/step - loss: 6.9158 - acc: 0.5576 - val_loss: 7.6334 - val_acc: 0.4659
Epoch 11/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 6.8156 - acc: 0.5646Epoch 00011: val_loss improved from 7.63339 to 7.50683, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 243us/step - loss: 6.8034 - acc: 0.5647 - val_loss: 7.5068 - val_acc: 0.4539
Epoch 12/20
6600/6680 [============================&gt;.] - ETA: 0s - loss: 6.7127 - acc: 0.5715Epoch 00012: val_loss improved from 7.50683 to 7.48149, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 244us/step - loss: 6.7148 - acc: 0.5713 - val_loss: 7.4815 - val_acc: 0.4707
Epoch 13/20
6480/6680 [============================&gt;.] - ETA: 0s - loss: 6.6701 - acc: 0.5793Epoch 00013: val_loss improved from 7.48149 to 7.48051, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 242us/step - loss: 6.6762 - acc: 0.5789 - val_loss: 7.4805 - val_acc: 0.4635
Epoch 14/20
6660/6680 [============================&gt;.] - ETA: 0s - loss: 6.6675 - acc: 0.5788Epoch 00014: val_loss improved from 7.48051 to 7.42253, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 243us/step - loss: 6.6674 - acc: 0.5786 - val_loss: 7.4225 - val_acc: 0.4778
Epoch 15/20
6500/6680 [============================&gt;.] - ETA: 0s - loss: 6.6523 - acc: 0.5828Epoch 00015: val_loss improved from 7.42253 to 7.42079, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 241us/step - loss: 6.6539 - acc: 0.5826 - val_loss: 7.4208 - val_acc: 0.4778
Epoch 16/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 6.6541 - acc: 0.5839Epoch 00016: val_loss improved from 7.42079 to 7.40213, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 242us/step - loss: 6.6523 - acc: 0.5840 - val_loss: 7.4021 - val_acc: 0.4886
Epoch 17/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 6.6376 - acc: 0.5847Epoch 00017: val_loss did not improve
6680/6680 [==============================] - 2s 239us/step - loss: 6.6483 - acc: 0.5841 - val_loss: 7.4043 - val_acc: 0.4695
Epoch 18/20
6460/6680 [============================&gt;.] - ETA: 0s - loss: 6.6553 - acc: 0.5837Epoch 00018: val_loss did not improve
6680/6680 [==============================] - 2s 241us/step - loss: 6.6395 - acc: 0.5847 - val_loss: 7.4345 - val_acc: 0.4778
Epoch 19/20
6660/6680 [============================&gt;.] - ETA: 0s - loss: 6.5596 - acc: 0.5856Epoch 00019: val_loss improved from 7.40213 to 7.24217, saving model to saved_models/weights.best.VGG16.hdf5
6680/6680 [==============================] - 2s 242us/step - loss: 6.5641 - acc: 0.5853 - val_loss: 7.2422 - val_acc: 0.4910
Epoch 20/20
6500/6680 [============================&gt;.] - ETA: 0s - loss: 6.4719 - acc: 0.5949Epoch 00020: val_loss did not improve
6680/6680 [==============================] - 2s 241us/step - loss: 6.4904 - acc: 0.5939 - val_loss: 7.2696 - val_acc: 0.4826
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt output_prompt">Out[50]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;keras.callbacks.History at 0x7f17f80c6b70&gt;</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Load-the-Model-with-the-Best-Validation-Loss">Load the Model with the Best Validation Loss<a class="anchor-link" href="#Load-the-Model-with-the-Best-Validation-Loss">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[51]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">VGG16_model</span><span class="o">.</span><span class="n">load_weights</span><span class="p">(</span><span class="s1">&#39;saved_models/weights.best.VGG16.hdf5&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Test-the-Model">Test the Model<a class="anchor-link" href="#Test-the-Model">&#182;</a></h3><p>Now, we can use the CNN to test how well it identifies breed within our test dataset of dog images.  We print the test accuracy below.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[52]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># get index of predicted dog breed for each image in test set</span>
<span class="n">VGG16_predictions</span> <span class="o">=</span> <span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">VGG16_model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">expand_dims</span><span class="p">(</span><span class="n">feature</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">0</span><span class="p">)))</span> <span class="k">for</span> <span class="n">feature</span> <span class="ow">in</span> <span class="n">test_VGG16</span><span class="p">]</span>

<span class="c1"># report test accuracy</span>
<span class="n">test_accuracy</span> <span class="o">=</span> <span class="mi">100</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="n">VGG16_predictions</span><span class="p">)</span><span class="o">==</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">test_targets</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span><span class="o">/</span><span class="nb">len</span><span class="p">(</span><span class="n">VGG16_predictions</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Test accuracy: </span><span class="si">%.4f%%</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">test_accuracy</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Test accuracy: 48.8038%
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
<h3 id="Predict-Dog-Breed-with-the-Model">Predict Dog Breed with the Model<a class="anchor-link" href="#Predict-Dog-Breed-with-the-Model">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[53]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">extract_bottleneck_features</span> <span class="k">import</span> <span class="o">*</span>

<span class="k">def</span> <span class="nf">VGG16_predict_breed</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="c1"># extract bottleneck features</span>
    <span class="n">bottleneck_feature</span> <span class="o">=</span> <span class="n">extract_VGG16</span><span class="p">(</span><span class="n">path_to_tensor</span><span class="p">(</span><span class="n">img_path</span><span class="p">))</span>
    <span class="c1"># obtain predicted vector</span>
    <span class="n">predicted_vector</span> <span class="o">=</span> <span class="n">VGG16_model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">bottleneck_feature</span><span class="p">)</span>
    <span class="c1"># return dog breed that is predicted by the model</span>
    <span class="k">return</span> <span class="n">dog_names</span><span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">predicted_vector</span><span class="p">)]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<p><a id='step5'></a></p>
<h2 id="Step-5:-Create-a-CNN-to-Classify-Dog-Breeds-(using-Transfer-Learning)">Step 5: Create a CNN to Classify Dog Breeds (using Transfer Learning)<a class="anchor-link" href="#Step-5:-Create-a-CNN-to-Classify-Dog-Breeds-(using-Transfer-Learning)">&#182;</a></h2><p>You will now use transfer learning to create a CNN that can identify dog breed from images.  Your CNN must attain at least 60% accuracy on the test set.</p>
<p>In Step 4, we used transfer learning to create a CNN using VGG-16 bottleneck features.  In this section, you must use the bottleneck features from a different pre-trained model.  To make things easier for you, we have pre-computed the features for all of the networks that are currently available in Keras.  These are already in the workspace, at /data/bottleneck_features.  If you wish to download them on a different machine, they can be found at:</p>
<ul>
<li><a href="https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG19Data.npz">VGG-19</a> bottleneck features</li>
<li><a href="https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogResnet50Data.npz">ResNet-50</a> bottleneck features</li>
<li><a href="https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz">Inception</a> bottleneck features</li>
<li><a href="https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogXceptionData.npz">Xception</a> bottleneck features</li>
</ul>
<p>The files are encoded as such:</p>

<pre><code>Dog{network}Data.npz

</code></pre>
<p>where <code>{network}</code>, in the above filename, can be one of <code>VGG19</code>, <code>Resnet50</code>, <code>InceptionV3</code>, or <code>Xception</code>.</p>
<p>The above architectures are downloaded and stored for you in the <code>/data/bottleneck_features/</code> folder.</p>
<p>This means the following will be in the <code>/data/bottleneck_features/</code> folder:</p>
<p><code>DogVGG19Data.npz</code>
<code>DogResnet50Data.npz</code>
<code>DogInceptionV3Data.npz</code>
<code>DogXceptionData.npz</code></p>
<h3 id="(IMPLEMENTATION)-Obtain-Bottleneck-Features">(IMPLEMENTATION) Obtain Bottleneck Features<a class="anchor-link" href="#(IMPLEMENTATION)-Obtain-Bottleneck-Features">&#182;</a></h3><p>In the code block below, extract the bottleneck features corresponding to the train, test, and validation sets by running the following:</p>

<pre><code>bottleneck_features = np.load('/data/bottleneck_features/Dog{network}Data.npz')
train_{network} = bottleneck_features['train']
valid_{network} = bottleneck_features['valid']
test_{network} = bottleneck_features['test']</code></pre>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[54]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Obtain bottleneck features from another pre-trained CNN.</span>

<span class="n">bottleneck_features</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="s1">&#39;/data/bottleneck_features/DogResnet50Data.npz&#39;</span><span class="p">)</span>
<span class="n">train_Resnet50</span> <span class="o">=</span> <span class="n">bottleneck_features</span><span class="p">[</span><span class="s1">&#39;train&#39;</span><span class="p">]</span>
<span class="n">valid_Resnet50</span> <span class="o">=</span> <span class="n">bottleneck_features</span><span class="p">[</span><span class="s1">&#39;valid&#39;</span><span class="p">]</span>
<span class="n">test_Resnet50</span> <span class="o">=</span> <span class="n">bottleneck_features</span><span class="p">[</span><span class="s1">&#39;test&#39;</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Model-Architecture">(IMPLEMENTATION) Model Architecture<a class="anchor-link" href="#(IMPLEMENTATION)-Model-Architecture">&#182;</a></h3><p>Create a CNN to classify dog breed.  At the end of your code cell block, summarize the layers of your model by executing the line:</p>

<pre><code>    &lt;your model's name&gt;.summary()

</code></pre>
<p><strong>Question 5:</strong> Outline the steps you took to get to your final CNN architecture and your reasoning at each step.  Describe why you think the architecture is suitable for the current problem.</p>
<p><strong>Answer:</strong>  Complex deep networks are expensive to train , but this is already done for Resnet50 model and we just prepare the bottleneck features. Here we leverage a network pre-trained on a large datase. After loading the bottleneck feature , we just need to do the last pooling with output layer. The final dense layer is the classification task with 133 outputs.</p>
<p>This model is more successful than the original model , as a much complex structure is differentiated and recoganized. It caputers complex boundaries and the shapes of the objects are used, as network is pretrained on a large number of similar images to the given data.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[55]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Define your architecture.</span>
<span class="n">Resnet50_model</span> <span class="o">=</span> <span class="n">Sequential</span><span class="p">()</span>
<span class="n">Resnet50_model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">GlobalAveragePooling2D</span><span class="p">(</span><span class="n">input_shape</span><span class="o">=</span><span class="n">train_Resnet50</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">1</span><span class="p">:]))</span>
<span class="n">Resnet50_model</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Dense</span><span class="p">(</span><span class="mi">133</span><span class="p">,</span> <span class="n">activation</span><span class="o">=</span><span class="s1">&#39;softmax&#39;</span><span class="p">))</span>

<span class="n">Resnet50_model</span><span class="o">.</span><span class="n">summary</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
global_average_pooling2d_8 ( (None, 2048)              0         
_________________________________________________________________
dense_12 (Dense)             (None, 133)               272517    
=================================================================
Total params: 272,517
Trainable params: 272,517
Non-trainable params: 0
_________________________________________________________________
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
<h3 id="(IMPLEMENTATION)-Compile-the-Model">(IMPLEMENTATION) Compile the Model<a class="anchor-link" href="#(IMPLEMENTATION)-Compile-the-Model">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[57]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Compile the model.</span>
<span class="kn">from</span> <span class="nn">keras.optimizers</span> <span class="k">import</span> <span class="n">Adam</span><span class="p">,</span> <span class="n">Adamax</span>

<span class="n">Resnet50_model</span><span class="o">.</span><span class="n">compile</span><span class="p">(</span><span class="n">loss</span><span class="o">=</span><span class="s1">&#39;categorical_crossentropy&#39;</span><span class="p">,</span> <span class="n">optimizer</span><span class="o">=</span><span class="n">Adamax</span><span class="p">(</span><span class="n">lr</span><span class="o">=</span><span class="mf">0.002</span><span class="p">),</span> <span class="n">metrics</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;accuracy&#39;</span><span class="p">])</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Train-the-Model">(IMPLEMENTATION) Train the Model<a class="anchor-link" href="#(IMPLEMENTATION)-Train-the-Model">&#182;</a></h3><p>Train your model in the code cell below.  Use model checkpointing to save the model that attains the best validation loss.</p>
<p>You are welcome to <a href="https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html">augment the training data</a>, but this is not a requirement.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[60]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Train the model.</span>
<span class="kn">from</span> <span class="nn">keras.callbacks</span> <span class="k">import</span> <span class="n">ModelCheckpoint</span>  

<span class="n">checkpointer</span> <span class="o">=</span> <span class="n">ModelCheckpoint</span><span class="p">(</span><span class="n">filepath</span><span class="o">=</span><span class="s1">&#39;saved_models/weights.best_adamax.ResNet50.hdf5&#39;</span><span class="p">,</span> 
                               <span class="n">verbose</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">save_best_only</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="n">epochs</span> <span class="o">=</span> <span class="mi">20</span>
<span class="n">batch_size</span> <span class="o">=</span> <span class="mi">128</span>

<span class="n">Resnet50_model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">train_Resnet50</span><span class="p">,</span> <span class="n">train_targets</span><span class="p">,</span> <span class="n">validation_data</span><span class="o">=</span><span class="p">(</span><span class="n">valid_Resnet50</span><span class="p">,</span> <span class="n">valid_targets</span><span class="p">),</span>
          <span class="n">epochs</span><span class="o">=</span><span class="n">epochs</span><span class="p">,</span> <span class="n">batch_size</span><span class="o">=</span><span class="n">batch_size</span><span class="p">,</span> <span class="n">callbacks</span><span class="o">=</span><span class="p">[</span><span class="n">checkpointer</span><span class="p">],</span> <span class="n">verbose</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Train on 6680 samples, validate on 835 samples
Epoch 1/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 2.8269 - acc: 0.4062Epoch 00001: val_loss improved from inf to 1.43655, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 1s 119us/step - loss: 2.7438 - acc: 0.4210 - val_loss: 1.4365 - val_acc: 0.6563
Epoch 2/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.9095 - acc: 0.8144Epoch 00002: val_loss improved from 1.43655 to 0.98801, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 61us/step - loss: 0.8988 - acc: 0.8171 - val_loss: 0.9880 - val_acc: 0.7701
Epoch 3/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.5933 - acc: 0.8895Epoch 00003: val_loss improved from 0.98801 to 0.84153, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.5883 - acc: 0.8900 - val_loss: 0.8415 - val_acc: 0.7856
Epoch 4/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.4490 - acc: 0.9225Epoch 00004: val_loss improved from 0.84153 to 0.76774, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 59us/step - loss: 0.4449 - acc: 0.9232 - val_loss: 0.7677 - val_acc: 0.7940
Epoch 5/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.3580 - acc: 0.9437Epoch 00005: val_loss improved from 0.76774 to 0.71614, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.3548 - acc: 0.9451 - val_loss: 0.7161 - val_acc: 0.8072
Epoch 6/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.2923 - acc: 0.9624Epoch 00006: val_loss improved from 0.71614 to 0.69070, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 61us/step - loss: 0.2912 - acc: 0.9620 - val_loss: 0.6907 - val_acc: 0.8108
Epoch 7/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.2443 - acc: 0.9726Epoch 00007: val_loss improved from 0.69070 to 0.65960, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 59us/step - loss: 0.2452 - acc: 0.9726 - val_loss: 0.6596 - val_acc: 0.8132
Epoch 8/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.2075 - acc: 0.9823Epoch 00008: val_loss improved from 0.65960 to 0.64257, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 59us/step - loss: 0.2092 - acc: 0.9816 - val_loss: 0.6426 - val_acc: 0.8144
Epoch 9/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.1826 - acc: 0.9858Epoch 00009: val_loss improved from 0.64257 to 0.62075, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.1830 - acc: 0.9856 - val_loss: 0.6208 - val_acc: 0.8180
Epoch 10/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.1595 - acc: 0.9900Epoch 00010: val_loss improved from 0.62075 to 0.60817, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.1591 - acc: 0.9895 - val_loss: 0.6082 - val_acc: 0.8263
Epoch 11/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.1413 - acc: 0.9919Epoch 00011: val_loss improved from 0.60817 to 0.60343, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.1410 - acc: 0.9916 - val_loss: 0.6034 - val_acc: 0.8323
Epoch 12/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.1252 - acc: 0.9935Epoch 00012: val_loss improved from 0.60343 to 0.59721, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.1255 - acc: 0.9933 - val_loss: 0.5972 - val_acc: 0.8395
Epoch 13/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.1109 - acc: 0.9955Epoch 00013: val_loss improved from 0.59721 to 0.58203, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 59us/step - loss: 0.1112 - acc: 0.9957 - val_loss: 0.5820 - val_acc: 0.8335
Epoch 14/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.1016 - acc: 0.9960Epoch 00014: val_loss did not improve
6680/6680 [==============================] - 0s 58us/step - loss: 0.1012 - acc: 0.9960 - val_loss: 0.5846 - val_acc: 0.8359
Epoch 15/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.0912 - acc: 0.9974Epoch 00015: val_loss improved from 0.58203 to 0.57778, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 58us/step - loss: 0.0910 - acc: 0.9975 - val_loss: 0.5778 - val_acc: 0.8323
Epoch 16/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.0832 - acc: 0.9974Epoch 00016: val_loss improved from 0.57778 to 0.57212, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 58us/step - loss: 0.0830 - acc: 0.9976 - val_loss: 0.5721 - val_acc: 0.8347
Epoch 17/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.0754 - acc: 0.9984Epoch 00017: val_loss improved from 0.57212 to 0.56704, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 60us/step - loss: 0.0759 - acc: 0.9981 - val_loss: 0.5670 - val_acc: 0.8347
Epoch 18/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.0697 - acc: 0.9978Epoch 00018: val_loss improved from 0.56704 to 0.55999, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 59us/step - loss: 0.0694 - acc: 0.9979 - val_loss: 0.5600 - val_acc: 0.8323
Epoch 19/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.0637 - acc: 0.9978Epoch 00019: val_loss did not improve
6680/6680 [==============================] - 0s 58us/step - loss: 0.0638 - acc: 0.9978 - val_loss: 0.5638 - val_acc: 0.8335
Epoch 20/20
6272/6680 [===========================&gt;..] - ETA: 0s - loss: 0.0591 - acc: 0.9989Epoch 00020: val_loss improved from 0.55999 to 0.55648, saving model to saved_models/weights.best_adamax.ResNet50.hdf5
6680/6680 [==============================] - 0s 59us/step - loss: 0.0591 - acc: 0.9987 - val_loss: 0.5565 - val_acc: 0.8407
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt output_prompt">Out[60]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;keras.callbacks.History at 0x7f17d09a30f0&gt;</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Load-the-Model-with-the-Best-Validation-Loss">(IMPLEMENTATION) Load the Model with the Best Validation Loss<a class="anchor-link" href="#(IMPLEMENTATION)-Load-the-Model-with-the-Best-Validation-Loss">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[61]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Load the model weights with the best validation loss.</span>

<span class="n">Resnet50_model</span><span class="o">.</span><span class="n">load_weights</span><span class="p">(</span><span class="s1">&#39;saved_models/weights.best_adamax.ResNet50.hdf5&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="(IMPLEMENTATION)-Test-the-Model">(IMPLEMENTATION) Test the Model<a class="anchor-link" href="#(IMPLEMENTATION)-Test-the-Model">&#182;</a></h3><p>Try out your model on the test dataset of dog images. Ensure that your test accuracy is greater than 60%.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[62]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Calculate classification accuracy on the test dataset.</span>
<span class="n">Resnet50_predictions</span> <span class="o">=</span> <span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">Resnet50_model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">expand_dims</span><span class="p">(</span><span class="n">feature</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">0</span><span class="p">)))</span> <span class="k">for</span> <span class="n">feature</span> <span class="ow">in</span> <span class="n">test_Resnet50</span><span class="p">]</span>

<span class="c1"># report test accuracy</span>
<span class="n">test_accuracy</span> <span class="o">=</span> <span class="mi">100</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="n">Resnet50_predictions</span><span class="p">)</span><span class="o">==</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">test_targets</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span><span class="o">/</span><span class="nb">len</span><span class="p">(</span><span class="n">Resnet50_predictions</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Test accuracy: </span><span class="si">%.4f%%</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">test_accuracy</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Test accuracy: 83.3732%
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
<h3 id="(IMPLEMENTATION)-Predict-Dog-Breed-with-the-Model">(IMPLEMENTATION) Predict Dog Breed with the Model<a class="anchor-link" href="#(IMPLEMENTATION)-Predict-Dog-Breed-with-the-Model">&#182;</a></h3><p>Write a function that takes an image path as input and returns the dog breed (<code>Affenpinscher</code>, <code>Afghan_hound</code>, etc) that is predicted by your model.</p>
<p>Similar to the analogous function in Step 5, your function should have three steps:</p>
<ol>
<li>Extract the bottleneck features corresponding to the chosen CNN model.</li>
<li>Supply the bottleneck features as input to the model to return the predicted vector.  Note that the argmax of this prediction vector gives the index of the predicted dog breed.</li>
<li>Use the <code>dog_names</code> array defined in Step 0 of this notebook to return the corresponding breed.</li>
</ol>
<p>The functions to extract the bottleneck features can be found in <code>extract_bottleneck_features.py</code>, and they have been imported in an earlier code cell.  To obtain the bottleneck features corresponding to your chosen CNN architecture, you need to use the function</p>

<pre><code>extract_{network}

</code></pre>
<p>where <code>{network}</code>, in the above filename, should be one of <code>VGG19</code>, <code>Resnet50</code>, <code>InceptionV3</code>, or <code>Xception</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[70]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Write a function that takes a path to an image as input</span>
<span class="c1">### and returns the dog breed that is predicted by the model.</span>

<span class="kn">from</span> <span class="nn">extract_bottleneck_features</span> <span class="k">import</span> <span class="o">*</span>

<span class="k">def</span> <span class="nf">Resnet50_predict_breed</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="c1"># extract bottleneck features</span>
    <span class="n">bottleneck_feature</span> <span class="o">=</span> <span class="n">extract_Resnet50</span><span class="p">(</span><span class="n">path_to_tensor</span><span class="p">(</span><span class="n">img_path</span><span class="p">))</span>
    <span class="c1"># obtain predicted vector</span>
    <span class="n">predicted_vector</span> <span class="o">=</span> <span class="n">Resnet50_model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">bottleneck_feature</span><span class="p">)</span>
    <span class="c1"># return dog breed that is predicted by the model</span>
    <span class="n">breed</span> <span class="o">=</span> <span class="n">dog_names</span><span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">predicted_vector</span><span class="p">)]</span>
    <span class="n">img</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span>
    <span class="n">cv_rgb</span> <span class="o">=</span> <span class="n">cv2</span><span class="o">.</span><span class="n">cvtColor</span><span class="p">(</span><span class="n">img</span><span class="p">,</span> <span class="n">cv2</span><span class="o">.</span><span class="n">COLOR_BGR2RGB</span><span class="p">)</span>
    <span class="n">imgplot</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">imshow</span><span class="p">(</span><span class="n">cv_rgb</span><span class="p">)</span>
    <span class="k">if</span> <span class="n">dog_detector</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
        <span class="k">return</span> <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The breed of dog is a </span><span class="si">{}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">breed</span><span class="p">))</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="k">return</span> <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Human resembles, the breed  </span><span class="si">{}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">breed</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<p><a id='step6'></a></p>
<h2 id="Step-6:-Write-your-Algorithm">Step 6: Write your Algorithm<a class="anchor-link" href="#Step-6:-Write-your-Algorithm">&#182;</a></h2><p>Write an algorithm that accepts a file path to an image and first determines whether the image contains a human, dog, or neither.  Then,</p>
<ul>
<li>if a <strong>dog</strong> is detected in the image, return the predicted breed.</li>
<li>if a <strong>human</strong> is detected in the image, return the resembling dog breed.</li>
<li>if <strong>neither</strong> is detected in the image, provide output that indicates an error.</li>
</ul>
<p>You are welcome to write your own functions for detecting humans and dogs in images, but feel free to use the <code>face_detector</code> and <code>dog_detector</code> functions developed above.  You are <strong>required</strong> to use your CNN from Step 5 to predict dog breed.</p>
<p>Some sample output for our algorithm is provided below, but feel free to design your own user experience!</p>
<p><img src="images/sample_human_output.png" alt="Sample Human Output"></p>
<h3 id="(IMPLEMENTATION)-Write-your-Algorithm">(IMPLEMENTATION) Write your Algorithm<a class="anchor-link" href="#(IMPLEMENTATION)-Write-your-Algorithm">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[66]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">### TODO: Write your algorithm.</span>
<span class="c1">### Feel free to use as many code cells as needed.</span>

<span class="k">def</span> <span class="nf">predict_breed</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">dog_detector</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span> <span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Detected a dog&quot;</span><span class="p">)</span>
        <span class="n">breed</span> <span class="o">=</span> <span class="n">Resnet50_predict_breed</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span>
        <span class="k">return</span> <span class="n">breed</span>
    
    <span class="k">elif</span> <span class="n">face_detector</span><span class="p">(</span><span class="n">img_path</span><span class="p">):</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Detected a human face&quot;</span><span class="p">)</span>
        <span class="n">breed</span> <span class="o">=</span> <span class="n">Resnet50_predict_breed</span><span class="p">(</span><span class="n">img_path</span><span class="p">)</span>
        <span class="k">return</span> <span class="n">breed</span>
   
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No human face or dog detected&quot;</span><span class="p">)</span>
        <span class="k">return</span> <span class="o">-</span><span class="mi">1</span>
        
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<p><a id='step7'></a></p>
<h2 id="Step-7:-Test-Your-Algorithm">Step 7: Test Your Algorithm<a class="anchor-link" href="#Step-7:-Test-Your-Algorithm">&#182;</a></h2><p>In this section, you will take your new algorithm for a spin!  What kind of dog does the algorithm think that <strong>you</strong> look like?  If you have a dog, does it predict your dog's breed accurately?  If you have a cat, does it mistakenly think that your cat is a dog?</p>
<h3 id="(IMPLEMENTATION)-Test-Your-Algorithm-on-Sample-Images!">(IMPLEMENTATION) Test Your Algorithm on Sample Images!<a class="anchor-link" href="#(IMPLEMENTATION)-Test-Your-Algorithm-on-Sample-Images!">&#182;</a></h3><p>Test your algorithm at least six images on your computer.  Feel free to use any images you like.  Use at least two human and two dog images.</p>
<p><strong>Question 6:</strong> Is the output better than you expected :) ?  Or worse :( ?  Provide at least three possible points of improvement for your algorithm.</p>
<p><strong>Answer:</strong>  The output is better than I expected. It definitely detects correctly if the image belongs to dog or human. The accuracy rate is 83.37 %. It will be interesting to explore more to get a better idea.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[81]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">## TODO: Execute your algorithm from Step 6 on</span>
<span class="c1">## at least 6 images on your computer.</span>
<span class="c1">## Feel free to use as many code cells as needed.</span>

<span class="n">predict_breed</span><span class="p">(</span><span class="s1">&#39;images/image4.jpg&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Detected a dog
The breed of dog is a in/050.Chinese_shar-pei
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
