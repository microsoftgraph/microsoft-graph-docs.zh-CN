---
title: 将 Azure AD Graph应用迁移到 Microsoft Graph
description: 介绍如何将 Azure AD Azure Active Directory (API) 迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 94a8eb93fc20fea677f6f221507eb2a046011d8e
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579802"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>将 Azure AD Graph应用迁移到 Microsoft Graph

Microsoft Graph完全替换Azure Active Directory (Azure AD) Graph。 对于大多数生产应用，Microsoft Graph可以完全支持 Azure AD 方案。 现在，你应该开始将 Azure AD Graph移动到 Microsoft Graph应用。

此外，Microsoft Graph 支持许多在 Azure AD Graph 中不可用的新 Azure AD 数据集和功能。 切换到 Microsoft Graph以充分利用这些新 API，全部通过一个终结点，包括：

- [Microsoft 365组管理](/graph/office365-groups-concept-overview)。
- [外部用户邀请](/graph/api/resources/invitation?view=graph-rest-1.0)。
- 删除[用户和Microsoft 365组](/graph/api/resources/directory?view=graph-rest-1.0)后还原用户和组的能力。
- [有关用户和组的 Webhook 通知](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)。
- 标识管理功能，例如：
  - [PRIVILEGEd identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) to elevate users to privileged roles only when needed and for a limited time.
  - [针对用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 访问权限证明的一次性或定期访问评审的访问评审。
  - [使组织能够提供](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 法律或合规性要求信息（如免责声明通知）的使用条款。
- 安全功能，例如：
  - [标识风险事件](/graph/api/resources/identityriskevent?view=graph-rest-beta)。
  - [有风险的用户](/graph/api/resources/riskyuser?view=graph-rest-beta)。
- [更多平台和语言](/graph/) 中提供了客户端库和示例。 Microsoft Graph SDK 提供了一个可发现接口，可轻松访问你的数据，同时以透明方式处理令牌获取、由于错误和限制而重试处理、安全重定向处理以及模型序列化和反序列化。

Microsoft Graph提供对更多服务的访问权限，而不只是 Azure Active Directory。 这也是提供[服务Microsoft 365 API 网关](/graph/)。

本部分中的其余文章可帮助你将应用从 Azure AD Graph Microsoft Graph。 你将找到：

- 帮助您进行规划的清单。
- 描述 API 之间特定差异的指南。
- 指向其他资源的链接和示例，用于说明特定差异。
- 用于解决其他问题或顾虑的常见问题解答


## <a name="frequently-asked-questions-faq"></a>常见问题 (FAQ)

### <a name="is-azure-ad-graph-aad-graph-deprecated"></a>Azure AD Graph (AAD Graph) 是否已弃用？  
是。 从 2020 年 6 月 30 日开始，我们将不再向 AAD Graph。 2022 年 6 月 30 日前，我们将继续添加关键安全修补程序。 2022 年 6 月 30 日之后，API 将不再正常工作。

### <a name="how-do-i-know-which-of-my-apps-are-using-aad-graph"></a>如何知道哪些应用程序正在使用 AAD Graph？  
必须注册应用程序，以使用 AAD Graph。  你可以查看 Azure 租户门户上的应用注册页面，以查看给定应用程序是否注册为使用 AAD Graph。

### <a name="how-do-i-know-which-apis-my-applications-are-calling"></a>如何知道应用程序正在调用哪些 API？
如果你有应用程序的源代码，可以参考本部分中的迁移指南，以帮助确定应用使用哪些 API 以及如何将其迁移到 Microsoft Graph。 如果无法访问应用程序的源代码，可以打开支持请求，获取每个应用程序调用的[](developer-support-help-options.md#open-a-support-request)API 列表。

### <a name="will-my-existing-aad-graph-apps-continue-to-work"></a>我现有的 AAD Graph应用会继续工作吗？ 
在 2022 年 6 月 30 日之前，现有应用将继续工作，无需修改。 AAD Graph API 函数和行为在此时间之后不保证。

### <a name="why-should-i-invest-in-moving-to-microsoft-graph"></a>为什么应投资迁移到 Microsoft Graph？  
Microsoft Graph 是 Microsoft 365 中通往数据和智能的网关。 它提供了一个统一的可编程模型，可用于访问 Microsoft 365、Azure、Windows 10 和 企业移动性 + 安全性 中的大量数据集和功能。 你可以利用 Microsoft Graph中丰富的数据来为任何规模的组织构建和管理应用。

### <a name="will-you-release-a-tool-that-helps-me-move-my-apps-from-aad-graph-to-microsoft-graph"></a>你发布一个工具来帮助我将我的应用从 AAD Graph Microsoft Graph？  
虽然我们目前没有任何要宣布的工具，但我们始终致力于改进开发人员的平台体验。 这包括提供工具和数据，以帮助使应用程序通过 API 更改保持最新。

### <a name="how-do-i-get-help-migrating-my-application"></a>如何获取有关迁移我的应用程序的帮助？  
请参阅本文的"下一步"部分。 如果你在阅读后有其他问题，可以使用 标记在 Stack Overflow 上发布，或在 API GitHub `[aadgraph-deprecation]` [库中打开问题](https://github.com/microsoftgraph)。


## <a name="next-steps"></a>后续步骤

- 演练应用 [迁移清单](migrate-azure-ad-graph-planning-checklist.md) ，帮助你规划移动。
- 了解[Microsoft Graph](/graph/overview)概念和做法。
- 使用[Graph资源管理器](https://aka.ms/ge)尝试 Microsoft Graph。
- 若要详细了解进度更新和日程表，请参阅[Microsoft Graph 或 Azure AD Graph。](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)

