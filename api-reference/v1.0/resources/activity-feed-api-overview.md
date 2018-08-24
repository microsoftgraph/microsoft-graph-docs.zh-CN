# <a name="use-the-activity-feed-rest-api"></a>使用活动源 REST API

您可以使用的活动源 API 在 Microsoft Graph 中恢复用户在设备和平台上的活动。 活动源 API 请求代表用户通过 [委派权限](../../../concepts/permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions)和[用户活动权限](../../../concepts/permissions_reference.md)执行，可用于个人或工作和学校帐户。 

用户活动由 [activity](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity) 资源表示，以基于时间且以集合中的 me/activities 表示的源来组织。 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>什么是构成好的用户活动的因素？

用户活动不只是启动应用程序——它们是深入到您的应用程序中的特定内容的链接。 您创建的用户活动不仅可用于您自己的应用程序，也将显示在 Cortana 和 Windows 时间线中，从而推动更多的应用程序后续互动，并让用户可以继续在多个设备上使用您的应用程序。  

### <a name="what-should-become-an-activity"></a>什么应成为活动？ 

由于每个应用程序都不同，每个应用程序开发人员应了解将用户活动映射到应用程序中的操作的最佳方式。 例如，游戏可能为每个关卡创建活动、文档创作应用程序可能会为每个唯一的文档创建活动，业务线应用程序可能会为每个工作流创建活动。 

在应用程序中定义活动时请应用以下准则：

**建议：** 为一组相关的用户操作记录单个活动。 如果您的应用程序用于相关内容的序列，可能将整个交互会话记录为单个活动比较合理。  

*播放列表方案：* 这与音乐播放列表或电视节目密切相关，可更新单个用户活动以显示您的进度。 在这种情况下，您的单个用户活动将拥有多个[历史记录项](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_historyitem)，它们代表跨多天或数周的交互时间段。  

**建议：** 存储用户数据到云中。 如果您想要支持跨设备活动，需要确保将后续开展此活动所需的内容存储到云端。 例如，如果在用户每次编辑文档时发布一个活动，文档应存储在云中而不是用户设备上的本地位置，以支持跨设备后续开展互动。  

**不建议：** 为用户无需将来继续的操作创建用户活动。 如果应用程序用于完成不会维持状态以用于将来跟踪的简单、一次性操作，可能不需要写入用户活动。 

为说明问题，即使用户活动显示在 Windows 日程表，这不是作为版本控制工具——选择基于文档的活动应始终显示最新版本的文档 （包括由其他用户所做的更改）。

**不建议：** 为由*其他用户*完成的操作创建用户活动。 如果某人在您的应用程序 中向用户发送消息或以 @ 提及用户，您不应编写新活动。 这些交互可通过显示通知来更好地满足需求。  

*协作方案：* 如果多人正在使用同一个活动 （如 Word 文档），将会存在您最后编辑后又有另一个用户对其更改的情况。 在这种情况下，应用程序开发人员可能要更新活动中的可视元素，以反映对文档进行的更改。 若要执行此操作，应用程序可能更新现有的活动而不创建新的历史记录项。 

>**注意：** 如果您发布 Web 应用程序的活动，请务必同时在您的每个活动包括 `activationURL` 和 `fallbackURL`。 活动将按预期方式将用户从类似于 Windows 日程表的 Microsoft 体验中启动回您的应用程序。 

## <a name="app-interaction-patterns-and-user-activities"></a>应用程序交互模式和用户活动 
您创建的用户活动取决于应用程序的交互模式。 虽然每个应用程序均有所不同，但大多数将归为以下交互模式之一： 

* **基于文档的应用程序**——为每个文档创建一个活动，以一个或多个历史记录反映使用的时段。 重要的是，如对文档进行了更改，需要更新活动卡。 
* **媒体播放应用程序**——针对每一组逻辑内容组合创建活动，例如播放列表、程序或独立内容。 
* **游戏**——为每次保存的游戏或打造的场景创建一个活动。 如果您的游戏支持单个序列的级别，可以随时间推移而写入同一个活动，但您可能要更新您的卡片显示您最新的进度或成绩。 
* **实用程序**——如果应用程序 中没有任何用户想要恢复的内容，不应发布活动。 较好的示例是一个简单的单一用途应用程序，如计算器。 
* **业务线应用程序**——用于管理简单任务或工作流而存在多个应用程序。 为您的应用程序访问每个单独的工作流创建一 个活动。 例如，每个零用金报销单应为单独的活动，因为您可能希望单击以查看活动是否已获批准。

*某些复杂的应用程序包括多个交互模式。您可能需要针对应用程序处理的不同方案而应用不同的用户活动创建模式。*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>后续步骤

- 请参阅 [活动资源](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity)，并定义您的应用程序的活动，以帮助用户继续重要任务。
- 浏览[自适应卡示例](http://adaptivecards.io/samples/)，以使您的活动**吸引用户**。  
- 尝试 [Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer)中的 API。

**寻找相关详细信息？** 
- 请参阅 [Microsoft 的体验如何使用活动](https://channel9.msdn.com/events/Build/2017/B8108)。
- 了解[活动源 API 和恢复中断的操作](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011)。
