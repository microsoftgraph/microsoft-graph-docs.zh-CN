---
title: 将 Azure Active Directory (Azure AD) Graph 迁移到 Microsoft Graph
description: 了解如何在 Azure AD Graph 停用之前将 Azure AD (Azure AD) Graph 应用迁移到 Microsoft Graph。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 12e080c58217a159d011a14a854f1bab3456f5fc
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577754"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>将 Azure AD Graph 应用迁移到 Microsoft Graph

> [!IMPORTANT]
> Azure Active Directory (Azure AD) Graph 已弃用，但不会像 [之前宣布](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363)的那样在 2022 年 6 月 30 日停用。 仔细听取你关于迁移如此关键的依赖项的挑战的反馈，我们将至少将退休日期推迟到今年年底，即 2022 年。 我们将在日历年中提供停用更新，包括发布更多工具来帮助你迁移应用。

## <a name="why-use-microsoft-graph"></a>为什么要使用 Microsoft Graph？

Microsoft Graph 表示我们最适合的 API 图面。 它提供单个统一终结点来访问 Azure AD 服务和 Microsoft 365 服务，如 Microsoft Teams 和 Microsoft Intune。 Microsoft 图形 API的使用量是 Azure AD Graph 的两倍多，在过去两年中，我们新增了 [167 项功能](https://developer.microsoft.com/en-us/graph/changelog)。 所有新功能只能通过 Microsoft Graph 使用。

Microsoft Graph 也比 Azure AD Graph 更安全且更具弹性。

Microsoft Graph 具有 Azure AD Graph 中提供的所有功能，以及标识保护和身份验证方法等新 API。 其客户端库为重试处理、安全重定向、透明身份验证和有效负载压缩等功能提供内置支持。

切换到 Microsoft Graph 以利用这些增强的功能，

- [Microsoft 365 组管理](/graph/office365-groups-concept-overview)。
- [外部用户邀请](/graph/api/resources/invitation)。
- 在 [删除用户、Microsoft 365 组、应用程序和服务主体](/graph/api/resources/directory) 后还原用户的功能。
- [用户和组上的 Webhook 通知](/graph/webhooks)。
- 高级许可证管理功能，包括 [基于组的许可](/graph/api/group-assignlicense)。
- 标识治理功能，例如：
  - [特权标识管理](/graph/api/resources/privilegedidentitymanagement-root) (PIM) 仅在需要时和有限的时间段内将用户提升为特权角色。
  - 针对一次性或定期访问评审的访问[评审](/graph/api/resources/accessreviewsv2-overview)，以证明用户的访问权限。
  - 使组织能够提供法律或合规性要求的信息（如免责声明通知）的[使用条款](/graph/api/resources/agreement)。
- 安全功能，例如：
  - [标识风险事件](/graph/api/resources/riskdetection)。
  - [有风险的用户](/graph/api/resources/riskyuser)。
- [客户端库和示例](/graph/) 可在更多平台和语言上使用。 Microsoft Graph SDK 提供了一个可发现的接口，可轻松访问数据，同时透明地处理令牌获取、由于错误和限制而重试处理、安全重定向处理以及模型序列化和反序列化。
- 用户、组、应用程序和服务主体等资源支持的更多 [OData 查询功能](/graph/query-parameters) 。

本部分的其余文章可帮助你将应用从 Azure AD Graph 迁移到 Microsoft Graph。 你会发现：

- 帮助你规划迁移的清单。
- 描述 API 之间的特定差异的指南。
- 指向更多资源和示例的链接，以说明具体的差异。
- 用于解决其他问题或问题的常见问题解答。

使用标记 [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html) 通过 Microsoft Q&A 发送任何其他问题、打开问题和功能请求。

## <a name="next-steps"></a>后续步骤

- 浏览 [应用迁移清单](migrate-azure-ad-graph-planning-checklist.md) ，帮助你规划迁移。
- 探索 [Microsoft Graph](/graph/overview) 概念和做法。
- 使用 [Graph 资源管理器](https://aka.ms/ge) 试验 Microsoft Graph。
- 详细了解 [Microsoft Graph 或 Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/) 中的进度更新和时间线。
- 获取有关迁移 [的问题的解答](/graph/migrate-azure-ad-graph-faq) 。