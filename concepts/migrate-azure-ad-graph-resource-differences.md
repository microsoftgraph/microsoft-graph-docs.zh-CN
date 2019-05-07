---
title: Azure AD Graph 与 Microsoft Graph 之间的资源类型差异
description: 介绍了 Azure AD Graph 中的资源与 Microsoft Graph 中的资源之间的差异, 以便帮助迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 590ec2fae33e5172e274341793c82409a4c28c8c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630200"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 与 Microsoft Graph 之间的资源类型差异

本文是*第1步: 查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

将应用程序从 Azure AD Graph 迁移到 Microsoft Graph 时, 请注意, 某些资源的名称和类型不同。  例如, 如果您的 Azure AD Graph 应用使用**tenantInfo**资源, 则需要更新代码以改为引用[组织](/graph/api/resources/organization?view=graph-rest-1.0)。

下表重点介绍了 Azure AD Graph 和 Microsoft Graph 资源之间的差异。  它显示具有不同名称或不可用的资源。它还突出显示了 Microsoft Graph beta 版中的可用资源, 而不是在 v1。0版本中。

如果某个资源未显示在此列表中, 则它已在第[1。0版](/graph/api/overview?view=graph-rest-1.0)Microsoft Graph 中可用, 与 Azure AD Graph 中的名称相同。

> **注意**: Azure AD Graph 中的资源类型名称是 pascal 大小写形式的, 而在 Microsoft Graph 中, 它们的大小写混合。

|Azure AD Graph <br>(1.60 1。6) 资源 |Microsoft Graph<br>resource|Comments|
|---|---|---|
| [接](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)       | beta 版-_尚不可用_<br>v1。0-_尚不可用_ ||
| [应用程序](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-[应用程序](/graph/api/resources/application?view=graph-rest-beta)<br>v1。0-_尚不可用_ ||
| [AppRole](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [appRole](/graph/api/resources/approle?view=graph-rest-beta)<br>v1。0-_尚不可用_ | |
| [AppRoleAssignment](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp;-beta&nbsp;[appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta)<br>v1。0-_尚不可用_ | |
| [联系人](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v1。0-_尚不可用_ | |
| [DirectoryLinkChange](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta 版 _-&nbsp;新方法_ <br>1。0版-_新&nbsp;方法_ | Delta 查询支持具有不需要此资源的机制的关系更改检测。 请参阅[AZURE AD Graph 和 Microsoft Graph 之间的功能差异](migrate-azure-ad-graph-feature-differences.md)。 |
| [KeyCredential](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)| beta- [keyCredential](/graph/api/resources/keyCredential?view=graph-rest-beta)<br>v1。0-_尚不可用_ | |
| [键值](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-[键值](/graph/api/resources/keyValue?view=graph-rest-beta) <br> v1。0-_尚不可用_ ||
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v1。0-_尚不可用_ ||
| [OAuth2PermissionGrant](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp;-beta&nbsp;[oAuth2PermissionGrant](/graph/api/resources/oAuth2PermissionGrant?view=graph-rest-beta) <br> v1。0-_尚不可用_ ||
| [OptionalClaim](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-optionalClaim <br> v1。0-_尚不可用_ | |
| [OptionalClaims](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-optionalClaims<br> v1。0-_尚不可用_ ||
| [ParentalControlSettings](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [parentalControlSettings](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) <br> v1。0-_尚不可用_ ||
| [PasswordCredential](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [passwordCredential](/graph/api/resources/passwordCredential?view=graph-rest-beta) <br> v1。0-_尚不可用_ ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [passwordProfile](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> v1。0-PasswordProfile ||
| [策略](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-[策略](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) _(可能会更改)_ <br> v1。0-_尚不可用_ | 每个策略都将具有唯一的类型名称和结构。|
| [ProvisioningError](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp;-beta&nbsp;[onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-beta) <br> &nbsp;-v1。0&nbsp;onPremisesProvisioningError  | |
| [RequiredResourceAccess](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [requiredResourceAccess](/graph/api/resources/requiredResourceAccess?view=graph-rest-beta) <br> v1。0-_尚不可用_ | |
| [ResourceAccess](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [resourceAccess](/graph/api/resources/resourceAccess?view=graph-rest-beta) <br> v1。0-_尚不可用_ | |
| [ServiceEndpoint](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-[终结点](/graph/api/resources/endpoint?view=graph-rest-beta) <br> v1。0-终结点_尚不可用_ | [终结点](/graph/api/resources/endpoint?view=graph-rest-beta)仅可用作[组](/graph/api/resources/group?view=graph-rest-beta)资源的一部分|
| [ServicePrincipal](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) <br> v1。0-_尚不可用_ | |
| [SignInName](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | 用于登录到用户帐户 (称为**identityObject**, 但尚不可用) 的标识符的新建模。 支持 Azure AD B2C 方案。 |
| [TenantDetail](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta-[组织](/graph/api/resources/organization?view=graph-rest-beta) <br> v1。0-[组织](/graph/api/resources/organization?view=graph-rest-v1.0) | |
| [TrustedCasForPasswordAuth](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_  | 重命名为**certificateBasedAuthConfiguration** , 但尚不可用。|
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ |  用于登录到用户帐户 (称为**identityObject**, 但尚不可用) 的标识符的新建模。 支持 Azure AD B2C 方案。 |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间的[实体属性差异](migrate-azure-ad-graph-property-differences.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
