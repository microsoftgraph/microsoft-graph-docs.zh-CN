---
title: 使用 Microsoft 图形 API与Project罗马合作
description: Project罗马是一项 Microsoft 计划，旨在构建跨设备体验平台。 Project罗马允许本地客户端或服务上的应用在用户使用用于在客户端设备上登录的同一 Microsoft 帐户登录时与远程主机上的应用和服务进行交互。 这样便可以编程以用户任务而不是设备为中心的跨设备和跨平台体验。
ms.localizationpriority: medium
author: ailae
ms.prod: project-rome
doc_type: conceptualPageType
ms.openlocfilehash: 30e0c2049a5c4ef0b9aea79ebe2d420f5a341c87
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034458"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft 图形 API与Project罗马合作

[Project罗马](https://developer.microsoft.com/en-us/windows/project-rome)是一项 Microsoft 计划，旨在构建跨设备体验平台。 Project罗马允许本地客户端或服务上的应用在用户使用用于在客户端设备上登录的同一 Microsoft 帐户登录时与远程主机上的应用和服务进行交互。 这样便可以编程以用户任务而不是设备为中心的跨设备和跨平台体验。

通过 Microsoft Graph 公开关键组件，以启用以下体验：活动。

## <a name="activities"></a>活动

Microsoft Graph中的活动使你能够跨设备和平台推动用户与应用的互动。 活动是用户参与的单元，由三个组件组成：

- 深层链接
- 视觉表示形式
- 使用 [https://schema.org/](https://schema.org/) 共享词汇描述活动的内容元数据

当应用程序创建会话时，会向活动添加历史记录项，以反映用户参与的时间段。 每次用户重新参与活动时，都会向活动添加一个新的历史记录项来累积用户参与。

当应用程序发布用户活动对象时，该对象将显示在Windows中的一些新 UI 图面中;例如，Cortana通知和时间线。 可以指定丰富元数据 (，以便在活动对象中使用 [自适应卡](https://adaptivecards.io/) 片标记)  (在正确的上下文) 和丰富的视觉对象中显示活动。

可以使用以下 Microsoft Graph API 创建和检索用户活动：

- [创建或替换活动](../api/projectrome-put-activity.md)
- [获取活动](../api/projectrome-get-activities.md)
- [获取最近的活动](../api/projectrome-get-recent-activities.md)
- [删除活动](../api/projectrome-delete-activity.md)
- [创建或替换历史记录项](../api/projectrome-put-historyitem.md)
- [删除历史记录项](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
