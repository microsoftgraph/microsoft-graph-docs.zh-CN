---
title: 将Azure AD Graph迁移到 Microsoft Graph
description: 介绍如何将 Azure Active Directory (Azure AD) API 应用迁移到 Microsoft Graph API。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 100fa23b9fdd7b82e201ed2fc6139f62ca93f74c
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651279"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>将Azure AD Graph迁移到 Microsoft Graph

> [!WARNING]
> **Azure Active Directory (Azure AD) Graph已弃用**。 为避免功能丢失，在 2022 年 6 月 30 Graph应用程序迁移到 Microsoft Azure AD Graph API 终结点将停止响应请求。
>
> 在 2022 年 6 月 30 Azure AD Graph，Microsoft 将继续提供技术支持，并应用安全修补程序。2022 年 6 月 30 日，所有功能和支持都将结束。 如果在 2022 年 6 月 30 Graph无法将应用程序迁移到 Microsoft Graph，则其功能和稳定性面临风险。

[Azure AD Graph弃用](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363)。 将你的Azure AD Graph应用更新为现在Graph Microsoft 应用。

## <a name="why-use-microsoft-graph"></a>为什么使用 Microsoft Graph？

Azure AD Graph仅提供对 Azure AD 服务的访问权限。 Microsoft Graph 提供了一个统一终结点，用于访问 Azure AD 服务和其他 Microsoft 365 服务，如 Microsoft Teams、Microsoft Exchange 和 Microsoft Intune。 对于大多数生产应用，Microsoft Graph完全支持Azure AD方案。

Microsoft Graph还比 Microsoft Azure AD Graph。

此外，Microsoft Graph 还支持许多在 Azure AD Graph 中不可用的新 Azure AD 数据集和功能，包括 Windows 10 和 企业移动性 + 安全性 (EMS) 。 切换到 Microsoft Graph以充分利用这些新 API，全部通过一个终结点，包括：

- [Microsoft 365组管理 。](/graph/office365-groups-concept-overview)
- [外部用户邀请](/graph/api/resources/invitation)。
- 删除用户[、Microsoft 365组](/graph/api/resources/directory)、应用程序和服务主体后还原它们的能力。
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

## <a name="next-steps"></a>后续步骤

- 演练应用 [迁移清单](migrate-azure-ad-graph-planning-checklist.md) ，帮助你规划迁移。
- 了解[Microsoft Graph](/graph/overview)概念和做法。
- 使用[Graph资源管理器](https://aka.ms/ge)尝试 Microsoft Graph。
- 若要详细了解进度更新和日程表，请参阅[Microsoft Graph 或 Azure AD Graph。](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)
- 获取 [你可能对迁移](/graph/migrate-azure-ad-graph-faq) 问题的解答。