---
title: Microsoft Teams API 许可和付款要求
description: 了解适用于 microsoft Teams API 的许可和付款模型，Microsoft Graph：model=A、model=B 和评估模式。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 3216ecfa998cf6b2a02ec588992e8622a523038c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668158"
---
# <a name="licensing-and-payment-requirements-for-the-microsoft-teams-api"></a>Microsoft Teams API 的许可和付款要求

本文介绍 Microsoft Graph 中 Microsoft Teams API 的许可和付款要求。

某些 API 提供通过 `model` 查询参数选择许可和付款模型的选项；其他 API 仅支持某一个模型或不支持许可和付款模型。 以下 API 具有消耗费用：

* [导出 Teams 内容](/microsoftteams/export-teams-content)
* [创建订阅](/graph/api/subscription-post-subscriptions)
* [更新聊天消息](/graph/api/chatmessage-update)
* [获取频道消息](/graph/api/chatmessage-get)
* [获取聊天中的消息](/graph/api/chatmessage-get)

以下许可模型可用：

- [`model=A`](#modela-requirements) 限于执行[安全或合规性功能](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms)或需要[受支持的许可证](#required-licenses-for-modela)的应用程序。 将来，应用还需要为其在[种子设定容量](#seeded-capacity)之外使用的消息付费。

- [`model=B`](#modelb-requirements)仅限于不执行[安全或合规性功能](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms)的应用程序。
`model=B` 没有许可要求。

- [评估模式（默认）](#evaluation-mode-default-requirements) 允许访问每个请求应用程序的 API，但出于评估目的，其使用率有限。 如果超出限制，则不会发送更改通知。

> [!NOTE]
> 从 2022 年 7 月 5 日开始，这些 API 的定价事件正式发布。 我们需要应用程序完成此[表单](https://aka.ms/teamsgraph/protectedApis_az)以提供活动的 Azure 订阅，以便计费。 有关详细信息，请参阅[最近更新](#recent-updates-and-price-for-additional-use)。

## <a name="modela-requirements"></a>`model=A` 要求

`model=A` 限于执行安全性或符合性功能的应用程序。 有关详细信息，请参阅 [Microsoft Azure Services 产品条款](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms)的安全与合规性应用程序部分的 API 条款。

|API                   | 需要[许可证](#required-licenses-for-modela)的人员  | 种子设定容量 | [其他用途的价格](#recent-updates-and-price-for-additional-use) | 备注 |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [chatMessage 更改通知](/graph/api/subscription-post-subscriptions) | 邮件发件人 | 每个应用每个月每个用户 800 条消息 | 每条消息 0.00075 美元 | 种子设定容量与 conversationMember 更改通知共享 |
| [conversationMember 更改通知](/graph/api/subscription-post-subscriptions) | 租户中的任何用户 | 每个应用每个月每个用户 800 条通知  | 每条通知 0.00075 美元 | 种子设定容量与 chatMessage 更改通知共享 |
| [为用户在所有聊天中获取消息](/graph/api/chats-getallmessages) | 已命名用户 | 每个应用每个月每个用户 1600 条消息 | 每条消息 0.00075 美元 | 命名用户是在 GET 请求 URL 中标识的用户。 每个 API 请求的最小费用为 1 条消息。 种子设定容量与通道导出共享。 |
| [在所有通道中获取消息](/graph/api/channel-getallmessages)| 任何团队成员 | 每个应用每个月每个用户 1600 条消息 | 每条消息 0.00075 美元 |  每个 API 请求的最小费用为 1 条消息。 种子设定容量与聊天导出共享。 |
| [正在更新 chatMessage 的 policyViolation](/graph/api/chatmessage-update) |  邮件发件人 |  每个应用每个月每个用户 800 条消息 | 每条消息 0.00075 美元 |

## <a name="modelb-requirements"></a>`model=B` 要求

`model=B` 仅限于不执行安全或合规性功能的应用程序。 有关详细信息，请参阅 [Microsoft Azure Services 产品条款](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms)的安全与合规性应用程序部分的 API 条款。

|API                   | 需要[许可证](#required-licenses-for-modela)的人员  | 种子设定容量 | [其他用途的价格](#recent-updates-and-price-for-additional-use) | 备注 |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [chatMessage 更改通知](/graph/api/subscription-post-subscriptions) | 不适用 | 无 | 每条消息 0.00075 美元 |  |
| [conversationMember 更改通知](/graph/api/subscription-post-subscriptions) | 不适用 | 无  | 每条通知 0.00075 美元 | |
| [为用户在所有聊天中获取消息](/graph/api/chats-getallmessages) |  不适用 | 无 | 每条消息 0.00075 美元 |  每个 API 请求的最小费用为 1 条消息。 |
| [在所有通道中获取消息](/graph/api/channel-getallmessages)|  不适用 | 无 | 每条消息 0.00075 美元 | 每个 API 请求的最小费用为 1 条消息。 |

## <a name="evaluation-mode-default-requirements"></a>评估模式（默认）要求

|API   | 需要[许可证](#required-licenses-for-modela)的人员  | 种子设定容量 | [其他用途的价格](#recent-updates-and-price-for-additional-use) | 备注 |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [chatMessage 更改通知](/graph/api/subscription-post-subscriptions) |  不适用 | 每个应用每月 500 条消息 | 不适用 |
| [conversationMember 更改通知](/graph/api/subscription-post-subscriptions) | 不适用 | 每个应用每月 500 条消息 | 不适用 | 
| [为用户在所有聊天中获取消息](/graph/api/chats-getallmessages) |  不适用 | 每个应用每月 500 条消息 | 不适用 |  每个 API 请求的最小费用为 1 条消息。 |
| [在所有通道中获取消息](/graph/api/channel-getallmessages)|  不适用 | 每个应用每月 500 条消息 | 不适用 |  每个 API 请求的最小费用为 1 条消息。 |
| [正在更新 chatMessage 的 policyViolation](/graph/api/chatmessage-update) |   不适用 |  每个应用每月 500 条消息 | 不适用 |

在评估模式下，种子设定容量在所有 API 之间共享。超出种子设定容量后，具有许可和付款要求的 API 调用将失败，并出现 402 错误代码，另外，具有许可和付款要求的订阅将不会发送更改通知。

## <a name="required-licenses-for-modela"></a>`model=A` 需要的许可证 

用户将需要支持 Microsoft 通信 DLP [服务计划](/azure/active-directory/enterprise-users/licensing-service-plan-reference)的许可证，例如这些[受支持的许可证](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-graph-apis-for-teams-data-loss-prevention-dlp-and-for-teams-export)之一。
需要许可证的用户因 API 而异；有关详细信息，请参阅[`model=A`要求](#modela-requirements)。

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

| 示例错误类型 | 状态代码 | 示例错误消息 |
|:-----------|:-----------|:-----------------|
|未满足 E5 许可证要求| 402（需要付款） |`...needs a valid license to access this API...`, `...tenant needs a valid license to access this API...`|
|修补程序 API 不支持模型 B| 402（需要付款） |`...query parameter 'model' does not support value 'B' for this API. Use billing model 'A'...`|
|超出评估容量|402（需要付款）|`...evaluation mode capacity has been exceeded. Use a valid billing model...`|


> [!NOTE]
> 成功的 API 调用并不意味着已实施适当的许可。 同样，评估模式的 API 成功并不能保证调用在种子设定容量内。

## <a name="seeded-capacity"></a>种子设定容量

种子设定容量是应用在对消耗量计费之前可以使用的容量。 容量在租户级别共用&mdash;将租户中所有用户的种子设定容量相加，并与租户中的应用使用情况进行比较。 种子设定容量是每个租户的每个应用&mdash;如果另一个应用用完，应用不会耗尽种子容量。

种子设定的容量因 API 而异;请参 [阅`model=A` 要求](#modela-requirements) 和 [`model=B` 要求](#modelb-requirements)。

## <a name="recent-updates-and-price-for-additional-use"></a>用于其他用途的最近更新和价格

2021 年 10 月，我们就这些 API 的使用即将产生的费用进行了[通信](https://devblogs.microsoft.com/microsoft365dev/announcing-general-availability-of-microsoft-graph-export-api-for-microsoft-teams-messages/#license-requirements-for-microsoft-graph-api-for-teams-export-and-dlp)。如[先前公布](https://devblogs.microsoft.com/microsoft365dev/upcoming-billing-changes-for-microsoft-graph-apis-for-teams-messages/)的那样，这些价格将于 2022 年 7 月 5 日生效。 如果你的应用程序是或将调用这些 API 中的任何一个，我们要求你完成此[请求表单](https://aka.ms/teamsgraph/protectedApis_az)，提供有效的 Azure 订阅。 当提交此[表单](https://aka.ms/teamsgraph/protectedApis_az)以注册应用程序后，你可以继续使用这些 API。 我们将按照后续步骤将应用程序加入计费。 

请注意，拥有应用注册的组织负责付款，Azure 订阅也应在同一租户中处于活动状态。 对于多租户应用，组织可能不同于运行应用的组织。
