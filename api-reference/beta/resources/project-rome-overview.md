---
title: '使用 Microsoft Graph API 处理 Project Rome '
description: 'Project Rome 是 Microsoft 的一项计划，旨在构建一个平台，使应用开发人员能够构建出色的跨设备体验。 Project在用户使用同一 Microsoft 帐户或工作或学校帐户登录时，Rome 将启用连接不同服务和客户端终结点的不同功能。 这允许你实现以用户任务而不是设备为中心的跨设备和跨平台体验。 '
ms.localizationpriority: medium
doc_type: conceptualPageType
author: ailae
ms.prod: project-rome
ms.openlocfilehash: d8dafd71d02a49080b9070254415b3b59d2ffd8a
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291427"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 处理 Project Rome

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Project Rome](https://developer.microsoft.com/windows/project-rome) 是 Microsoft 的一项计划，旨在构建一个平台，使应用开发人员能够构建出色的跨设备体验。 Project在用户使用同一 Microsoft 帐户或工作或学校帐户登录时，Rome 将启用连接不同服务和客户端终结点的不同功能。 这允许你实现以用户任务而不是设备为中心的跨设备和跨平台体验。

通过 Microsoft Project公开了三个关键的 Rome 功能Graph可帮助你实现出色的跨设备体验：活动、设备和通知。

## <a name="activities"></a>活动

通过 Microsoft Graph，你可以推动用户跨设备和平台参与你的应用。 活动是用户参与度的单位，由三个部分组成：

- 深层链接
- 视觉表示形式
- 使用共享词汇描述活动 [https://schema.org/](https://schema.org/) 的内容元数据

当应用程序创建会话时，会向活动添加历史记录项以反映用户参与的时间段。 每次用户重新参与某个活动时，会向活动添加一个新的历史记录项，以增加用户参与度。

当应用程序发布用户活动对象时，该对象将在 Windows 中的某些新 UI 图面中显示;例如，Cortana通知和时间线。 你可以指定丰富的元数据 (以允许活动在正确的上下文) 中显示，也可以指定使用 (对象中的自适应卡片标记) 丰富的视觉效果。[](https://adaptivecards.io/)

可以使用以下 Microsoft Graph API 创建和检索用户活动：

- [创建或替换活动](../api/projectrome-put-activity.md)
- [获取活动](../api/projectrome-get-activities.md)
- [获取最近的活动](../api/projectrome-get-recent-activities.md)
- [删除活动](../api/projectrome-delete-activity.md)
- [创建或替换历史记录项](../api/projectrome-put-historyitem.md)
- [删除历史记录项](../api/projectrome-delete-historyitem.md)

## <a name="devices-deprecated"></a>已 (的设备) 

可以使用 Microsoft Project Rome API 来Graph：

- 发现并连接到用户设备
- 在这些设备上远程启动应用
- 向这些设备上的应用发送消息

借助这些 API，你可以构建能够创建超越单个设备的丰富体验的应用。 例如，你可以扩展应用以在较大的屏幕上启动。 或者，你可以为用户的另一台设备上的应用创建配套体验。

可以使用以下 Microsoft Graph API 与其他设备Windows通信：

- [列出用户设备](../api/user-list-devices.md)
- [向设备发送命令](../api/send-device-command.md)
- [获取命令状态](../api/get-device-command-status.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

