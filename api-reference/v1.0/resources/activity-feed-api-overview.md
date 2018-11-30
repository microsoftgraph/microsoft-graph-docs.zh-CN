---
title: 使用活动源 REST API
description: '您可以使用的活动源 API 在 Microsoft Graph 中恢复用户的 actiity 设备和平台。 代表用户通过委派的权限和用户活动权限，可用于个人或工作和学校帐户执行活动订阅源的 API 请求。 '
ms.openlocfilehash: 25b7af22671256a6dd48536a7da232f16251184f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008116"
---
# <a name="use-the-activity-feed-rest-api"></a>使用活动源 REST API

您可以使用的活动源 API 在 Microsoft Graph 中恢复用户的 actiity 设备和平台。 代表用户通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[用户活动权限](/graph/permissions-reference)，可用于与个人或工作和学校帐户执行活动订阅源的 API 请求。 

用户活动由[活动](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_activity)资源和组织中的基于时间的源表示在集合中的我 / 活动。 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>什么使很好的用户活动？

用户活动不只是启动应用程序 — 它们是深入到您的应用程序中的特定内容的链接。 您创建的用户活动不仅可在您自己的应用程序，但也将显示在 Cortana 和 Windows 时间线 — 推动多个应用程序 reengagement 和简化您的用户可以继续使用多个设备的应用程序。  

### <a name="what-should-become-an-activity"></a>什么应成为活动？ 

由于每个应用程序不同，这取决于每个应用程序开发人员了解将映射到用户活动应用程序中的操作的最佳方式。 例如，游戏可能创建活动的每个市场活动、 文档创作应用程序可能会创建每个唯一的文档，活动和业务线应用程序可能会创建每个工作流活动。 

在您的应用程序中定义 activitites 应用以下准则：

**执行操作：** 记录一组相关的用户操作的单个活动。 如果您的应用程序用于序列的相关内容，可能有意义的整个项目会话记录的单个活动。  

*播放列表方案：* 这是音乐播放列表或 TV 显示密切相关 — 单个用户活动可以更新以显示您的进度。 在这种情况下，您将拥有多个[历史记录项](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_historyitem)的项目的时间段代表跨多个天或数周单个用户活动。  

**执行操作：** 存储到云中的用户数据。 如果您想要支持跨设备活动，您需要确保所需 reengage 此活动的内容存储到云位置。 例如，如果用户在编辑文档的每次发布活动时，文档应存储在云中而不是用户的设备上的本地以启用跨设备 reengagement。  

**不：** 创建用户活动用户无需继续将来的操作。 如果您的应用程序用于完成简单、 一次性不会保留，用于在将来跟踪状态的操作，您可能不需要写入用户活动。 

要清除，即使用户活动显示在 Windows 日程表，这不是作为版本控制工具 — 选择基于文档的活动应始终显示的最新版本的文档 （包括由其他用户所做的更改）。

**不：** 创建用户活动完成由*其他用户*的操作。 如果某人发送用户的消息或 @mentions 用户在您的应用程序，您不应编写新活动。 这些交互更好地构成显示通知。  

*的协作方案：* 如果多人正在使用同一个活动 （如 Word 文档），将会情况下当另一个用户所做更改文档后最后一个编辑它。 在这种情况下，应用程序开发人员可能要更新的可视元素中活动的以反映对文档进行更改。 若要执行此操作，应用程序可能不创建新的历史记录项更新现有的活动。 

>**注意：** 如果您发布 web 应用程序的活动，请务必同时包括`activationURL`和`fallbackURL`您的活动的每个。 活动将回您的应用程序启动用户，按预期方式从 Microsoft Windows 日程表类似的体验。 

## <a name="app-interaction-patterns-and-user-activities"></a>应用程序交互模式和用户活动 
您创建的用户活动取决于您的应用程序的交互模式。 不同每个应用程序时，大多数将分为以下交互模式之一： 

* **基于文档的应用程序**— 这就反映了使用时段的一个或多个历史记录具有创建每个文档的一个活动。 非常重要更新活动卡，如对文档进行更改。 
* **媒体播放应用程序**— 创建的内容，例如播放列表、 程序或独立内容的逻辑分组每一个活动。 
* **游戏**— 游戏或打造为每保存创建一个活动。 如果您的游戏支持单个序列的级别，您可以随时间推移，编写同一个活动，但您可能要更新您的卡片显示您最新的进度或成绩。 
* **实用程序应用程序**— 如果没有任何应用程序的用户将想要恢复中，您不能发布活动。 较好的示例是一个简单的单一用途应用程序，如计算器。 
* **业务线应用程序**— 用于管理简单任务或工作流存在多个应用程序。 创建一个通过您的应用程序访问每个单独的工作流活动。 例如，每个费用报表应为单独的活动，因为您可能希望单击以查看是否它已批准的活动。

*某些复杂的应用程序包括多个交互模式。您可能需要关注的处理您的应用程序的不同方案的不同用户活动创建模式。*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>后续步骤

- 请参阅[活动资源](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_activity)，并定义您的应用程序的活动，以帮助用户继续重要任务。
- 浏览的信息，以使您活动**pop**[自适应卡示例](https://adaptivecards.io/samples/)示例。  
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。

**寻找相关详细信息？** 

- 请参阅[Microsoft 的体验如何使用活动](https://channel9.msdn.com/events/Build/2017/B8108)。
- 了解[活动源 API 和拿起回忆其中](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011)。
