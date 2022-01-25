---
title: '使用 Microsoft Graph API 处理 Project Rome '
description: 'Project Rome 是 Microsoft 的一项计划，旨在构建一个平台，使应用开发人员能够构建出色的跨设备体验。 Project在用户使用同一 Microsoft 帐户或工作或学校帐户登录时，Rome 将启用连接不同服务和客户端终结点的不同功能。 这允许你实现以用户任务而不是设备为中心的跨设备和跨平台体验。 '
ms.localizationpriority: medium
doc_type: conceptualPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: 1ac28fb48ef7b954bd51519124e628fbb9029bab
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201433"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 处理 Project Rome

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome)是 Microsoft 的一项计划，旨在构建一个平台，使应用开发人员能够构建出色的跨设备体验。 Project在用户使用同一 Microsoft 帐户或工作或学校帐户登录时，Rome 将启用连接不同服务和客户端终结点的不同功能。 这允许你实现以用户任务而不是设备为中心的跨设备和跨平台体验。

通过 Microsoft Project公开了三个关键的 Rome 功能Graph可帮助你实现出色的跨设备体验：活动、设备和通知。

## <a name="activities"></a>活动

通过 Microsoft Graph，你可以跨设备和平台推动用户与应用互动。 活动是用户参与度的单位，由三个部分组成：

- 深层链接
- 视觉表示形式
- 使用共享词汇描述活动 [https://schema.org/](https://schema.org/) 的内容元数据

当应用程序创建会话时，会向活动添加历史记录项以反映用户参与的时间段。 每次用户重新参与某个活动时，会向活动添加一个新的历史记录项，以增加用户参与度。

当应用程序发布用户活动对象时，该对象将在 Windows 中的某些新 UI 图面中显示;例如，Cortana通知和时间线。 你可以指定丰富的元数据 (以允许活动在正确的上下文) 中显示，也可以指定富 (在活动对象) 卡片标记。 [](https://adaptivecards.io/)

可以使用以下 Microsoft Graph API 创建和检索用户活动：

- [创建或替换活动](../api/projectrome-put-activity.md)
- [获取活动](../api/projectrome-get-activities.md)
- [获取最近的活动](../api/projectrome-get-recent-activities.md)
- [删除活动](../api/projectrome-delete-activity.md)
- [创建或替换历史记录项](../api/projectrome-put-historyitem.md)
- [删除历史记录项](../api/projectrome-delete-historyitem.md)

## <a name="devices-deprecated"></a>已 (的设备) 

可以使用 Microsoft Project Rome API 进行Graph：

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

