---
title: Privileged Identity Management
description: 适合于 Azure AD Privileged Identity Management 的 API，用于管理 Azure Active Directory 角色和 Azure 资源角色。
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 212de5ba66227a090fd6c43e1aff883faf5438ee
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "64477844"
---
# <a name="privileged-identity-management-deprecated"></a>Privileged Identity Management（已弃用）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>2021 年 5 月 31 日，用于 **Azure AD 角色** 的 Privileged Identity Management (PIM) API 已弃用，并停止返回数据。 使用 [角色管理](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) API 并查看 [下面的迁移指南](#migrate-from-pim-v2-to-pim-v3-apis)。
>
>用于 **Azure 资源** 的特权标识管理 (PIM) API 即将弃用。 使用新的 [用于 Azure 资源的 Azure REST PIM API](/rest/api/authorization/role-eligibility-schedule-requests)。 如果要迁移，请参阅下面的迁移指南。

[特权标识管理 (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) 是一项服务，支持你管理、控制和监视对组织中重要资源的访问。 此范围包括对 Azure AD 中的资源、Azure 资源和其他 Microsoft 联机服务（例如 Microsoft 365 或 Microsoft Intune）的访问。

在过去几年中，PIM API 进行了多次迭代。 此迭代是第二次迭代（此处称为 PIM v2），它由 PIM v3 接替。 有关 PIM API 历史记录的详细信息，请参阅 [PIM API 历史记录](/azure/active-directory/privileged-identity-management/pim-apis#pim-api-history)。

Microsoft Graph 提供了以下 PIM v2 API 来管理 Azure AD 角色和 Azure 资源角色。 我们建议从 PIM v2 迁移到 PIM v3。

- [面向 Azure AD 角色的 API](privilegedidentitymanagement-directory.md)（已弃用）
- [面向 Azure 资源的 API](privilegedidentitymanagement-resources.md)

## <a name="migrate-from-pim-v2-to-pim-v3-apis"></a>从 PIM v2 迁移到 PIM v3 API

[!INCLUDE [pimv2AADRoles-migration](../../includes/pimv2AADRoles-migration.md)]

[!INCLUDE [pimv2AzureResources-migration](../../includes/pimv2AzureResources-migration.md)]

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
