---
title: 检查 Azure AD Graph API 应用使用情况
description: 介绍如何审核 Azure Active Directory (Azure AD) API 以将应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e7e21f03cdfd8ce3d45f0201d15ec489c7322530
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760691"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>检查 Azure AD Graph API 应用使用情况

这是迁移应用 [过程的第](migrate-azure-ad-graph-planning-checklist.md)2 步。

在计划迁移到 Microsoft Graph 时，请花时间查看现有应用程序并编录你当前使用的 Azure AD Graph API。

将列表与已知差异进行比较。  这有助于确定迁移应用所需的特定更改。  其中包括使用编辑器的搜索和替换功能轻松解决的简单更改，或者可能需要更多分析的更复杂的更新。

Microsoft Graph 支持 Azure AD 图形的许多相同特性和功能。  有一些关键区别：

- [请求差异](migrate-azure-ad-graph-request-differences.md)
- [功能差异](migrate-azure-ad-graph-feature-differences.md)
- [资源类型差异](migrate-azure-ad-graph-resource-differences.md)
- [属性差异](migrate-azure-ad-graph-property-differences.md)
- [方法差异](migrate-azure-ad-graph-method-differences.md)

你还希望验证应用使用的功能所需的权限。  在某些情况下，可以使用更精细的权限。

若要了解详细信息，请参阅[权限](permissions-reference.md)。

## <a name="next-steps"></a>后续步骤

- 了解 [Azure](migrate-azure-ad-graph-app-registration.md) AD Graph 和 Microsoft Graph 之间的应用注册、权限和许可差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。

