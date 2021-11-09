---
title: Privileged Identity Management
description: 适合于 Azure AD Privileged Identity Management 的 API，用于管理 Azure Active Directory 角色和 Azure 资源角色。
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 09d416ebe637a82f174b9668d4b9396626e0d5a3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695473"
---
# <a name="privileged-identity-management-deprecated"></a>Privileged Identity Management（已弃用）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>2021 年 5 月 31 日，用于 **Azure AD 角色** 的 Privileged Identity Management (PIM) API 已弃用，并停止返回数据。 请使用[角色管理](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) API。
>
>用于 **Azure 资源角色** 的 Privileged Identity Management (PIM) API 即将弃用。 使用新的[用于 Azure 资源角色的 Azure REST PIM API](/rest/api/authorization/role-eligibility-schedule-requests)。

[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) 是可便于管理、控制和监视对组织中重要资源的访问的服务。 这包括访问 Azure AD、Azure 资源和其他 Microsoft Online Services（例如 Microsoft 365 或 Microsoft Intune）中的资源。

Microsoft Graph 提供了以下 API 来管理 Azure AD 角色和 Azure 资源角色：

- [适用于 Azure AD 橘色的 API](privilegedidentitymanagement-directory.md)
- [适用于 Azure 资源角色 的 API](privilegedidentitymanagement-resources.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
