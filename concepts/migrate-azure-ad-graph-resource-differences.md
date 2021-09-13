---
title: Azure AD Azure Active Directory (和 Microsoft) Graph 之间的资源类型Graph
description: 介绍 Azure AD Azure Active Directory (中) Graph与 Microsoft Graph 中的资源之间的差异，以帮助迁移应用。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ffd0f23c417ead7fa8457bac9ef8cd00e10f1dcd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044249"
---
# <a name="resource-type-differences-between-azure-active-directory-azure-ad-graph-and-microsoft-graph"></a>Azure AD Azure Active Directory (和 Microsoft) Graph 之间的资源类型Graph

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

将应用从 Azure AD Graph Microsoft Graph时，请注意，某些资源具有不同的名称和类型。  例如，如果你的 Azure AD Graph应用使用 **tenantInfo** 资源，你将需要更新代码以引用 [组织](/graph/api/resources/organization)。

下表重点介绍了 Azure AD Graph 和 Microsoft Graph之间的差异。  它显示名称不同或不可用的资源;它还突出显示了 Beta 版 Microsoft Graph但 v1.0 版本中可用的资源。

如果资源未 **在此** 列表中显示，则它已在 [v1.0](/graph/api/overview)版本的 Microsoft Graph 中可用，其名称与 Azure AD Graph。

> **注意**：Azure AD Graph中的资源类型名称是 Pascal 大小写的，而在 Microsoft Graph它们使用 Camel 大小写。

|Azure AD Graph <br> (v1.6) 资源 |Microsoft Graph<br>resource|注释|
|---|---|---|
| [CertificateAuthorityInformation](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta&preserve-view=true)<br>v1.0 &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority) | |
| [联系人](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta&preserve-view=true)<br>v1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact) | |
| [DirectoryLinkChange](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _&nbsp; 新方法_ <br>v1.0 &nbsp; - &nbsp; _&nbsp; 新方法_ | Delta 查询支持使用不需要此资源的机制进行关系更改检测。 请参阅 Azure [AD Graph 和 Microsoft Graph 之间的功能差异](migrate-azure-ad-graph-feature-differences.md)。 |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope) ||
 [策略](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [策略](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [策略](/graph/api/resources/policy-overview)| 每种类型的策略在 Microsoft Graph 的策略 **URL** 路径段下都有唯一的类型名称和Graph。 在 Azure AD Graph这是单个策略类型。 例如，对于 Azure AD Graph可以使用 **Policy** 资源，将 **type** 属性设置为 ，而在 Microsoft Graph这将是 `TokenIssuancePolicy` **tokenIssuancePolicy** 资源。 |
| [ProvisioningError](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | 此资源已弃用。  但是，可以在[onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError)连接描述任何 AD 或相关设置错误的新资源。 |
| [ServiceEndpoint](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [终结点](/graph/api/resources/endpoint?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [终结点](/graph/api/resources/endpoint) | **endpoints** 仅作为 beta 版 [](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)中的组资源的一部分，以及 beta 和 v1.0 中的 [servicePrincipal](/graph/api/resources/serviceprincipal)资源提供。|
| [SignInName](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _新方法_ <br> v1.0 &nbsp; - &nbsp; _新方法_ | 用于登录用户帐户的标识符的新建模。 有关详细信息 [，请参阅 objectIdentity](/graph/api/resources/objectIdentity) 资源类型。 支持 Azure AD B2C 方案。 |
| [TenantDetail](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [组织](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [组织](/graph/api/resources/organization) | |
| [TrustedCasForPasswordAuth](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity) |  用于登录用户帐户的标识符的新建模称为 **objectIdentity**。 支持 Azure AD B2C 方案。 |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD[应用程序与](migrate-azure-ad-graph-property-differences.md)Microsoft Graph 之间的实体Graph。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
