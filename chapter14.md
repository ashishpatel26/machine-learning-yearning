## 14. 错误分析：查看开发集的例子来评估想法

![](pics/14.1.jpg)

当你使用你的猫应用程序，你会注意到把狗误认为是猫的例子。一些狗很像猫！

一个团队成员建议加入可以使系统在狗图像上做的更好的第三方软件。这将需要一个月的时间，团队成员非常热情。应该让他们继续吗？

在投入一个月时间来完成这项任务之前，我建议你首先评估一下它能够真正提高多少系统的准确率。然后你可以更合理的决定是否值得开发一个月，或者你最好在其他任务上使用这段时间。

详细的说，这是你可以做的事情：

1. 收集100个系统错误分类的开发集样本，即，你的系统发生错误的样本。

2. 手动查看这些样本，并计算它们中狗的图像占的比例。

查看错误样本的过程称为**错误分析**。在这个例子中，如果你发现只有5%的错误分类图像是狗，那么无论你如何改进狗的图像识别算法，你都不会消除5%以上的狗。换句话说，5%是做这个提议的项目可以提供多少帮助的“上限”（意思是最大可能数额）。因此，如果你的系统目前有90%的准确率（10%的误差），那么这种改进最好的结果是90.5%的准确率（或9.5%的误差，比原来的10%的误差小5%）。

相反，如果你发现50%的错误都是狗，那么你可以更加确信这个提议会产生很大的影响。它可以把准确率从90%最高提高到95%（误差相对减少50%，从10%降低到5%）。

这种简单的错误分析方法给你提供了一种快速估算合并第三方狗图片软件的可能价值的方法。它为决定是否进行这项头巾提供了量化基础。

错误分析通常可以帮助你弄清不同方向有多少价值。我看到许多工程师不愿意进行错误分析。通常情况下，进入实施一些想法更令人兴奋，而不是质疑这个想法是否值得投入时间。这是一个常见的错误：它可能会导致你的团队花费一个月的时间只得到意识到它没什么好处的结果。

手动检查100个样例并不需要很长时间。即使你每张图片花费一分钟，你也可以在两个小时内完成。这两个小时可以为你节约一个月的时间。

**错误分析**是指检查开发集中算法错误分类样本的过程，以便能够了解错误的根本原因。这可以帮助你确定项目的优先顺序（如本例所示），并极力我们接下来讨论的新方向。接下来的几章将会介绍执行错误分析的最佳实践。


