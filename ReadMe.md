## 在 Ubuntu 上实现文字的 typing 效果可以使用一个叫做 pv 的命令行工具。pv 命令可以将输入流（例如一个文本文件）的内容逐字符地显示出来，从而实现 typing 效果。 \

-以下是在 Ubuntu 上使用 pv 命令实现 typing 效果的步骤： \
-安装 pv 命令：在终端中运行以下命令进行安装： \

$   sudo apt-get update  \
$   sudo apt-get install pv  \
-创建一个文本文件，将要显示的文字写入其中。 \
-在终端中运行以下命令，将文本文件的内容传递给 pv 命令，并使用 -q 参数使 pv 命令的输出不显示进度条： \

$   cat 文本文件 | pv -qL 10   \
在上面的命令中，-q 参数表示“quiet”（不显示进度条），-L 10 参数表示每秒输出 10 个字符。你可以根据需要自行调整这些参数。 \
运行上述命令后，你应该会看到你所写的文字被逐字符地打印出来，就像是在进行 typing 一样。 \
注意：使用 pv 命令需要先创建一个文本文件，将要显示的文字写入其中。如果你想要在命令行中直接输入文字并实现 typing 效果，可以尝试使用 xdotool 工具，它可以模拟键盘输入并实现 typing 效果。 \

<video width="640" height="360" controls>
   <source src="key_tech_AI.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
  
![](key_tech_AI.mp4)
