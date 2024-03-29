# 引言
----------
&emsp;&emsp;推荐系统是一种针对特殊用户提供建议选择项的软件工具与技术。这种“建议”与许多不同的决策程序相关，比如，推荐买什么、推荐听什么歌、或者推荐阅读什么新闻。


&emsp;&emsp;“选项”是一个常用术语，通常用于表示系统推荐什么给用户。一个推荐系统一般关注于明确类型的选项（比如，CD或者新闻），以及它相应的设计、用户图形界面和常用于产生推荐项的核心推荐技术（针对项目明确的类型全自定义化地提供有用且高效的建议）。

&emsp;&emsp;推荐系统主要针对那些缺乏个人经验或者能力的个人，以评估网站中潜在大量的可替代项目，比如，有许多工作岗位。一个基本的例子就是书本推荐系统，其帮助用户选择他们想要阅读的书籍。在著名的亚马逊网，其采用了一个推荐系统为每一个客户提供个性化服务。由于推荐通常是个性化的，不同的用户或用户组可以从不同的、定制的建议中获益。另外，同样也有非个性化的推荐，杂志或报纸上的非个性化推荐产生比较简单且有特征性。典型的例子有：购买排名前十的书籍、CD等等。虽然它们在某些情况下是有用且有效的，但是这些非个性化推荐显然不是推荐系统研究的领域。

&emsp;&emsp;在最简单的形式中，个性化的推荐是作为项目的排序列表提供的。在执行这个排名时，推荐系统会试图根据用户的偏好和约束来预测什么是最适合的产品或服务。为了完成计算任务，推荐系统会从用户收集关于他们自身的偏好信息，这些信息要么是明确表示的，例如，作为产品的评级，要么是通过解释用户的行为来推断的。例如，推荐系统可以将用户搜索的特定产品页面上的选项作为用户的隐式偏好标志。


&emsp;&emsp;推荐系统的发展源于一个相当简单的观察：个体在日常的抉择中通常会依赖与他人提供的建议。例如，在选择阅读书籍时，通常依赖于同行推荐的内容；雇主在招聘决定中依赖于推荐信；而在选择观看电影时，个人倾向于阅读并依赖电影评论家撰写的电影评论，这些评论包括出现在他们读的报纸上。

&emsp;&emsp;为了模仿这种行为，第一个推荐系统应用了算法，以利用用户社区产生的建议，并将这些建议传递给“活动”用户或正在寻找建议的用户。这些建议是针对那些相似的用户，或者有相似品味的用户喜欢的产品。这种方法被称为**协作过滤**，其**基本原理**是：如果活动用户在过去与某些用户达成一致，那么来自这些相似用户的其他建议应该与活动用户相关，并且与活动用户感兴趣。

&emsp;&emsp;随着电子商务网站的发展，迫切需要通过过滤所有可用的解决方案来提供针对性建议。因为用户发现很难从这些网站提供的种类繁多的商品（产品和服务）中做出最合适的选择。

&emsp;&emsp;网络上信息的爆炸性增长和多样性，以及新的电子商务服务（销售产品、产品比较、拍卖等）的迅速推出，经常让用户不知所措，导致他们做出错误的决定。选择的可获得性并没有带来好处，反而开始降低用户的幸福感。据了解，虽然选择是好的，但更多的选择并不总是好的。事实上，选择及其自由、自治和自我决定的含义可能变得过分，并最终导致自由统治可能被视为一种导致痛苦的暴政。

&emsp;&emsp;近年来，推荐系统已经被证明是解决信息过载问题的有效手段。最终，推荐系统通过将用户指向可能与用户当前任务相关的新的、尚未体验的项目来解决这一现象。根据用户的请求（可以根据用户的上下文和需要根据推荐方法来表达），推荐系统使用关于用户、可用项和存储在自定义数据库中的以前事务的各种类型的知识和数据来生成推荐。接着，用户可以浏览这些建议。一个人可以接受或不接受它们，并可以立即或在稍后阶段提供内隐或外显的反馈。此用户操作和反馈可存储在推荐者数据库中，并可用于在即将到来的用户系统交互中生成新的推荐。

