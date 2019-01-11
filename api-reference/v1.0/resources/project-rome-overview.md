---
title: 使用 Microsoft Graph API 来处理项目 Rome
description: 项目 Rome 是 Microsoft 计划中，以构建一个跨设备体验平台。 当用户注销，使用客户端设备上登录这些用户使用同一 Microsoft 帐户时，项目 Rome 启用上进行交互的应用程序的本地客户端或服务应用程序和远程主机上的服务。 这将允许您围绕用户任务，而不是设备的程序跨设备和跨平台体验。
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840962"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 来处理项目 Rome

[项目 Rome](https://developer.microsoft.com/en-us/windows/project-rome)是 Microsoft 计划中，以构建一个跨设备体验平台。 当用户注销，使用客户端设备上登录这些用户使用同一 Microsoft 帐户时，项目 Rome 启用上进行交互的应用程序的本地客户端或服务应用程序和远程主机上的服务。 这将允许您围绕用户任务，而不是设备的程序跨设备和跨平台体验。

通过 Microsoft Graph 启用这些体验公开的关键组件： 活动。

## <a name="activities"></a>活动

跨设备和平台中，Microsoft Graph 中的活动使您能够与您的应用程序的驱动器用户工作效率。 活动用户工作效率的单位，包括三个组件：

- 深度链接
- 直观表示形式
- 描述该活动的内容元数据使用[https://schema.org/](https://schema.org/)共享词汇

应用程序创建会话时, 的历史记录项添加到活动的以反映用户工作效率期。 每次用户 reengages 与活动，新的历史记录项添加到活动以应计用户工作效率。

当应用程序发布用户活动对象时，该对象将显示某些 Windows; 中新的 UI 曲面例如，Cortana 通知和日程表。 活动对象中，可以指定丰富的元数据 （以允许活动在适当的上下文中呈现） 和丰富的视觉效果 （使用[自适应卡片](https://adaptivecards.io/)标记）。

以下 Microsoft Graph Api 可用于创建和检索用户活动：

- [创建或替换活动](../api/projectrome-put-activity.md)
- [获取活动](../api/projectrome-get-activities.md)
- [获取最近的活动](../api/projectrome-get-recent-activities.md)
- [删除活动](../api/projectrome-delete-activity.md)
- [创建或替换历史记录项](../api/projectrome-put-historyitem.md)
- [删除历史记录项](../api/projectrome-delete-historyitem.md)

