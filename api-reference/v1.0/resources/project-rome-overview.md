---
title: 使用 Microsoft Graph API 处理 Project 罗马
description: 项目罗马是构建跨设备体验平台的 Microsoft 计划。 Project 罗马启用本地客户端或服务上的应用程序，以便在用户使用用于登录客户端设备的相同 Microsoft 帐户登录时与远程主机上的应用程序和服务进行交互。 这使您可以对用户任务（而不是设备）周围的跨设备和跨平台体验进行编程。
localization_priority: Normal
author: ailae
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 945d3925362c6d013fa411d9b586bca18c8a24a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037204"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 处理 Project 罗马

[项目罗马](https://developer.microsoft.com/en-us/windows/project-rome) 是构建跨设备体验平台的 Microsoft 计划。 Project 罗马启用本地客户端或服务上的应用程序，以便在用户使用用于登录客户端设备的相同 Microsoft 帐户登录时与远程主机上的应用程序和服务进行交互。 这使您可以对用户任务（而不是设备）周围的跨设备和跨平台体验进行编程。

通过 Microsoft Graph 公开一个关键组件，以启用以下体验：活动。

## <a name="activities"></a>活动

通过 Microsoft Graph 中的活动，您可以在设备和平台之间推动用户参与应用。 活动是用户接洽的单位，由三个组件组成：

- 深层链接
- 可视化表示形式
- 使用共享词汇描述活动的内容元数据 [https://schema.org/](https://schema.org/)

当应用程序创建会话时，会向活动中添加一个历史记录项目，以反映用户参与的时段。 用户每次 reengages 活动时，都会向活动中添加一个新的历史记录项，以计入用户约定。

当应用程序发布用户活动对象时，该对象将显示在 Windows 中的一些新 UI 图面上;例如，Cortana 通知和时间线。 您可以指定丰富的元数据 (，以允许在活动对象中使用 [自适应卡片](https://adaptivecards.io/) 标记) 仅在适当的上下文中显示活动) 和丰富的视觉对象 (。

您可以使用以下 Microsoft Graph Api 来创建和检索用户活动：

- [创建或替换活动](../api/projectrome-put-activity.md)
- [获取活动](../api/projectrome-get-activities.md)
- [获取最近的活动](../api/projectrome-get-recent-activities.md)
- [删除活动](../api/projectrome-delete-activity.md)
- [创建或替换历史记录项](../api/projectrome-put-historyitem.md)
- [删除历史记录项](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
