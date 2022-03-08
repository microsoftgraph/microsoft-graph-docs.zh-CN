---
title: 将Azure AD Graph应用迁移到 Microsoft Graph
description: 介绍如何将 Azure Active Directory (Azure AD) API 应用迁移到 Microsoft Graph API。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a59b32d7c042d7a6300abb97dc602700a769d3cf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333839"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>将Azure AD Graph应用迁移到 Microsoft Graph

> [!IMPORTANT]
> Azure Active Directory (Azure AD) Graph已弃用，但将不会在 2022 年 6 月 30 日停用，正如[之前所宣布的](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363)。 我们至少将停用日期延迟到 2022 年末尾，认真听取你有关迁移此类关键依赖项的挑战的反馈。 我们将在日历年中提供停用更新，包括发布更多工具来帮助你迁移应用。

## <a name="why-use-microsoft-graph"></a>为什么使用 Microsoft Graph？

Microsoft Graph表示我们的最佳应用 API 图面。 它提供了一个统一终结点，Azure AD服务Microsoft 365服务，如 Microsoft Teams 和 Microsoft Intune。 Microsoft Graph API 的使用量超过 Azure AD Graph 的两倍，在过去两年，我们添加了 [167 项新功能](https://developer.microsoft.com/en-us/graph/changelog)。 所有新功能将仅通过 Microsoft Graph。

Microsoft Graph还比 microsoft Azure AD Graph 更安全、更具弹性。

Microsoft Graph 具有所有可用于新 API Azure AD Graph如标识保护和身份验证方法的功能。 其客户端库为重试处理、安全重定向、透明身份验证和负载压缩等功能提供内置支持。

切换到 Microsoft Graph以利用这些增强功能，并：

- [Microsoft 365组管理](/graph/office365-groups-concept-overview)。
- [外部用户邀请](/graph/api/resources/invitation)。
- 删除用户[、Microsoft 365组、应用程序和服务主体后](/graph/api/resources/directory)还原它们的能力。
- [有关用户和组的 Webhook 通知](/graph/webhooks)。
- 高级许可证管理功能， [包括基于组的许可](/graph/api/group-assignlicense)。
- 标识管理功能，例如：
  - [PRIVILEGEd identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) (PIM) to elevate users to privileged roles only when needed and for a limited time.
  - [有关用户](/graph/api/resources/accessreviewsv2-overview) 访问权限证明的一次性或定期访问评审的访问评审。
  - [使组织能够提供](/graph/api/resources/agreement) 法律或合规性要求信息（如免责声明通知）的使用条款。
- 安全功能，例如：
  - [标识风险事件](/graph/api/resources/riskdetection)。
  - [有风险的用户](/graph/api/resources/riskyuser)。
- [更多平台和语言](/graph/) 中提供了客户端库和示例。 Microsoft Graph SDK 提供了一个可发现接口，可轻松访问你的数据，同时以透明方式处理令牌获取、由于错误和限制而重试处理、安全重定向处理以及模型序列化和反序列化。
- 资源 [（如](/graph/query-parameters) 用户、组、应用程序和服务主体）支持的更多 OData 查询功能。

本部分中的其余文章可帮助你将应用从 Azure AD Graph 迁移到 Microsoft Graph。 你将找到：

- 帮助您规划迁移的清单。
- 描述 API 之间特定差异的指南。
- 指向更多资源和示例的链接，用于说明特定差异。
- 用于解决其他问题或顾虑的常见问题解答。

使用标记 [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html)，通过 Microsoft Q&A 发送任何其他问题、打开问题和功能请求。

## <a name="next-steps"></a>后续步骤

- 演练应用 [迁移清单](migrate-azure-ad-graph-planning-checklist.md) ，帮助你规划迁移。
- 了解 [Microsoft Graph](/graph/overview)概念和做法。
- 使用[Graph资源管理器](https://aka.ms/ge)尝试 Microsoft Graph。
- 若要详细了解进度更新和日程表，请参阅 [Microsoft Graph 或 Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)。
- 获取 [你可能对迁移](/graph/migrate-azure-ad-graph-faq) 问题的解答。