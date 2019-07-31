---
title: 使用活动源 REST API
description: '您可以使用 Microsoft Graph 中的活动源 API, 在设备和平台之间恢复用户的活动。 活动源 API 请求通过委派权限和用户活动权限 (可用于个人或工作和学校帐户) 代表用户执行。 '
localization_priority: Normal
ms.prod: project-rome
doc_type: conceptualPageType
author: ''
ms.openlocfilehash: 0e45fc94df443cb2067d5e5e492d4186ba074eeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013484"
---
# <a name="use-the-activity-feed-rest-api"></a>使用活动源 REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


您可以使用 Microsoft Graph 中的活动源 API, 在设备和平台之间恢复用户的活动。 活动源 API 请求通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[用户活动权限](/graph/permissions-reference)(可用于个人或工作和学校帐户) 代表用户执行。 

用户活动由[活动](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/projectrome_activity)资源表示, 并在由 "收藏"/"活动" 表示的基于时间的订阅源中进行组织。 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>什么使用户成为出色的活动？

用户活动不只是启动应用程序, 它们都是应用程序中的特定内容的深层链接。 您创建的用户活动不仅可以在您自己的应用程序中使用, 还会显示在 Cortana 和 Windows 时间线中—驱动更多的应用程序 reengagement, 使用户可以更轻松地在多个设备上继续使用您的应用程序。  

### <a name="what-should-become-an-activity"></a>什么应该成为活动？ 

由于每个应用程序都不同, 因此, 每个应用程序开发人员都可以了解将应用程序中的操作映射到用户活动的最佳方式。 例如, 游戏可能会为每个市场活动创建一个活动, 文档创作应用程序可能会为每个唯一文档创建一个活动, 并且业务线应用程序可能会为每个工作流创建一个活动。 

在应用程序中定义 activitites 时, 请遵循以下准则:

操作 **:** 记录一组相关用户操作的单个活动。 如果您的应用程序用于一系列相关的内容, 则记录整个参与会话的单个活动可能很有意义。  

*播放列表方案:* 这一点尤其适用于音乐播放列表或电视节目-可以更新单个用户活动以显示进度。 在这种情况下, 您将有一个用户活动, 其中多个[历史项目](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/projectrome_historyitem)表示一段时间内多天或几周的服务。  

操作 **:** 将用户数据存储到云。 如果要支持跨设备活动, 则需要确保将 reengage 此活动所需的内容存储到云位置。 例如, 如果您在每次用户编辑文档时发布活动, 则应将文档存储在云中, 而不是在用户的设备上本地存储, 以便启用跨设备 reengagement。  

**请勿执行以下操作:** 为用户无需在将来恢复的操作创建用户活动。 如果您的应用程序用于完成简单的一次性操作, 这些操作不会保留状态以供将来跟踪, 则您可能不需要编写用户活动。 

若要清楚, 即使用户活动出现在 Windows 日程表中, 也不会将其设计为版本控制工具—选择基于文档的活动应始终显示该文档的最新版本 (包括其他用户所做的更改)。

**请勿执行以下操作:** 为*其他用户*完成的操作创建用户活动。 如果某人向用户发送邮件, 或在您的应用程序中 @mentions 用户, 则不应编写新活动。 通过呈现通知, 可以更好地提供这些交互。  

*协作方案:* 如果有多个用户在同一个活动 (如 Word 文档) 上工作, 则在您最后一次编辑文档后, 其他用户已对其进行了更改。 在这种情况下, 应用程序开发人员可能需要更新活动中的可视元素, 以反映对文档所做的更改。 若要执行此操作, 应用程序可能会更新现有活动, 而不会创建新的历史记录项。 

>**注意:** 如果要为 web 应用程序发布活动, 请务必同时`activationURL` `fallbackURL`为每个活动包含和。 这些活动将从 Microsoft 体验 (如 Windows 日程表) 按预期方式将用户重新启动到应用中。 

## <a name="app-interaction-patterns-and-user-activities"></a>应用交互模式和用户活动 
您创建的用户活动将根据您的应用程序的交互模式而变化。 虽然每个应用程序不同, 但大多数都属于以下交互模式之一: 

* **基于文档的应用程序**-为每个文档创建一个活动, 其中包含一个或多个历史记录, 并反映使用时间段。 对文档进行更改时, 更新活动卡非常重要。 
* **Media 回放应用**—根据内容 (如播放列表、程序或独立内容) 的逻辑分组创建一个活动。 
* **游戏**—为每个已保存的游戏或世界创建一个活动。 如果你的游戏仅支持一系列级别, 则可以在一段时间内编写相同的活动, 尽管你可能需要更新卡片以显示你的最新进度或成就。 
* **实用程序应用**程序-如果用户要恢复的应用程序中没有任何内容, 则不应发布活动。 一个很棒的示例是简单的单一用途应用 (如计算器)。 
* **业务线应用程序**—用于管理简单任务或工作流的许多应用程序都存在。 为通过您的应用程序访问的每个单独的工作流创建一个活动。 例如, 每个零用金报销单都是一个单独的活动, 因为您可能想要单击该活动以查看该活动是否已获得批准。

*一些复杂的应用程序包含多个交互模式。您可能需要针对应用程序处理的不同应用场景遵循不同的用户活动创建模式。*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>后续步骤

- 查看[活动资源](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/projectrome_activity)并定义您的应用程序活动, 以帮助用户恢复重要任务。
- 浏览[自适应卡示例](https://adaptivecards.io/samples/)示例, 以获取活动**pop**的创意。  
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。

**是否要查找更多创意？** 

- 了解[Microsoft 在使用活动时的体验](https://channel9.msdn.com/events/Build/2017/B8108)。
- 了解[活动源 API 并获取我离开的位置](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011)。
