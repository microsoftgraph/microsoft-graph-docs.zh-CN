---
title: 使用活动源Microsoft Teams的最佳实践
description: 本文提供了在 Microsoft Graph 中处理活动源通知的最佳实践和Graph。
author: KirtiPereira
localization_priority: Normal
ms.prod: teamwork
ms.openlocfilehash: cfb62de20bfa74ccc91ce99189cf5be5a9dc1787
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060622"
---
# <a name="best-practices-for-using-microsoft-teams-activity-feed-notifications"></a>使用活动源Microsoft Teams的最佳实践

本文介绍了在 Microsoft Microsoft Teams 中使用活动源Graph。 这些最佳做法适用于：
* 创建行动号召通知
* 请求通知响应
* 创建有关外部事件的通知

下图显示了活动源通知在Teams。

![显示活动Teams视图的桌面应用屏幕截图。](./images/activity-feed-notification.png)

实现活动源通知时，请记住以下几点：
* Toast 通知将用户重定向到活动源，而不是应用。 若要查看其他活动，用户必须在活动源中选择关联的通知。
* 只有在选定应用发送通知后，用户才能管理通知设置。
* 每个通知的图标都包含在应用清单中。 Microsoft Graph不支持自定义图标。
* 不支持优先级通知。

## <a name="enhance-the-notification-experience"></a>增强通知体验

Microsoft Teams以活动源和 Toast 格式显示通知。 用户通过聊天、频道、会议或其他应用接收来自多个源的通知。 若要增强用户体验，请应用以下建议：

* 本地化通知 toast 或源中的内容。 本地化仅在应用内容本地化 [时发生](/platform/concepts/build-and-test/apps-localization)。
* 为活动类型提供适当的标题 **和说明**。 使用短标题，如 **@mention****和通知**。 避免使用长标题，例如"提到 **的用户"活动和** " **创建后"活动**。
* 通知应传达与用户相关的重要信息。 例如 *，在 一个销售票证分配给你* 时，是一条相关消息; *Joni 未离开* 销售团队。
* 避免发送本质上是促销性的通知，例如尝试循环 *应用中的新功能*。
* 避免来自自动程序消息和活动源通知的重复通知。 有关详细信息，请参阅活动 [源通知或自动程序框架消息](#activity-feed-notifications-or-bot-framework-messages)。
* 使用 **通知中的** 文本预览部分。 提供可帮助用户确定通知重要性的信息，并在必要时采取措施。
* 请勿在通知标题末尾添加一个时间段，以与通知标题中的所有其他通知设置Teams。
* 让用户清楚通知及其内容之间的关系。 例如，当用户收到批准请假的通知时，通知应将其重定向到应用的相应部分。 如果通知与删除实体（如用户和任务）相关，请引导收件人访问内容并指示所需操作。
* 确保源体验是自包含的。 例如，任何弹出窗口和模式必须保留在应用中。
* 验证你的应用每分钟每个用户发送的通知数是否不超过 10 个。 如果计数超过 10，将自动限制通知。
* 确保应用的加载时间不会对用户在源中的通知之间切换时的体验产生负面影响。
* 通知用户活动源中的通知存储周期。 在Microsoft Teams中，存储期限为 30 天。
    > [!NOTE]
    > 30 天存储限制适用于所有通知。 它并不特定于通过活动源通知 API 发送的通知。

## <a name="activity-feed-notifications-or-bot-framework-messages"></a>活动源通知或自动程序框架消息

可以使用活动源通知或自动程序框架消息，但请勿同时使用这两种通知类型。 以下各节介绍通知类型以及何时使用每一种通知类型。 

### <a name="activity-feed-notifications"></a>活动源通知

活动源通知显示在活动Teams中，并可以包含指向不同位置的链接。 这些通知： 
* 允许用户采取措施或对通知进行会审。
* 将用户引导到聊天或频道、个人应用、聊天或频道消息中的选项卡。 

活动源通知 API 允许用户根据通知设置为每个 **通知类型** 配置通知。

如果使用活动源通知，请注意，如果应用向聊天或频道以及活动源发送自动程序通知，则应用可能会发送双重通知。 仅在方案需要时发送双重通知。 

使用委派通知创建更好的通知体验。 活动源通知 API 可以发送委托调用或仅应用程序调用。 在委派呼叫中，通知的发件人显示为启动通知的用户，在仅应用程序呼叫中，发件人显示为应用程序。 

可以更新现有活动源通知，而不是使用 *chainId* 参数创建新的通知。

### <a name="bot-framework-messages"></a>自动程序框架消息

自动程序消息作为聊天或频道消息传递。 如果用户打开聊天或频道通知，则触发的通知将作为聊天或频道消息发送。 若要发送自动@mention，请指定通知显示在活动源中的用户名称。

将警报用作聊天或频道消息非常有用;例如，所有频道成员使用的消息。
