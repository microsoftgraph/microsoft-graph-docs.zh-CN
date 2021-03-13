---
title: Azure AD Graph 和 Microsoft Graph 之间的资源类型差异
description: 介绍 Azure AD Graph 中的资源与 Microsoft Graph 中的资源之间的差异，以帮助迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 78cfd1a5f817de6c7efbf7dfc3ec05a13ffaa6ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760642"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 和 Microsoft Graph 之间的资源类型差异

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

将应用从 Azure AD Graph 迁移到 Microsoft Graph 时，请注意某些资源具有不同的名称和类型。  例如，如果你的 Azure AD Graph 应用使用 **tenantInfo** 资源，你将需要更新代码来引用 [组织](/graph/api/resources/organization?view=graph-rest-1.0) 。

下表重点介绍了 Azure AD Graph 和 Microsoft Graph 资源之间的差异。  它显示名称不同或不可用的资源;它还突出显示了 Beta 版 Microsoft Graph 中（而非 v1.0 版本）中的可用资源。

如果资源 **未在此** 列表中显示，则它在 [v1.0](/graph/api/overview?view=graph-rest-1.0) 版本的 Microsoft Graph 中已经可用，其名称与 Azure AD Graph 中的名称相同。

> **注意**：Azure AD Graph 中的资源类型名称是 Pascal 大小写名称，而在 Microsoft Graph 中，它们使用 Camel 大小写。

|Azure AD Graph <br> (v1.6) 资源 |Microsoft Graph<br>resource|备注|
|---|---|---|
| [CertificateAuthorityInformation](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-1.0) | |
| [联系人](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-1.0) | |
| [DirectoryLinkChange](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _&nbsp; 新方法_ <br>v1.0 &nbsp; - &nbsp; _&nbsp; 新方法_ | Delta 查询支持使用不需要此资源的机制进行关系更改检测。 请参阅 Azure [AD Graph 和 Microsoft Graph 之间的功能差异](migrate-azure-ad-graph-feature-differences.md)。 |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
 [策略](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [策略](/graph/api/resources/policy-overview?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [策略](/graph/api/resources/policy-overview?view=graph-rest-1.0)| 每种类型的策略在 Microsoft Graph 的策略 **URL** 路径段下都有唯一的类型名称和结构。 在 Azure AD Graph 中，这是单个策略类型。 例如，对于 Azure AD Graph，你将使用 **Policy** 资源，将 **type** 属性设置为 ，而在 Microsoft Graph 中，这将是 `TokenIssuancePolicy` **tokenIssuancePolicy** 资源。 |
| [ProvisioningError](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | 此资源已弃用。  但是，可以在 [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-1.0)中找到描述任何 AD Connect 相关设置错误的新资源。 |
| [ServiceEndpoint](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [终结点](/graph/api/resources/endpoint?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [终结点](/graph/api/resources/endpoint?view=graph-rest-1.0) | **endpoints** 仅作为 beta 版中的 [组](/graph/api/resources/group?view=graph-rest-beta) 资源的一部分，以及 beta 和 v1.0 中的 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 资源提供。|
| [SignInName](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _新方法_ <br> v1.0 &nbsp; - &nbsp; _新方法_ | 用于登录用户帐户的标识符的新建模。 有关详细信息 [，请参阅 objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0) 资源类型。 支持 Azure AD B2C 方案。 |
| [TenantDetail](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [组织](/graph/api/resources/organization?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [组织](/graph/api/resources/organization?view=graph-rest-1.0) | |
| [TrustedCasForPasswordAuth](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-1.0) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-1.0) |  用于登录用户帐户的标识符的新建模称为 **objectIdentity**。 支持 Azure AD B2C 方案。 |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph [和](migrate-azure-ad-graph-property-differences.md) Microsoft Graph 之间的实体属性差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。