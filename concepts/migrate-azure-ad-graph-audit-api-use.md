---
title: 检查 Azure AD Graph Api 应用程序使用情况
description: 介绍如何审核 Azure Active Directory (Azure AD) Api, 以将应用程序迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecf6d1897d8473b42ac8b5bcb45c59747eb36f13
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630270"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>检查 Azure AD Graph Api 应用程序使用情况

这是[迁移应用程序过程](migrate-azure-ad-graph-planning-checklist.md)的步骤2。

在规划到 Microsoft Graph 的迁移时, 请花时间查看现有应用程序, 并对您当前使用的 Azure AD Graph Api 进行编目。

将您的列表与已知的区别进行比较。  这有助于确定迁移应用程序所需的特定更改。  其中包括使用编辑器的搜索和替换功能或更多可能需要更多分析的更复杂的更新轻松解析的简单更改。

Microsoft Graph 支持 Azure AD Graph 的许多相同特性和功能。  有几个关键区别:

- [请求差异](migrate-azure-ad-graph-request-differences.md)
- [功能差异](migrate-azure-ad-graph-feature-differences.md)
- [资源类型差异](migrate-azure-ad-graph-resource-differences.md)
- [属性差异](migrate-azure-ad-graph-property-differences.md)
- [方法差异](migrate-azure-ad-graph-method-differences.md)

您还需要验证您的应用程序所使用的功能所需的权限。  在某些情况下, 可以使用更精细的权限。

若要了解详细信息，请参阅[权限](/concepts/permissions-reference.md)。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间[的应用注册、权限和同意差异](migrate-azure-ad-graph-app-registration.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
