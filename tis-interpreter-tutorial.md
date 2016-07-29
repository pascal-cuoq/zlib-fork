STEP 1

Typing `./configure` modifies the files `Makefile` and `zconf.h`, and generates a couple of other files that weren't present. tis-interpreter, as a compilation platform, is identical neither  to the host platform on which I typed `./configure` nor to the minimal compilation platform that the initial zconf.h targeted without assumptions. But tis-interpreter is closer to the latter, and also I may want to compile zlib with an ordinary compiler later, so I will go with the flow and start from the `zconf.h` that was generated when I typed `./configure`. We will not use the generated `Makefile` for tis-interpreter, instead passing the C source files on the command-line.

