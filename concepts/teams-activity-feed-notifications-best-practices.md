---
title: 使用 Microsoft Teams 活动源通知的最佳做法
description: 获取有关在 Microsoft Graph 中增强 Microsoft Teams 活动源通知体验的提示，并了解何时选择通知或机器人框架消息。
author: KirtiPereira
ms.localizationpriority: medium
ms.prod: teamwork
ms.openlocfilehash: 37dd5cda8200aeeac0e810ae7a86408f3db876b3
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555869"
---
# <a name="best-practices-for-using-microsoft-teams-activity-feed-notifications"></a>使用 Microsoft Teams 活动源通知的最佳做法

本文介绍在 Microsoft Graph 中使用 Microsoft Teams 活动源通知的最佳做法。 这些最佳做法适用于：
* 创建操作呼叫通知
* 请求对通知的响应
* 创建有关外部事件的通知

下图显示了 Teams 中活动源通知的示例：

![Teams 应用的屏幕截图，其中显示了活动源通知视图。](./images/activity-feed-notification.png)

实现活动源通知时，请记住以下几点：
* Toast 通知将用户重定向到活动源，而不是应用。 若要查看其他活动，用户必须在活动源中选择关联的通知。
* 用户只能在所选应用发送通知后管理通知设置。
* 每个通知的图标都包含在应用清单中。 Microsoft Graph 不支持自定义图标。
* 不支持优先级通知。

## <a name="enhance-the-notification-experience"></a>增强通知体验

Microsoft Teams 以活动源和 Toast 格式显示通知。 用户通过聊天、频道、会议或其他应用从多个源接收通知。 若要增强用户体验，请应用以下建议：

* 本地化通知 Toast 或源中的内容。 仅当应用的内容已 [本地化](/microsoftteams/platform/concepts/build-and-test/apps-localization)时，才会发生本地化。
* 为 **活动类型** 提供适当的标题和说明。 使用短标题，例如 **@mention** 和 **公告**。 避免使用长标题，例如 **用户提及的活动** 和 **发布创建活动**。
* 通知应传达与用户相关的重要信息。 例如， *Diego 为您分配了一张销售票* 证是一条相关消息; *乔尼离开销售团队* 不是。
* 避免发送具有促销性质的通知，例如 *在循环应用中试用新功能*。
* 避免来自机器人消息和活动源通知的重复通知。 有关详细信息，请参阅 [选择活动源通知或机器人框架消息](#choose-activity-feed-notifications-or-bot-framework-messages)。
* 在通知中使用 **文本预览** 部分。 提供信息，帮助用户确定通知的重要性，并在必要时采取措施。
* 请勿在通知标题末尾添加一个句点，以便与 Teams 中的所有其他通知设置保持一致。
* 向用户明确通知与其内容之间的关系。 例如，当用户收到批准休假的通知时，通知应将其重定向到应用的相应部分。 如果通知与删除或删除实体（如用户和任务）有关，请将收件人定向到内容并指示所需的操作。
* 确保源体验是自包含的。 例如，任何弹出窗口和模式都必须保留在应用中。
* 验证每个用户的应用每分钟发送的通知数不超过 10 条。 如果计数超过 10，将自动限制通知。
* 确保应用的加载时间不会对用户在源中的通知之间切换时体验产生负面影响。
* 告知用户活动源中的通知存储期。 在 Microsoft Teams 中，存储期为 30 天。
    > [!NOTE]
    > 30 天的存储限制适用于所有通知。 它不特定于通过活动源通知 API 发送的通知。

## <a name="choose-activity-feed-notifications-or-bot-framework-messages"></a>选择活动源通知或机器人框架消息

可以使用活动源通知或机器人框架消息，但不使用这两种通知类型。 以下各节介绍通知类型以及何时使用每个通知类型。

### <a name="activity-feed-notifications"></a>活动源通知

活动源通知显示在 Teams 活动源中，并且可以包含指向不同位置的链接。 这些通知： 
* 允许用户执行操作或对通知进行会审。
* 将用户引导到聊天或频道、个人应用或聊天或频道消息中的选项卡。 

活动源通知 API 允许用户从通知设置为每个 **通知类型** 配置通知。

如果使用活动源通知，请注意，如果应用向聊天或频道以及活动源发送机器人通知，则应用可能会发送双重通知。 仅在方案需要时发送双重通知。 

使用委派通知创建更好的通知体验。 活动源通知 API 可以发送委托的或仅限应用程序的调用。 在委托的调用中，通知的发件人显示为发起通知的用户，在仅限应用程序的调用中，发件人将显示为应用。 

可以更新现有活动源通知，而不是使用 *chainId* 参数创建新通知。

### <a name="bot-framework-messages"></a>机器人框架消息

机器人消息作为聊天或频道消息传递。 如果用户打开聊天或频道通知，则触发的通知将作为聊天或频道消息发送。 若要发送机器人消息， *@mention* 要在活动源中显示通知的用户的名称。

将警报用作聊天或频道消息非常有用;例如，所有通道成员使用的消息。

## <a name="see-also"></a>另请参阅

- [为 Microsoft Teams 设计活动源通知](/microsoftteams/platform/concepts/design/activity-feed-notifications?tabs=mobile)
- [Microsoft Teams API 概述](teams-concept-overview.md)