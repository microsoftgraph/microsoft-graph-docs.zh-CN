---
title: '使用 Microsoft Graph API 来处理项目 Rome '
description: '项目 Rome 是 Microsoft 旨在构建一个平台，使应用程序开发人员可以构建出色的跨设备体验。 项目 Rome 启用连接不同的服务和客户端终结点，当用户迹象使用同一 Microsoft 帐户或工作或学校帐户时的不同功能。 这样，您可以实现跨设备和跨平台围绕用户任务，而不是设备的体验。 '
ms.openlocfilehash: f779c04a76331d27fdcae6436e758bacfc052f8e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043778"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 来处理项目 Rome 

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[项目 Rome](https://developer.microsoft.com/en-us/windows/project-rome)是 Microsoft 旨在构建一个平台，使应用程序开发人员可以构建出色的跨设备体验。 项目 Rome 启用连接不同的服务和客户端终结点，当用户迹象使用同一 Microsoft 帐户或工作或学校帐户时的不同功能。 这样，您可以实现跨设备和跨平台围绕用户任务，而不是设备的体验。 

三个主要项目 Rome 功能公开通过 Microsoft Graph 可帮助您启用绝佳跨设备体验： 活动、 设备和通知。 

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

## <a name="devices"></a>设备

您可以在 Microsoft Graph 中使用项目 Rome Api:

- 发现并连接到用户的设备
- 远程启动这些设备上的应用程序
- 将邮件发送到您在这些设备上的应用程序

使用这些 Api，您可以生成创建跨越单个设备的丰富体验的应用程序。 例如，您可以扩展您的应用程序，以更大的屏幕上启动。 也可以在另一个用户的设备上创建应用程序的辅助体验。

以下 Microsoft Graph Api 可用于与其他 Windows 设备进行通信：

- [列出用户的设备](../api/user-list-devices.md)
- [向设备发送命令](../api/send-device-command.md)
- [获取 status 命令](../api/get-device-command-status.md)

## <a name="notifications"></a>Notifications

您可以使用在 Microsoft Graph 通知 Api 个相同的用户登录的多个终结点发送通知。 发布而不是担心设备地址/通道通知时，您可以直接目标用户。 这种方式，您可以集中设计 human 为中心，而不是一种设备中心的方法中的右侧的通知方案。 

您可以发布原始数据通知或直接 visual 通知。 原始数据通知传递到设备的终结点，可以使用[客户端 SDK](https://github.com/Microsoft/project-rome) （Microsoft Graph 通知 SDK for Windows，适用于 iOS 的项目 Rome SDK 和 Android） 接收和管理通知。 直接的可视通知传递到设备的终结点，它向用户显示特定于平台的本机通知。 

有关详细信息，请参阅[创建和发送通知](../api/projectrome-notification-post.md)。

