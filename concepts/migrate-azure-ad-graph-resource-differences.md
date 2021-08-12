---
title: Azure AD 应用程序与 Microsoft Graph 之间的资源类型Graph
description: 介绍 Azure AD 应用中的资源Graph Microsoft Graph中的资源之间的差异，以帮助迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 5a02e165b84ae35299fe6b6b91e1c4eade61bcb1cd771a1aa43f92f6e4a468fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174792"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD 应用程序与 Microsoft Graph 之间的资源类型Graph

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

将应用从 Azure AD Graph Microsoft Graph时，请注意，某些资源具有不同的名称和类型。  例如，如果你的 Azure AD Graph应用使用 **tenantInfo** 资源，你将需要更新代码来引用 [组织](/graph/api/resources/organization?view=graph-rest-1.0)。

下表重点介绍了 Azure AD Graph 和 Microsoft Graph之间的差异。  它显示名称不同或不可用的资源;它还突出显示了 Microsoft Graph beta 版本中提供的资源，但不在 v1.0 版本中。

如果资源未 **在此** 列表中显示，则它在 [v1.0](/graph/api/overview?view=graph-rest-1.0)版本的 Microsoft Graph 中已经可用，其名称与 Azure AD Graph。

> **注意**：Azure AD Graph资源类型名称是 Pascal 大小写的，而在 Microsoft Graph它们使用 Camel 大小写。

|Azure AD Graph <br> (v1.6) 资源 |Microsoft Graph<br>resource|备注|
|---|---|---|
| [CertificateAuthorityInformation](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-1.0) | |
| [联系人](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-1.0) | |
| [DirectoryLinkChange](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _&nbsp; 新方法_ <br>v1.0 &nbsp; - &nbsp; _&nbsp; 新方法_ | Delta 查询支持使用不需要此资源的机制进行关系更改检测。 请参阅 Azure [AD Graph 和 Microsoft Graph 之间的功能差异](migrate-azure-ad-graph-feature-differences.md)。 |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
 [策略](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [策略](/graph/api/resources/policy-overview?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [策略](/graph/api/resources/policy-overview?view=graph-rest-1.0)| 每种类型的策略在 Microsoft Graph 的策略 **URL** 路径段下都有唯一的类型名称和Graph。 在 Azure AD Graph这是单个策略类型。 例如，对于 Azure AD Graph可以使用 **Policy** 资源，将 **type** 属性设置为 ，而在 Microsoft Graph这将是 `TokenIssuancePolicy` **tokenIssuancePolicy** 资源。 |
| [ProvisioningError](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | 此资源已弃用。  但是，可以在[onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-1.0)连接描述任何 AD 或相关设置错误的新资源。 |
| [ServiceEndpoint](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [终结点](/graph/api/resources/endpoint?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [终结点](/graph/api/resources/endpoint?view=graph-rest-1.0) | **endpoints** 仅作为 beta 版中的 [组](/graph/api/resources/group?view=graph-rest-beta) 资源的一部分，以及 beta 和 v1.0 中的 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 资源提供。|
| [SignInName](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _新方法_ <br> v1.0 &nbsp; - &nbsp; _新方法_ | 用于登录用户帐户的标识符的新建模。 有关详细信息 [，请参阅 objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0) 资源类型。 支持 Azure AD B2C 方案。 |
| [TenantDetail](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [组织](/graph/api/resources/organization?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [组织](/graph/api/resources/organization?view=graph-rest-1.0) | |
| [TrustedCasForPasswordAuth](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-1.0) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-1.0) |  用于登录用户帐户的标识符的新建模称为 **objectIdentity**。 支持 Azure AD B2C 方案。 |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD[应用程序与](migrate-azure-ad-graph-property-differences.md)Microsoft Graph 之间的实体Graph。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。