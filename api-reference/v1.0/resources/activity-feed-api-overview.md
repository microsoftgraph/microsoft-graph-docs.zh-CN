---
title: 使用活动源 REST API
description: '可以使用 Microsoft 活动源 API Graph跨设备和平台恢复用户的活动。 活动源 API 请求通过委派权限和用户活动权限代表用户执行，这些权限可以与个人帐户或工作和学校帐户一同使用。 '
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: conceptualPageType
ms.openlocfilehash: 37b4a7113d0f52155d6fa8a96167600cf9a33a86
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056114"
---
# <a name="use-the-activity-feed-rest-api"></a>使用活动源 REST API

命名空间：microsoft.graph

可以使用 Microsoft 活动源 API Graph跨设备和平台恢复用户的活动。 活动源 API 请求通过委派权限和用户活动权限代表[](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)用户执行，这些权限可以[](/graph/permissions-reference)与个人帐户或工作和学校帐户一同使用。

用户活动由活动资源 [表示](/graph/api/resources/projectrome-activity) ，并且组织在由集合 me/activities 表示的基于时间的源中。
<!-- Add missing content.
Each activity represents a unique...
-->
## <a name="what-makes-a-great-user-activity"></a>什么是出色的用户活动？

用户活动不只是启动应用，而是指向应用中特定内容的深层链接。 你创建的用户活动不仅可用于你自己的应用，而且还会显示在 Cortana 和 Windows 时间线中 - 推动更多应用重新参与，并让用户更轻松地跨多个设备继续使用你的应用。

### <a name="what-should-become-an-activity"></a>什么应该成为活动？

由于每个应用都不同，因此由每个应用开发人员了解将应用程序中的操作映射到用户活动的最佳方法。 例如，游戏可能会为每个市场活动创建一个活动，文档创作应用可能会为每个唯一文档创建一个活动，业务线应用可能会为每个工作流创建一个活动。

在应用中定义活动时应用以下指南：

**DO：** 记录一组相关用户操作中的单个活动。
如果你的应用程序用于一系列相关内容，则记录整个参与会话的单个活动可能有意义。

*播放列表方案：* 这尤其与音乐播放列表或电视节目相关 - 可以更新单个用户活动以显示进度。 在这种情况下，你将具有单个用户活动，其多个历史记录项表示[](/graph/api/resources/projectrome-historyitem)数天或数周参与期。

**DO：** 将用户数据存储到云。
如果你想要支持跨设备活动，则需要确保重新参与此活动所需的内容已存储到云位置。 例如，如果每次用户编辑文档时发布活动，文档应存储在云中，而不是在本地用户设备上存储，以便启用跨设备重新参与。

**请勿：** 为用户将来不需要恢复的操作创建用户活动。
如果应用程序用于完成简单、一次的操作，这些操作不会保留状态，因此将来可能不需要编写用户活动。

为清楚说明，尽管用户活动显示在 Windows 时间线中，但这不是设计为版本控制工具 - 选择基于文档的活动应始终显示该文档的最新版本 (包括由其他用户所做的更改。) 

**请勿：** 为其他用户完成的操作创建 *用户活动*。
如果有人向用户发送消息，或@mentions应用中的用户发送邮件，则不应编写新活动。 通过显示通知可以更好地提供这些交互。

*协作方案：* 如果多个用户正在处理同一活动 (如 Word 文档) ，则在某些情况下，其他用户在您上次编辑文档后对其进行了更改。 在这种情况下，应用开发人员可能需要更新活动中的可视元素，以反映对文档所做的更改。 为此，应用可能会更新现有活动，而无需创建新的历史记录项。

>**注意：** 如果要为 Web 应用程序发布活动，则对于每个活动都包括 和 ，这 `activationURL` `fallbackURL` 一点很重要。 活动将用户从 Microsoft 体验（如时间线）中预期启动Windows应用。

## <a name="app-interaction-patterns-and-user-activities"></a>应用交互模式和用户活动
你创建的用户活动将因应用的交互模式而异。 虽然每个应用都不同，但大多数应用将属于以下交互模式之一：

* **基于文档的应用程序** — 每个文档创建一个活动，其中一个或多个历史记录反映了使用周期。 对文档进行更改时，更新活动卡片非常重要。
* **媒体播放应用** — 按内容（如播放列表、程序或独立内容）的逻辑分组创建一个活动。
* **游戏** — 为每个保存的游戏或世界创建一个活动。 如果你的游戏仅支持一系列级别，你可以随着时间的一段时间编写相同的活动，尽管你可能想要更新卡片以显示最新进度或成就。
* **实用程序应用** — 如果用户希望恢复的应用中没有任何内容，则不应发布活动。 一个很好的示例是一个简单的单用途应用，如计算器。
* **业务线应用** — 存在许多用于管理简单任务或工作流的应用。 为通过应用访问的每个单独工作流创建一个活动。 例如，每个费用报表都是一个单独的活动，因为您可能希望单击该活动以查看其是否得到批准。

*一些复杂的应用包含多个交互模式。对于你的应用处理的不同方案，你可能希望遵循不同的用户活动创建模式。*

<!-- Add content or remove H2.
## Common use cases
-->

## <a name="next-steps"></a>后续步骤

- 查看 [活动资源](/graph/api/resources/projectrome-activity) 并定义应用的活动，以帮助用户恢复重要任务。
- 浏览自适应 [卡片示例示例](https://adaptivecards.io/samples/) ，了解让活动弹出 **的创意**。
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。

**寻找更多想法？**

- 了解 [Microsoft 体验如何使用活动](https://channel9.msdn.com/events/Build/2017/B8108)。
- 了解 [活动源 API，并选取我离开的地方](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011)。
