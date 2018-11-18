# 用于管理开源项目的工具集

采用开源的战略之路，开始于小心翼翼的规划、精心的组织、以及成立开源项目办公室，从而希望能够指导和管理开源项目的创建、分发以及使用。但是要知道，这仅仅是万里长征的第一步。欲使开源项目办公室按照预定的顺利运行，我们还需要有效的利用一些工具。这些工具在整个开源当中都起着重要的作用，它们被用来跟踪各个部门的目标、各项指标，包括工程、法律、以及行政管理、公关、市场营销等等部门，同时给予员工所有它们需要收集的资源，并提供业绩表现的记录，以及管理公司内部日常使用的开源。

本指南提供了如何管理开源项目工具的详细介绍和场景使用，其中包括用于跟踪和管理开源项目这样最为重要工具的信息。本指南中的所提及的大多数工具来自于Linux基金会所创建，且是开源的，当然也收录了其它相关的优秀的厂商或社区的工具，它们多数是免费而容易获得的。另外，还有一些工具提供了整合式的工具，通过一个集中的仪表操作多项工具。

**Table of Contents**

- [开源项目管理为何需要特别的工具](#why-you-need-special-tools-for-open-source-program-management)
- [如何选择和规划工具](#how-to-select-and-plan-your-tools)
- [工具集的基本元素](#elements-of-a-basic-toolset)
- [用于管理源代码的工具](#tools-for-managing-source-code)
- [用于跟踪项目健康度的工具](#tools-for-tracking-project-health)
- [沟通和协作的工具](#tools-for-communications-and-collaboration)
- [公司级扩展的用户GitHub管理工具](#tools-for-corporate-scale-github-management)
- [写在最后](#final-words)

## Why you need special tools for open source program management

当开源项目办公室开始启动并运行时，那么也就是开始收集好用的软件工具，从而让开发团队来管理、跟踪、指引、和改进他们的开源项目、贡献以及发布。

这些工具之所以重要，是因为使用开源来为业务战略所需要，它有自身的方法论和流程，而这是区别于使用商业软件的特别的地方。开源的工具可以让公司完成许多令人惊奇的任务：

* 为协作和代码构建提供工作台
* 管理项目的健康度
* 自动化关键且重复的任务，如代码审核、跟踪和许可证合规检查
* 生成一些数据，以说明开源项目办公室和开源战略的ROI是合理的
* 监控项目的质量，若有突发状况，能及时的响应应对

在你开启自己的开源之路时，拥有正确的工具将会为贵司的开发者和其它员工带来益处，成功的几率也更高，当然它也是整体公司开源项目成功协作和沟通的基石。

> “如果贵司已经拥有超过100个代码仓库，或者是已经有超过100位开源开发者需要管理，那么你再也不能采用电子表格来将就。但是，现实的情况是，依然有很多人就是这么将就的【捂脸】，不过，这样做的弊端是很让人抓狂的，而且往往卖力不讨好。那么这个时候就体现出工具的优势了，因为它可以让你如虎添翼！” – [Jeff McAffer](https://twitter.com/jeffmcaffer), 微软开源项目办公室总监

> “总而言之，你需要工具来自动化你的一切，否则就得浪费大量时间手动完成工作。”  - [Chris Aniszczyk](https://twitter.com/cra) –云原生计算基金会首席运营官、前Twitter开源项目负责人

## How to select and plan your tools

关于那些开源工具是需要的，在早期的讨论阶段，往往取决于公司所依赖的业务、产品、服务以及是如何服务于自己的用户和雇主。正如开源项目办公室所开发的规划流程和战略蓝图，工具的选择是可以和企业的目标、流程、基础设施集成在一起的。

归根到底，想知道将需要使用哪些工具，唯一的方法就是，去了解想要对开源代码进行何种操作。

以下列出的是管理开源项目办公室所需工具选择的基本步骤：

1. 获得开发者和社区成员的口味和选择偏好。为了实现这点，需要与开发者和社区成员进行深度的讨论，开发者和社区成员们会描述什么样的工具是他们所喜爱和适合的。要认真的对待他们的建议和需求，并学会倾听这些能够让你实现目标的人们的声音。他们一般都有使用顺手的工具和习惯，所以直接从中吸取经验是最有益的。
2. 根据关键业务的应用，去了解依赖和集成的相关软件。这也就意味着，要去了解并通晓贵司业务所依赖的开源软件，以让贵司的开发者可以紧跟项目，在安全和软件的更新跟进方面保持优势。
3. 去了解现成的工具，然后去决定哪些工具可以直接使用，或者根据需要进行构建。不要从头开发每一个工具。去了解贵司所参与的开源社区已经在使用的工具，并就这些工具获得进一步的建议和反馈，到线上的开发社区中寻求那些工具好用，并请求他们的建议和推荐。到一些开源的研讨会上询问人们，在相关的会议上和开发人员进行沟通，要向那些已经淌过河的前辈的学习。

这些工具一旦被选定，在落地使用之前，还需要一些额外的准备：

1. 创建内部的基础设施用来支撑、管理和使用这些工具。在贵司新建立的开源项目办公室中，指定一名工程师来维护和构建这些基础设施，然后创建内部的在线门户，用来组织任务并分发这些工具。在此分发工具的门户中，关于权限和认证部分可以根据实际情况而定，可以选择开放给所有的开发人员，也可以根据特定的人员职责来划分。
2. 为使用这些工具的员工提供相应的培训计划。仅仅让他们拿到工具是远远不够的，要确保开发者知道如何使用这些工具并且具备掌控的能力。至于培训的形式，可以灵活的进行选择，可以是在线培训、也可以是专门的教室，甚至是小型的午餐小组都是可以的，重要的是让使用工具的这些人们懂得如何使用。询问开发者们那种学习方式更加适合他们，并让他们自己做出选择。
3. 确保这些工具在贵司中是集中呈现的。要使得开发者们能够轻松的找到并使用它们，最好的办法是整合到公司原来的开发者门户当中，另外，这也有助于日后运营当中组织和分发重要的工具。

请牢记上述的建议，它会帮助你选择工具，也会影响到你的决定。（有些工具是可能有学习曲线的，记得要提供相应的培训。）

### 利用现成的工具

在你想好了团队需要那些方能满足贵司的开源目标之后，也了解了自身所依赖和基础设施的局限，那么接下来要做的事情就是探索和学习现有的工具，那些已经生产就绪而且随时可用的工具。由于大多数开源工具是根据自身需求所开发的，所以这些工具未必拿来之后就立即满足了贵司所有的需求，如果不满足的话，也没有关系，贵司有的是开发者，看需要那些功能直接和他们沟通、贡献就好了。

颇具意味深长的是，很多公司的开源项目办公室并不经常利用其它公司所开发的工具，甚至也不会去和其它公司协作来开发工具，尽管这些公司很不情愿的去重复制造轮子，但包括 Facebook 和微软在内的许多企业已经拥有现有的工具套件，这些工具套件在真正成为一个协作议题之前就已经实现。由于他们已经拥有了自己的工具集并进行了投资，他们似乎并没有很大意愿采用其他公司的工具。

话说回来，对于贵司来说，这不就是开源所带来的最大优势吗？直接使用他们已经开发好的工具，有不满足的地方，开发即可。而不用像早期的那些建立开源项目办公室的公司，因为没有可用的工具而需要进行大量的开发。

对于刚刚建立开源项目办公室的公司来说，明智地去利用他人成功的经验和失败的教训不是更好吗。他们可以利用近年来由这些伟大的先行者公司所开发的成熟的工具来打造属于自己的开源管理工具箱。Linux基金会的开源行业组织，TODO Group，从成立伊始就一直致力于搞一个“开源项目办公室工具箱”的入门套件，其可以为新进入开源的公司能够通过一套紧密结合的预先组装工具来开展开源相关工作。目前来说该工具箱还有大量的工作要做，但是希望随着时间的增长，Linux基金会可以提供这样一个愿景：“让新加入开源的公司可以通过这样一套百宝箱，可以轻松部署和配置它们所需要的工具”。目前参与这个工具箱开发的公司有：Adobe、Capital One、Comcast、Facebook、谷歌、eBay、IBM、微软、三星以及Twitter。

### 创建一个仪表盘

除了配备完适当的工具之外，贵司还应有一个集中的仪表盘来展示实时的监控和跟踪有关开源项目的进展情况。绝大多数公司在这之前就有相应的应用，那么能够将开源的这些工具集成起来也是最好不过了。没有的话也没有关系，创建或采用一个新的！

> “对于整体的仪表盘来说，实现它的方式实在是太多了，而对于公司如何展现开发者相关信息这是真正的艺术。有些同仁们会打造出非常酷炫的显示效果，其实没什么必要，重要的是中心位置上能展现关键的内容，最好是和现有的仪表程序能够和谐共存，这个唯一存在的价值就是让人们能够一目了然的了解开源项目的健康度、各项指标等。” – [Chris Aniszczyk](https://twitter.com/cra), 云原生计算基金会首席运营官

## Elements of a basic toolset

有关管理开源项目和项目的报表的工具越来越多了起来，而且这个趋势非常的明显。如果贵司是开源的刚刚入行者，那么一些基本的工具对于聚焦初步的研究是很有益处的。

伴随着项目的增长，你会获得使用这些工具更多的经验，你或许会开始采用一些新的工具来帮助你自动化或流化增长需要的流程。不过要切记，新选择的工具将用于内部文化和流程的补充和支持 —— 而不是相反。

接下来的几节内容涵盖了几乎所以开源项目日常使用的工具类别。如此的分类对于你组织研究自己的项目也是非常有益处的。

### 自动化流程

对于贵司的开源项目来说，你所选择和使用的自动化流程工具是非常重要的。不过有关自动化的流程的工具非常的广泛，甚至还包括可以自动执行贡献者许可协议（CLAs）的程序，贡献者许可协议（CLAs）是一份按法律声明，声明开发人员创建了代码且不是从其他任何地方非法复制。在过去，这些协议通过打印出一份、签名然后传真回来等一系列手动流程来完成的。或许年轻的你对于如今电子邮件和即时通讯迅猛发展的世界里，觉得不可思议。现在有了自动化的程序来实现自这一流程的自动化，通过使用电子签名，跟踪并处理提交的内容。

为满足公司的更多需求，自动化工具也变得越来越庞大且规模化。它可以准确的告诉管理员都有谁为项目做出贡献，甚至可以帮助管理员去处理那些导致项目拖沓的日常摩擦。

据微软声称，在微软的开源项目办公室，大约在GitHub上托管了8000个项目，牵涉到的贡献者有11000多，在2016年，约有40000个内部请求被用于开源项目。为了管理这些请求，以及所创建的代码和正在更新的代码版本，公司转而使用可以自动化解决混乱的工具。不仅如此，由于数百个项目中很可能会共用同一段代码，因此必须对其进行仔细跟踪，以便在出现安全错误时，可以快速绘制并修复所有的软件影响。在如此大规模的情况下，自动化非常关键，手动更新几乎是不可能的。

下图展示了微软的一个仪表盘：

![Microsoft’s Azure open source portal displays useful information such as the number of daily users on GitHub. Source: https://www.jeff.wilcox.name/2015/11/azure-on-github/](images/tools-for-managing-open-source-programs1.png)

### 管理关键任务

其它一些有助于管理关键任务重要的工具也是要考虑并上线的，如项目管理、跟踪项目健康度、能够确保让开发者、开源社区、公司内部之间快速而清晰沟通的工具等等。

### 源代码管理

目前，绝大多数的公司软件项目都使用 [GitHub](https://GitHub.com/about) 来作为集中的托管和开发平台，尤其是拥有开源项目办公室的公司。

GitHub 是一家在线的源代码管理站点，其允许开源开发者们去管理和托管代码，相当于一个中心化的“仓库”或者叫存储空间，在这里大家可以协作参与从而一起构建代码。如今，大约有6400万个开源代码项目在GitHub上托管，涉及大约2300万个开发人员。

GitHub 的用户可以添加代码、审核所提交的代码、申请更改、收获或者提交反馈，并且提供项目管理的服务。GitHub 使用的是[Git 版本控制系统](https://git-scm.com/)，Git 是由著名的 Linux 创始人 Linus Torvalds 所开发，其旨在为组织代码和基于开源的人们的协作解决分布式的问题。每个“贡献者”均有一份项目仓库属于自己的拷贝，这些“贡献者”可以在自己的本地进行更改，然后提交回去，以便于未来进行合并。

GitHub 最具特色的莫过于流行日久的“pull request”, 通过 PR 开发者可以提交代码、然后进行审核、讨论、修改以及最后的批准或者修改。

### 许可证合规

同样重要的是代码的扫描和合规性工具的使用，它们有助于追踪代码起源和许可要求。对于公司来说，监视开源代码引入到自身的基础设施、产品和服务确保许可证是满足需求的，这实在是太重要了。

举例来说，贵司有一个应用，其中包含了上千个开源组件，为了保护贵司免于法律纠纷，了解这些开源组件的细节是非常重要的。在风险较高的情况下，用户必须根据其业务，进而定位风险谱中的所处位置，通过深入的代码扫描，能够更加深入地审核并验证许可证的合规性。（具体请参考使用和分发开源代码指南）

> “作为开源项目办公室的负责人，你必须了解项目的风险状况，因为扫描的最终目标是和风险管理相关的。或许你采取鸵鸟政策，对于潜在的风险当做视而不见。或许你会很明智的提前想到：”假如公司被起诉，会严重影响到公司的业务“，那么就会慎重对待。所以，你要自己开始检视自己，逐行的审核代码，任何可能的风险都不要放过。” – [Jeff McAffer](https://twitter.com/jeffmcaffer), 微软开源项目办公室总监

## Tools for managing source code

尽管我们刚刚讨论了目前大多数的开源项目办公室均使用GitHub作为源代码管理系统，但是仅仅使用GitHub是无法满足所有需求的，尤其是贵司的规模很大的时候。

在开源的世界中，有些工具仅仅是为了改进 GitHub 自身所欠缺的功能，如支持检查开发者原创认证（DCO）代码，以确保代码可以被合法授权且应用于开源项目中。

GitHub 同样也在代码的审核方面有些不足之处，所以在方面就有一些增强的工具，比如可以为贡献者自动回复关于代码问题的issue或PR，并要求他们检查并作出修改。GitHub 本身并没有实现让人强迫去检查他们的代码，而这些增强的工具弥补了这一点，进而让开发的流程有所改进。

还有一些针对 GitHub 特定的工具，如扩展了性能指标能力的相关，这些功能通常针对特定的项目，而不是提供整个公司层面的详细信息。对于公司维护多个开源代码仓库，而且是跨 GitHub 的项目管理，那么就有对以公司为单位的统一管理的需求。亚马逊，Netflix和微软均开发了大量这样的工具来帮助完成这些需求。

以下是一些最流行和实用的源代码管理工具，可以帮助贵司轻松驾驭 GitHub：

**源代码扫描和许可证合规**

[Antepedia Reporter](http://www.antepedia.com/pages/tools.html) –  这是一款商业收费应用，由 Antepedia 公司出品，它是一款报告生成的工具，可以让开发者、项目经理、法律顾问、以及诸如创建许可证合规的审计者、知识产权管理使用的报告，当然都是公司代码仓库关于开源的、公开的或者私有组件。

[Black Duck Hub](https://www.blackducksoftware.com/products/hub) – 这也是一款商业的整合服务，其可以扫描代码以识别所有嵌入的开源组件，还可以自动搜索已知的漏洞并进行修复。另外在其发现新的漏洞时还会发出告警。

[Black Duck Protex](https://www.blackducksoftware.com/products/protex) – Protex 是一款商业的，基于付费的许可证合规管理工具，来自黑鸭子公司，Protex 还整合了该公司其它的软件，可以实现自动化的代码扫描、认证、清点开源软件，同时执行许可证合规性和公司政策的要求。

[版权所有审核工具](https://wiki.debian.org/CopyrightReviewTools) – 该系列工具用于命令行下帮助创建初始的版权所有文件，并使之在以后的更新和审核中更为容易。

[dep-checker](http://git.linuxfoundation.org/dep-checker.git/) – 由 Linux 基金会所开发的一款依赖检测工具，该工具会在代码的包之间检查分析所有的关联依赖。

[FlexNet Code Insight](https://www.flexerasoftware.com/enterprise/products/software-vulnerability-management/flexnet-code-insight/) – Flexera于2016年收购了许可证合规性供应商Palamida，提供了FlexNet Code Insight，以帮助开发人员、法律团队和安全人员自动化企业开源应用。

[FOSSA](http://fossa.io/) – 这是一款商业工具，可自动执行代码依赖性跟踪和后台许可证合规性的扫描。

[FOSSology](https://www.fossology.org/) – Linux 基金会的项目，FOSSology是一个开源许可证合规性软件工具包，它可以从命令行运行许可证、版权并导出控制扫描。它还包含了一个数据库和Web UI，这些也都可用于创建合规工作流程。

![The Linux Foundation’s FOSSology compliance tool](images/tools-for-managing-open-source-programs3.png)

[janitor.git](http://git.linuxfoundation.org/janitor.git/) – Code Janitor 是一款开源工具，旨在帮助提升源代码符合开源许可证的合规。同样由Linux基金会托管， [Code Janitor](https://www.linuxfoundation.org/sites/default/files/lf_foss_compliance_cjt.pdf) 可以与其他产品一同使用以检查代码。

[LicenseFinder](https://github.com/pivotal/LicenseFinder) – 为项目所使用的代码探测许可证，将这些许可证与用户定义的白名单进行比较，并提供可操作的报告。

[Protecode Enterprise Analyzer](http://www.protecode.com/our-products/system-4/enterprise-analyzer/) – 这款商业应用程序用于分析和识别任何目录中的所有代码， 以确定代码的所有权并根据预先确定的内部政策确保开源许可证合规性。

[scancode-toolkit](https://github.com/nexB/scancode-toolkit) – 来自于 nexB 的 ScanCode 工具套件，可以扫描代码的许可证、版权和代码依赖性，从而查找、发现和清点代码中所使用的开放源代码和第三方组件。

[SPDX](https://spdx.org/tools) – 软件包数据交换 (简称SPDX) 是一套规范，是关于软件包相关的组件、许可证和版权的标准，SPDX标准通过标准化开发人员和公司之间共享许可证信息的方式，帮助遵守免费和开源的软件许可证。SPDX规范由Linux基金会主办的SPDX工作组所开发的。该工作组还提供了 The group offers open source [工具](https://spdx.org/tools)，用来帮助用户使用 SPDX 文档。

[WhiteSource](https://www.whitesourcesoftware.com/) – 通过自动且持续的扫描十多个开源仓库，进而实现实时的提供许可证、安全、代码质量以及报告分析，来管理开源的组件。

### 缺陷和 issue 跟踪

[Bugzilla](https://www.bugzilla.org/) – 传统的服务端-客户单模式软件，具有搜索记忆功能的高级查询工具，而且集成电子邮件功能，同时也拥有完善的权限控制。著名的[Mozilla](https://bugzilla.mozilla.org/) 项目使用 Bugzilla来作为他们的缺陷跟踪系统。

[GitHub Issues](https://help.github.com/articles/about-issues/) – GitHub 自身所集成的用户收集反馈和缺陷跟踪，GitHub issue 是作为GitHub项目托管的一部分提供给用户。

[GitLab](https://about.gitlab.com/) – 该项目在统一的界面中集成了缺陷跟踪、代码审核、Git仓库管理、活跃示意、维基百科等等，从而希望让用户完成开源项目的协作。

[JIRA](https://www.atlassian.com/software/jira) –来自于 Atlassian 公司的 JIRA，实现了完整的缺陷跟踪，该系统还包含自定义过滤器、开发人员工具整合、可定制的工作流程和丰富的 API 等高级功能，最重要的是 JIRA 可以和 Atlassian 公司的其他应用整合在一起。

### 归档和发布管理

[Artifactory](https://www.jfrog.com/artifactory/) – 同样来自于 JFrog 公司， Artifactory 是一款仓库管理者，支持任何语言的软件包创建，它还整合了几乎所有主流的 DevOps 和持续集成、持续部署的工具。

[Bintray](https://bintray.com/) – 一款来自于 JFrog 的归档工具，允许公司发布他们的代码发布档案以维护更久远和更庞大文件的存储。

[Docker Hub](https://hub.docker.com/) – 基于云服务的注册服务，其允许上传代码到其仓库，并构建、测试所生成的镜像。它还可以存储手动推送的镜像，并可连接到 [Docker Cloud](https://docs.docker.com/docker-cloud/) ，这样用户就可以部署镜像到托管的主机。Docker Hub 是一个中心化的资源，用户容器镜像的发现、分发、以及变更管理，甚至是通过开发的管道来完成协作和工作流自动化。

[github-release](https://github.com/aktau/github-release) – GitHub 内置功能之一，其允许用户[打包并编辑](https://help.github.com/articles/about-releases/) GitHub 上的项目发布，以便其他社区成员可以使用它们。

## Tools for tracking project health

对于企业的开源项目来说，随着项目的增长和成熟，监控和跟踪这些项目的整体健康程度是他们的核心任务。为了能够实现或完成这个任务，作为开源项目办公室的负责人，你必须整合一些工具，用来报告每个单独开源项目的表现，以及他们社区的反馈，这通常会涉及到很多很多的项目。另外，这些工具还可以实现将数据转化更加有意义、实用、可操作的信息，从而将整个的开源项目的绩效表现出来。

![Amazon’s Open Source Program Dashboard can be used to view and monitor many GitHub organizations and/or users at one time. Source: https://github.com/amzn/oss-dashboard](images/tools-for-managing-open-source-programs4.png)

这里最起码的底线是，尽量收集那些重要且有用的信息，而不是那些看似花哨却无用的信息，比如常见的项目有多少被关注的星星数、亦或是从项目启动伊始有多少贡献者参与、等等之类没啥含金量的信息。

最好的项目健康工具，除了上述功能之外，还应该可以帮助项目团队很好的响应社区：同时鼓励贡献开发者的参与和多样化的氛围。这也就意味着，这些工具可以协助维护者快速的响应社区成员提出的或反馈的问题，从而能够激励这些参与者的热情，而不是让他们觉得心灰意冷，转投到其它的社区。

每个开源项目的社区是不同的，有些项目的社区拥有大量的贡献者，也有的有着小而精的团队。无论如何，你所选择的项目健康跟踪工具应该可以适应各种规模的社区。

> “就现有的工具和系统来说，我希望毋须创建任何的工具和技术就可以实现公司开源项目办公室的目标，人们应该去寻找并使用现成的工具来管理开源项目。” – [Jeff McAffer](https://twitter.com/jeffmcaffer), 微软开源项目办公室总监

以下所列出的是目前比较流行的用于项目统计和项目健康度跟踪的工具集：

* [CatWatch](https://github.com/zalando-incubator/catwatch) – CatWatch 是一款开源的指标集中呈现的工具，由 Zalando 开发，CatWatch 会基于你的GitHub账号从GitHub站点拉取统计信息，然后将之处理、保存到数据库，这些数据会包括你开源项目的受欢迎程度、你的最活跃的贡献者以及其它有趣的统计信息。
* [Gander](https://github.com/paypal/Gander) – Gander 是一款为快速查看一系列开源项目生成使用指标的仪表工具。 Gander 由 PayPal 创建，专为负责运行开源项目办公室或跟踪多个开源项目的人员而设计。
* [GHCrawler](https://github.com/Microsoft/ghcrawler) – 由微软所发起的项目，是一款基于 GitHub API 所写的爬行程序， 用于抓取在 GitHub 托管的项目并自动追踪、检索和存储其内容。GHCrawler主要适用于组织的跟踪以及相关数据的存储。
* [Gittagstats](https://github.com/mcharleb/gittagstats) – Gittagstats是一款根据Git仓库的一组标签生成统计数据报告的工具。该工具由Qualcomm创建。
* [GrimoireLab](https://grimoirelab.github.io) – GrimoireLab 有着各式各样的开源工具，能够衡量开源项目的统计信息且将这些信息可视化，如Git 仓库、GitHub Pull Request、Bugzllia 的Ticket、以及邮件列表、Meetup小组、Slack频道等等。GrimoireLab 是[CHAOSS](https://chaoss.community) 下的一个项目，CHAOSS 是一组开源开发指标的协作工具集。
* [OSS-dashboard](https://github.com/amzn/oss-dashboard) – 来自亚马逊的开源项目呈现工具，是一款多功能仪表盘，可用于一次性同时查看和监视多个 GitHub 的组织和用户。
* [OSS Tracker](https://github.com/Netflix/osstracker) – 由 Netflix 发起的OSS Tracker，可以收集 GitHub 上基于组织的数据，且可以将该组织下所有的项目整合呈现在单个用户界面，所有的仓库均会被列出，所有的该组织下指标项均会被合并，而且社区管理员还可以组织项目到不同的功能区域，且可指派管理员给管理和工程相关。

> “使用这些工具的最终目的，就是通过这些透明的数据和相关的指标信息，能够为公司提供参考。” – [Chris Aniszczyk](https://twitter.com/cra), 云原生计算基金会首席运营官

TODO 小组 还提供了另外一份 [很有帮助的工具清单](https://GitHub.com/todogroup/awesome-oss-mgmt) :

### 更好的代码审核工具：

* [mention-bot](https://github.com/facebook/mention-bot) – 由 Facebook 所开发，该工具会自动地为代码贡献者提醒到可能的代码审核人员，从而加速审核的流程。
* [PullApprove](https://about.pullapprove.com/) – 通过同行审查改进代码质量、执行格式准则、捕获错误代码以及提供代码安全检查的形式，从而使代码贡献或pull request更加规范化。
* [sentinel](https://github.com/habitat-sh/sentinel) – 这是一个仓库管理机器人，其可以审核和测试代码，并会为仓库构建一个维护者列表，还能够与用户沟通 pull request的进展状态。

### 用于贡献者许可协议（CLA）

[CLA Assistant](https://github.com/cla-assistant/cla-assistant) – 由 SAP 提供的 CLA Assistant 通过处理用户贡献的合法部分来简化工作流程。当代码贡献者提供代码时，CLA Assistant 要求他们签署 CLAs 并通过 GitHub 帐户对每个贡献者进行身份验证。它还会在贡献者同意 CLA 时更新 Pull  equests的状态，并自动要求用户在对 CLA 进行更改时为每个新的 Pull Request重新签署CLA。

![SAP’s CLA Assistant tool](images/tools-for-managing-open-source-programs5.png)

[CLA Portal](https://github.com/vmware/claportal) –由 VMware 发起，CLA Portal 为 GitHub 增加了一个流程，以使贡献者能够在GitHub存储库中签署关于 Pull Requests 的贡献者许可协议。当开发人员发出pull requests时，会提示他们在需要时签署协议。同时包括一个为 CLA 创作、CLA-to-project 绘制和协议审查建立的管理员界面。

[DCOB](https://github.com/chef/dcob) –  一款开发者原创证书机器人，其可以帮助增强开发者为每个 Pull Request 的代码变更都加上原创认证。DCOB 会为每个接受的代码变更设置状态，完全遵照[开发者原创认证](http://developercertificate.org/)的要求。

### 公司级较大规模的 GitHub 管理

* [hubcommander](https://github.com/Netflix/hubcommander) - 该工具是一款基于 Slack 机器人，用于 GitHub 的组织管理，HubCommander 使用 Chat-ops 或者叫做”对话驱动” 的理念，来帮助管理 GitHub 的项目，它实现了一种简单的方式完成 GitHub 组织管理的任务，而不是那些繁琐的权限赋予的流程。
* [opensource-portal](https://github.com/Microsoft/opensource-portal) – 由微软研发的工具，旨在帮助大型企业进行大规模的GitHub 管理操作。这是微软开源项目办公室提供的一套工具之一。
* [settings](https://github.com/bkeepers/github-configurer) – 此应用程序将.github/settings.yml中定义的存储库设置同步到GitHub中，从而启用存储库的 pull requests。
* [zappr](https://github.com/zalando/zappr) - Zappr 是一款 GitHub 集成的用于增强项目工作流的工具，Zappr 由 Zalando 发起，旨在帮助开发者增加生产力，并改进开源项目的质量，主要是围绕 Pull Request 审批的瓶颈改善、帮助项目所有者在合并到项目主要分支之前暂停劣质pull requests等方式实现。

### 项目质量

* [CII Best Practices Badging](https://bestpractices.coreinfrastructure.org/) – 由 Linux基金会所开发和维护，核心基础设施发起者（CII）最佳实践套件，是 Free/Libre and Open Source Software (FLOSS)项目展示其遵循最佳实践的方式。通过使用这个Web应用程序，项目可以自愿进行免费的自我认证来解释他们如何遵循最佳实践。
* [CodeClimate](https://codeclimate.com/) – Code Climate 授权组织通过在整个开发流程中引入完全可配置的测试覆盖率和可维护性数据，从而实现代码质量的控制。它对开源项目是完全免费的！


## Tools for communications and collaboration

毫无疑问，开源的开发绝不仅仅是只有代码就可以的。一个健康运转的社区是开源项目的充分条件，社区为来自公司内外的许多不同背景的人之间的协作提供了可能，当然毫无例外，开源项目办公室的工作人员更加要和社区紧密的联系。

对于开源的开发者来说，尤其是稍微有些历史的社区参与者，对于一些沟通和协作工作不用说早已经轻车熟路了，如[IRC](http://www.irc.org/links.html)，开发者可以利用 IRC 来进行实时的沟通，详情请参考[更为传神的描述](http://blog.andrewray.me/irc-the-secret-weapon-of-developers/)。另外一个例子是[TWiki](http://twiki.org/)，这是开源的企业级的维基百科，开发者可以利用该协作平台进行日常的代码讨论或者项目相关的内容。

此外，企业还可以通过社交媒体平台，门户网站，开源项目代码仓库以及其它的通道入口，进行提问和讨论，进而促进沟通交流。

其它一些有用的工具，如 Facebook 发起的[mention-bot](https://github.com/facebook/mention-bot)项目，该工具会自动地为代码贡献者提醒到可能的代码审核人员，从而加速审核的流程。当贵司 GitHub 项目颇具规模之时，社区成员们已经无法通过订阅项目通知来获悉状况时，这一工具尤其值得推荐。

当然还有颇为流行的 [Slack](https://slack.com/)工具，不用多说，这是一款在线的团队项目管理和沟通的平台，在该平台下用户可以访问和分享信息、文件、组织工作流、以及历史信息检索等等，Slack 还可以配置为接受支持请求的通知、代码签入、错误日志、以及其它常见的任务等等。

最后要提醒的就是，贵司的公共关系和营销人员，也应该是参与和支持开源的重要有生力量。一些重要的社交媒体如Twitter，Reddit，Facebook，LinkedIn，Google+等，以及公司的官网和博客均是沟通的有效渠道。客户关系管理（CRM）软件、电子邮件群发、新闻简报统统都可以帮助公司让客户了解开源的最新进展。

## Tools for corporate-scale GitHub management

说了这么多，其实对于贵司来讲，提供和使用管理开源项目工具之时，最为重要的还要看帮助公司管理企业级的 GitHub 相关运营的工具。尽管 GitHub 能够满足绝大多数的需求，已经很完美了，但是对于大型、复杂的公司，如巨头Google、微软、Facebook、Twitter、Linkedin等等，就显得力不从心，会有很多意想不到的需求难以满足。

这些大型的企业会需要更多的功能，如认证管理、设置和权限管理、安全和双因子认证增强等，甚至包括代码仓库的深度检测和跟踪。

特别需要指出的，自动化的处理一些诸如员工入职、离职、增强的安全规则、赋予开发者访问仓库权限等等的工具是必须的。

这里列举微软为例，微软为了满足自身独特的需求，从头构建了自身的工具，从而实现简化和改进相关开源项目。迄今为止，微软在 GitHub 上[健壮地运行着](https://github.com/Microsoft)超过1,345 个仓库，参与人员多达 3,580 名。

> “随着贵司的扩展，GitHub 的项目管理会日益越发的重要起来，你掌管着GitHub的组织，那意味着是众多的仓库，多个团队，以及日渐增长的开发者成员，管理所有的事情开始复杂起来了，尤其是规模大到数百个代码仓库、数百位贡献者、跨多个组织的时候。” – [Jeff McAffer](https://twitter.com/jeffmcaffer), 微软开源项目办公室总监

微软所做的其中一件事就是，创建了可定制构建的自助服务的 [GitHub 管理和上线门户](http://www.jeff.wilcox.name/2015/11/azure-on-github/)，用于组织其项目、代码仓库、和团队。就其最基本的功能来说，基于 Web 的门户允许开发人员将他们的微软公司ID映射到他们的GitHub ID，这可以提高系统安全性并帮助简化参与大量重要项目的大量开发人员的组织工作。

该门户还实现了员工基于 GitHub 和微软的认证关联，为员工的身份创建了一个“虚拟链接”，然后员工们就可以根据所赋予的权限、根据工作角色的任务来完成自己的工作了。如果员工离职了，这些系统就会调整，删除认证关联，或者重新根据需要分配权限。

该门户运行与多个云平台之上，通过采用缓存技术来保持会话和减轻 GitHub API 的压力。该门户，平均每天有大约1，000个独立用户会使用到。这些仅仅是微软的开源工作的不断发展的一部分，该工作现在包括超过10,000名正在使用、贡献和发布开放源代码的工程师。

## Final words

呵呵，从来没有人说过，贵司选择拥抱开源就能让事情变得更为简单。但是很幸运的是，作为出入开源世界的你，可以看到已经有很大一批公司已经走在了前面，包括如 Google、微软这样的IT巨头已经做了很多，而且提供了详细的路线图、代码、建议，相信这一切会让你的开源之路更为轻松些。

创建开源项目办公室，选择一些重要的工具，进而开始开展开源的相关工作，这一切都在作为开源项目办公室负责人你的手里。通过你所做的这一切，很可能已经激发了贵司开发者们的极大期望，而且他们很可能已经参与开源项目中了（很有可能是在工作之余，隐秘的进行着）。

通过和开源项目的协作，并且邀请他人参与到贵司的项目，贵司将收获得难以估量的好处，进而形成正循环，以让创新推动公司发展。

使用合适的工具很重要，用好了可以有效的推动公司的开发式创新！切莫等闲视之。

## 致谢

贡献者：

* [Chris Aniszczyk](https://twitter.com/cra), 云原生计算基金会首席运营官
* [Jeff McAffer](https://twitter.com/jeffmcaffer), 微软开源项目办公室总监

> 这些资源是与TODO（公开对话，开放式开发）小组 – Linux基金会的专业开源程序网络小组合作创建的。 特别感谢那些贡献自己的时间和知识来制作这些综合指南的开源项目经理。 参与的公司包括Autodesk，Comcast，Dropbox，Facebook，Google，Intel，Microsoft，Netflix，Oath（Yahoo + AOL），Red Hat，Salesforce和Samsung。 要了解更多信息，请访问 [todogroup.org](http://todogroup.org/)。我们邀请您在GitHub上下载、传播，如果可以请积极的参与这些指南。
