# pocketsphinx.js.external
pocketsphinx.js.external

This is a test of the https://github.com/syl22-00/pocketsphinx.js/ repository.  Specifically the part in the documentation where you try to use the lazyLoad feature to load the acoustic model from external files.  It is an attempt to recreate the pocketsphinx.js demo located at /webapp/live.html using the external model files.  The file /webapp/js/pocketsphinx.js was created using this command:

`cmake -DEMSCRIPTEN=1 -DCMAKE_TOOLCHAIN_FILE=c:\software\emcc\emscripten\1.35.0\cmake\Modules\Platform\Emscripten.cmake -G "MinGW Makefiles" -DHMM_EMBED=OFF ..`

pocketsphinx-default.js is the original from the original repository included for testing.

You can test it here.
https://rawgit.com/Thread7/pocketsphinx.js.external/master/webapp/lazy.html

The example should work for you if you are using Chrome on Windows or Android.  If you want to customize for yourself beware that most acoustic models do not work with the lazyLoad command.  This one cmusphinx-en-us-ptm-5.2 is the only one so far that I have found to work.  You will get various errors other models.  If anyone can post other models that work, please do so.



