---
title: 检查Azure AD Graph API 应用使用情况
description: 介绍如何审核 Azure Active Directory (Azure AD) Graph API 以将应用迁移到 Microsoft Graph API。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: d6a440e71350433feacc1a92fbc6928523c0b534
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077626"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>检查Azure AD Graph API 应用使用情况

这是迁移应用 [过程的第](migrate-azure-ad-graph-planning-checklist.md)2 步。

在规划迁移到 Microsoft Graph时，请花些时间查看现有应用程序，并编录Azure Active Directory (Azure AD) Graph当前使用的 API。

将列表与已知差异进行比较。  这有助于确定迁移应用所需的特定更改。  其中包括使用编辑器的搜索和替换功能轻松解决的简单更改，或者可能需要更多分析的更复杂的更新。

Microsoft Graph 支持许多与 microsoft graph 相同的Azure AD功能。  有一些关键区别：

- [请求差异](migrate-azure-ad-graph-request-differences.md)
- [功能差异](migrate-azure-ad-graph-feature-differences.md)
- [资源类型差异](migrate-azure-ad-graph-resource-differences.md)
- [属性差异](migrate-azure-ad-graph-property-differences.md)
- [方法差异](migrate-azure-ad-graph-method-differences.md)

你还希望验证应用使用的功能所需的权限。  在某些情况下，可以使用更精细的权限。

若要了解详细信息，请参阅[权限](permissions-reference.md)。

## <a name="next-steps"></a>后续步骤

- 了解[应用注册、Azure AD Graph](migrate-azure-ad-graph-app-registration.md)和 Microsoft Graph。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。

