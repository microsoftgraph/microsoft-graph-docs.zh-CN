---
title: 将 Azure AD Graph 应用迁移到 Microsoft Graph
description: 介绍如何将 Azure Active Directory （Azure AD） API 应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 311bc8c800d7415e7e2d192f5b11aed971faafa4
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926776"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>将 Azure AD Graph 应用迁移到 Microsoft Graph

Microsoft Graph 完全替换 Azure Active Directory （Azure AD）图形。 对于大多数生产应用程序，Microsoft Graph 可能已经完全支持 Azure AD 场景。 你现在应开始将 Azure AD Graph 应用移动到 Microsoft Graph。

此外，Microsoft Graph 支持许多新的 Azure AD 数据集和功能，这些功能在 Azure AD Graph 中不可用。 切换到 Microsoft Graph 以利用这些新的 Api，这一切都通过一个单终结点，包括：

- [Office 365 组管理](/graph/office365-groups-concept-overview)
- [外部用户邀请](/graph/api/resources/invitation?view=graph-rest-1.0)
- 能够在删除[用户和 Office 365 组](/graph/api/resources/directory?view=graph-rest-1.0)之后对其进行还原
- [用户和组上的 Webhook 通知](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- 身份管理功能，如：
  - [特权标识管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta)（PIM）仅在需要时和在有限时间段内将用户提升到特权角色
  - [对用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta)访问权限证明的一次性或定期访问审核
  - 帮助组织提供有关法律或合规性要求的信息（如免责声明通知）[的使用条款](/graph/api/resources/accessreviews-root?view=graph-rest-beta)
- 安全功能，如：
  - [身份风险事件](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [风险用户](/graph/api/resources/riskyuser?view=graph-rest-beta)
- 可在更多平台和语言中使用的[客户端库和示例](/graph/)。 Microsoft Graph Sdk 提供了一个可发现接口，可在透明地处理令牌获取、重试处理（由于错误和限制、安全重定向处理以及模型序列化和反序列化）而轻松访问数据。

与 Azure Active Directory 相比，Microsoft Graph 提供了更多的服务访问权限。 这也是[Microsoft 365 服务的 API 网关](/graph/)。

本节中的其余文章将帮助你将应用从 Azure AD Graph 移动到 Microsoft Graph。 你会发现：

- 帮助您进行规划的检查表。
- 描述 Api 之间的特定差异的指南。
- 指向说明特定差异的其他资源和示例的链接。

## <a name="next-steps"></a>后续步骤

- 浏览[应用程序迁移清单](migrate-azure-ad-graph-planning-checklist.md)以帮助您规划移动。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
- 若要了解有关进度更新和时间线的详细信息，请参阅[Microsoft Graph 或 AZURE AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)。
