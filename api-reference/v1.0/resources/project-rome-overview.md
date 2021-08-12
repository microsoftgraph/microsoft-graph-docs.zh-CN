---
title: 使用 Microsoft Graph API 处理 Project Rome
description: ProjectRome 是 Microsoft 构建跨设备体验平台的一项计划。 Project当用户使用他们用于登录客户端设备的同一 Microsoft 帐户登录时，Rome 允许本地客户端或服务上的应用与远程主机上的应用和服务交互。 这允许你对以用户任务而不是设备为中心的跨设备和跨平台体验进行编程。
localization_priority: Normal
author: ailae
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 4b011f217d4ef3f55afdafa6880e60a8cd38bf53cecadee70f4355dafbdb7642
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152311"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 处理 Project Rome

[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome)是 Microsoft 构建跨设备体验平台的一项计划。 Project当用户使用他们用于登录客户端设备的同一 Microsoft 帐户登录时，Rome 允许本地客户端或服务上的应用与远程主机上的应用和服务交互。 这允许你对以用户任务而不是设备为中心的跨设备和跨平台体验进行编程。

一个关键组件通过 Microsoft Graph实现以下体验：活动。

## <a name="activities"></a>活动

Microsoft Graph中的活动使你可以推动用户跨设备和平台与你的应用互动。 活动是用户参与度的单位，由三个部分组成：

- 深层链接
- 视觉表示形式
- 使用共享词汇描述活动 [https://schema.org/](https://schema.org/) 的内容元数据

当应用程序创建会话时，会向活动添加历史记录项以反映用户参与的时间段。 每次用户重新参与某个活动时，会向活动添加一个新的历史记录项，以增加用户参与度。

当应用程序发布用户活动对象时，该对象将显示在应用程序中的一Windows;例如，Cortana通知和时间线。 你可以指定丰富的元数据 (以允许在正确的上下文) 中显示活动，也可以指定 (活动对象中的自适应卡片标记) 丰富的视觉效果。 [](https://adaptivecards.io/)

可以使用以下 Microsoft Graph API 创建和检索用户活动：

- [创建或替换活动](../api/projectrome-put-activity.md)
- [获取活动](../api/projectrome-get-activities.md)
- [获取最近的活动](../api/projectrome-get-recent-activities.md)
- [删除活动](../api/projectrome-delete-activity.md)
- [创建或替换历史记录项](../api/projectrome-put-historyitem.md)
- [删除历史记录项](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