&emsp;&emsp;如前所述，与其他经典信息系统工具和技术（如数据库或搜索引擎）相比，国际上对推荐系统的研究相对较新。推荐系统作为一个独立的研究领域出现于20世纪90年代中期，近年来，人们对推荐系统的兴趣急剧增加，事实表明：

 1. 推荐系统在诸如amazon.com、youtube、netflix、spotify、linkedin、facebook、tripadvisor、last.fm和imdb等高评价的互联网网站中发挥着重要作用。此外，许多媒体公司现在正在开发和部署推荐系统作为它们向用户提供的服务的一部分。例如，在线点播流媒体提供商netflix为这个首次成功地大幅度提高推荐系统性能的团队颁发了百万美元的奖金。
 2. 有专门针对这一领域的会议和讲习班，即2007年成立的计算机协会（ACM）推荐系统系列会议。本次会议是推荐技术研究与应用领域的年度盛会。此外，在数据库、信息系统和自适应系统领域的较传统的会议中，常常包括专门讨论推荐系统的会议。在这一范围内的其他值得注意的会议包括：ACM的信息检索特别兴趣组（SIGIR）；用户建模、自适应和个性化（UMAP）；智能用户界面（IUI）；万维网（WWW）；以及ACM的数据管理特别兴趣组（SIGM）OD）。
 3. 在世界各地的高等教育机构中，本科生和研究生课程现在都完全致力于推荐系统，推荐系统的教程在计算机科学会议上非常流行，还出版了一本介绍rss技术的书。Springer出版了几本关于推荐系统中特定主题的书：电气和计算机工程中的斯普林格简介。最近还出版了大量新的文章，专门介绍推荐系统在软件工程中的应用。
 4. 学术期刊中有一些专刊涉及rss领域的研究和发展。专门出版rss的期刊有：ai communications（2008）；ieee intelligent systems（2007）；international journal of electronic commerce（2006）；international journal of computer science and applications（2006）；acm transactions on computer human interaction（2005）；acm tra信息系统NSActions（2004）；用户建模和用户适应性交互（2014、2012）；交互式智能系统ACM交易（2013）；智能系统和技术ACM交易（2015）。

&emsp;&emsp;在本介绍性章节中，我们将简要讨论推荐系统的基本思想和概念。我们的主要目标不是提供一个关于推荐系统的完整的调查，而是以一种连贯和结构化的方式描述本手册中包含的章节，并帮助读者浏览本手册提供的丰富和详细的内容。读者也可以参考最近关于推荐系统的介绍或调查。在本章的最后，我们确定了一些我们认为对该领域未来特别重要的研究挑战。

&emsp;&emsp;该手册分为五个部分：推荐技术；推荐系统评估；推荐系统应用；推荐系统与人机交互；高级算法。

&emsp;&emsp;第一部分介绍了目前构建推荐系统最常用的技术，如协作过滤、基于内容的数据挖掘方法和上下文感知方法。

&emsp;&emsp;第二部分调查了用于评价建议质量的技术和方法。本章还考虑了可能影响推荐系统设计的方面（域、设备、接口、用户等）。最后，讨论了用用户实验评价所开发系统的方法、挑战和措施。

&emsp;&emsp;第三部分包括一些与如何提出、浏览、解释和可视化建议有关的问题。其中，本部分重点介绍了用户隐私和推荐系统支持的决策过程。

&emsp;&emsp;第四部分是推荐系统的应用。我们在这里提供这些技术在音乐、移动计算、约会、社交网络、教育和电影中的广泛应用。

&emsp;&emsp;最后一部分介绍了各种高级主题的论文，例如：利用主动学习原则来指导新知识的获取；建议的新颖性和多样性；保护推荐系统免受恶意用户攻击的适当技术；以及推荐系统聚合了多种类型的用户反馈和偏好以构建更可靠的推荐。