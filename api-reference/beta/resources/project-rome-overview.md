---
title: '使用 Microsoft Graph API 处理 Project 罗马 '
description: '项目罗马是 Microsoft 计划，用于构建一个平台，使应用程序开发人员能够生成强大的跨设备体验。 Project 罗马启用不同的功能，以便在用户使用相同的 Microsoft 帐户或工作或学校帐户登录时连接不同的服务和客户端终结点。 这使您能够实现以用户任务（而不是设备）为中心的跨设备和跨平台体验。 '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: f9d9900aecb7226ed33c5e0cf51c7ccfaf3d2e8d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809319"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 处理 Project 罗马

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[项目罗马](https://developer.microsoft.com/en-us/windows/project-rome) 是 Microsoft 计划，用于构建一个平台，使应用程序开发人员能够生成强大的跨设备体验。 Project 罗马启用不同的功能，以便在用户使用相同的 Microsoft 帐户或工作或学校帐户登录时连接不同的服务和客户端终结点。 这使您能够实现以用户任务（而不是设备）为中心的跨设备和跨平台体验。

通过 Microsoft Graph 公开三个关键项目罗马功能，可帮助您实现大量的跨设备体验：活动、设备和通知。

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

## <a name="devices"></a>设备

您可以使用 Microsoft Graph 中的 Project 罗马 Api 执行以下操作：

- 发现并连接到用户的设备
- 在这些设备上远程启动应用程序
- 将邮件发送到这些设备上的应用程序

使用这些 Api，您可以生成可在一个设备上创建丰富体验的应用程序。 例如，您可以扩展您的应用程序，使其在更大的屏幕上启动。 或者，您可以为用户设备上的另一个应用创建配套体验。

您可以使用以下 Microsoft Graph Api 与其他 Windows 设备进行通信：

- [列出用户的设备](../api/user-list-devices.md)
- [向设备发送命令](../api/send-device-command.md)
- [获取命令状态](../api/get-device-command-status.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。