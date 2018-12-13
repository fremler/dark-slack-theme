# dark-slack-theme

Go to C:\Users\USER\AppData\Local\slack\app-3.3.3\resources\app.asar.unpacked\src\static

Open ssb-interop.js

Add to bottom of file
document.addEventListener('DOMContentLoaded', function() {
 $.ajax({
   url: 'https://raw.githubusercontent.com/fremler/dark-slack-theme/master/black.css',
   success: function(css) {
     $("<style></style>").appendTo('head').html(css);
   }
 });
});

Save file

Reload slack
