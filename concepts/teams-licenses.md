---
title: 许可和付款要求
description: 了解适用于 Microsoft Graph 中的 Microsoft Teams API 的许可和付款模式。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: ca09c2fbfe2256f7858e12ed3ac3566025bfca2a
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545313"
---
# <a name="licensing-and-payment-requirements-for-microsoft-teams-apis-in-microsoft-graph"></a>Microsoft Graph 中 Microsoft Teams API 的许可和付款要求

本文介绍了 Microsoft Teams API 的许可和付款要求。

某些 API 提供通过 `model` 查询参数选择许可和付款模型的选项；其他 API 仅支持某一个模型或不支持许可和付款模型。以下许可模型可用：

- [`model=A`](#modela-requirements) 限于执行[安全或合规性功能](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms)或需要[受支持的许可证](#required-licenses-for-modela)的应用程序。
将来，应用还需要为其在[种子设定容量](#seeded-capacity)之外使用的消息付费。

- [`model=B`](#modelb-requirements) 现在可以免费使用，但是，在将来，应用将根据它们使用的消息数向你收费。 `model=B` 没有许可要求，并且不限于执行安全性或合规性功能的应用程序。

- [评估模式（默认）](#evaluation-mode-default-requirements)可以访问 API 进行评估，每个请求应用程序的使用量有限。 如果超出限制，则不会发送更改通知。

## <a name="modela-requirements"></a>`model=A` 要求

`model=A` 限于执行安全性或符合性功能的应用程序。 有关详细信息，请参阅 [Microsoft Azure Services 产品条款](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms)的安全与合规性应用程序部分的 API 条款。

|API                   | 需要[许可证](#required-licenses-for-modela)的人员  | 种子设定容量 | 其他用途的价格 | 备注 |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [chatMessage 更改通知](/graph/api/subscription-post-subscriptions) | 邮件发件人 | 每个应用每个月每个用户 800 条消息 | 每条消息 0.00075 美元 | 种子设定容量与 conversationMember 更改通知共享 |
| [conversationMember 更改通知](/graph/api/subscription-post-subscriptions) | 租户中的任何用户 | 每个应用每个月每个用户 800 条通知  | 每条通知 0.00075 美元 | 种子设定容量与 chatMessage 更改通知共享 |
| [为用户在所有聊天中获取消息](/graph/api/chats-getallmessages) | 已命名用户 | 每个应用每个月每个用户 1600 条消息 | 每条消息 0.00075 美元 | 命名用户是在 GET 请求 URL 中标识的用户。 每个 API 请求的最小费用为 1 条消息。 种子设定容量与通道导出共享。 |
|  [在所有通道中获取消息](/graph/api/channel-getallmessages)| 任何团队成员 | 每个应用每个月每个用户 1600 条消息 | 每条消息 0.00075 美元 |  每个 API 请求的最小费用为 1 条消息。 种子设定容量与聊天导出共享。 |
| [正在更新 chatMessage 的 policyViolation](/graph/api/chatmessage-update) |  邮件发件人 |  每个应用每个月每个用户 800 条消息 | 每条消息 0.00075 美元 |

## <a name="modelb-requirements"></a>`model=B` 要求

>**注意：** [ `model=B`](#modelb-requirements) 现在可以免费使用，但将来应用将根据其使用的消息数收费。 

|API                   | 需要[许可证](#required-licenses-for-modela)的人员  | 种子设定容量 | 其他用途的价格 | 备注 |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [chatMessage 更改通知](/graph/api/subscription-post-subscriptions) | 不适用 | 无 | 每条消息 0.00075 美元 |  |
| [conversationMember 更改通知](/graph/api/subscription-post-subscriptions) | 不适用 | 无  | 每条通知 0.00075 美元 | |
| [为用户在所有聊天中获取消息](/graph/api/chats-getallmessages) |  不适用 | 无 | 每条消息 0.00075 美元 |  每个 API 请求的最小费用为 1 条消息。 |
|  [在所有通道中获取消息](/graph/api/channel-getallmessages)|  不适用 | 无 | 每条消息 0.00075 美元 | 每个 API 请求的最小费用为 1 条消息。 |

## <a name="evaluation-mode-default-requirements"></a>评估模式（默认）要求

|API                   | 需要[许可证](#required-licenses-for-modela)的人员  | 种子设定容量 | 其他用途的价格 | 备注 |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [chatMessage 更改通知](/graph/api/subscription-post-subscriptions) |  不适用 | 每个应用每月 500 条消息 | 不适用 |
| [conversationMember 更改通知](/graph/api/subscription-post-subscriptions) | 不适用 | 每个应用每月 500 条消息 | 不适用 | 
| [为用户在所有聊天中获取消息](/graph/api/chats-getallmessages) |  不适用 | 每个应用每月 500 条消息 | 不适用 |  每个 API 请求的最小费用为 1 条消息。 |
|  [在所有通道中获取消息](/graph/api/channel-getallmessages)|  不适用 | 每个应用每月 500 条消息 | 不适用 |  每个 API 请求的最小费用为 1 条消息。 |
| [正在更新 chatMessage 的 policyViolation](/graph/api/chatmessage-update) |   不适用 |  每个应用每月 500 条消息 | 不适用 |

在评估模式下，种子设定容量在所有 API 之间共享。超出种子设定容量后，具有许可和付款要求的 API 调用将失败，并出现 402 错误代码，另外，具有许可和付款要求的订阅将不会发送更改通知。

> **注意**：成功的 API 调用并不意味着正确的许可已经就位。 
> 并非所有许可证冲突都可检测到，在某些情况下可能会授予宽限期。

## <a name="required-licenses-for-modela"></a>`model=A` 需要的许可证 

用户需要[支持许可证](https://aka.ms/teams-api-license-list)之一。 需要许可证的用户因 API 而异；有关详细信息，请参阅[`model=A`要求](#modela-requirements)。

来宾用户不受这些许可要求的约束。
同样地，从租户外部发送的消息（联合聊天）不受约束。
消耗计量仍适用。

租户所有者（而不是应用所有者）负责确保用户获得正确许可。
管理员可以使用 [Teams 管理中心](https://admin.teams.microsoft.com/analytics/reports)中的信息保护许可证报告来查看哪些用户没有受支持的许可证。

许多受支持的许可证提供免费试用版。 
例如，[Office 365 E5](https://www.microsoft.com/microsoft-365/enterprise/office-365-e5?activetab=pivot%3aoverviewtab) 在 `Buy` 按钮下方有一个 `Free trial` 链接。

你可以通过 [Microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)获取包含 25 个用户许可证的免费 Microsoft 365 E5 开发人员沙盒订阅。

## <a name="improper-licensing-and-evaluation-mode-seeded-capacity-exceeded"></a>超出了不正确的许可和评估模式种子设定容量

如果检测到不正确的许可，API 调用将失败，并且不会返回数据。
具体而言，对于大多数 API，尝试为未经授权的用户获取消息将导致 402 错误代码。 对于更改通知，未经授权的用户发送的消息将不会生成更改通知。 同样，在评估模式下使用的超出种子设定容量的 API 调用和更改通知将失败。

> **注意**：成功的 API 调用并不意味着正确的许可已经就位。 
> 并非所有许可证冲突都可检测到，在某些情况下可能会授予宽限期。
> 同样，评估模式下的 API 成功并不能保证调用在种子设定容量内，因为在某些情况下可能会授予宽限期。

## <a name="seeded-capacity"></a>种子设定容量

种子设定容量是应用在对消耗量计费之前可以使用的容量。
容量在租户级别共用 - 租户中所有用户的种子设定容量会加在一起与租户中的应用使用情况对比。
种子设定容量按每个租户的每个应用计 - 如果一个应用消耗完了种子设定容量，其他应用的种子设定容量不会耗尽。

种子设定容量因 API 而异，具体请参阅[`model=A`要求](#modela-requirements)和[`model=B`要求](#modelb-requirements)

## <a name="price-for-additional-use"></a>其他用途的价格

将来，Microsoft 会对种子设定容量之外的使用量收取费用。 你还可以将 Azure 订阅关联到应用程序注册。
