---
title: Azure AD应用程序身份验证方法 API 概述
description: 应用程序身份验证方法允许应用获取令牌以访问 Azure AD。
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 8c89a07cae63959904d902ae96ffb886f4877cda
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334112"
---
# <a name="azure-ad-application-authentication-methods-api-overview-preview"></a>Azure AD应用程序身份验证方法 API 概述 (预览) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

应用程序身份验证方法（如证书和密码密码）允许应用获取令牌以访问 Azure Active Directory (Azure AD) 。 这些策略允许 IT 管理员强制执行有关其组织中应用如何使用这些应用程序身份验证方法的最佳实践。 例如，管理员可能会配置一个策略来阻止使用或限制密码密码的生存期，并使用对象的创建日期强制执行该策略。

这些策略允许组织利用新的应用安全强化功能。 通过强制执行基于应用程序或服务主体创建日期的限制，组织可以检查其当前的应用安全状况、清单应用，并按其资源计划和需求强制执行控制。 使用创建日期的此方法，组织可以强制实施新应用程序的策略，还可以将策略应用于现有应用程序。

有两种类型的策略控件：

- 适用于所有应用程序或服务主体的租户默认策略。
- 应用程序 (或服务主体) 管理策略，这些策略允许包含或排除租户默认策略中的单个应用程序。

## <a name="tenant-default-app-management-policy"></a>租户默认应用管理策略

租户默认策略是始终存在的单个对象，默认情况下处于禁用状态。 它由 [tenantAppManagementPolicy](tenantappmanagementpolicy.md) 资源定义，并强制实施对应用程序和服务主体对象的限制。 它包含以下两个属性：

- **applicationRestrictions** 允许将租户拥有的应用程序 (应用程序对象) 。
- **servicePrincipalRestrictions** 允许从另一个租户设置目标 (服务主体对象。

这些属性允许组织锁定源自租户的应用，或提升从租户边界外预配的应用的质量栏。

## <a name="app-management-policy-for-applications-and-service-principals"></a>应用程序和服务主体的应用管理策略

应用管理策略在 [appManagementPolicy](appmanagementpolicy.md) 资源中定义，其中包含一组策略，这些策略具有与租户默认策略中定义的不同限制或强制执行日期。 可以将其中一个策略分配给应用程序或服务主体，将其从租户默认策略中排除。

当租户默认策略和应用管理策略同时存在时，应用管理策略优先，分配的应用程序或服务主体不会从租户默认策略继承。 只能将一个策略分配给应用程序或服务主体。

> [!Note]
> 租户默认策略和应用管理策略均不会阻止现有应用程序的令牌颁发。 不满足策略要求的应用程序将继续工作，直到它尝试更新资源以添加新密码。

## <a name="what-restrictions-can-be-managed-in-microsoft-graph"></a>Microsoft 管理中心可以管理哪些Graph？

应用程序身份验证方法策略 API 提供以下限制：

| 限制名称       | 说明                                                            | 示例                                                                                                    |
| :--------------------- | :--------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------- |
| passwordAddition       | 完全限制应用程序的密码密码。                  | 阻止在"01/01/2019"或之后创建的应用程序的新密码。                                       |
| passwordLifetime       | 强制实施密码密码的最长生存期范围。                    | 对于在 01/01/2015 之后创建的应用程序，将所有新密码密码限制为最多 30 天。        |
| customPasswordAddition | 限制应用程序或服务主体上的自定义密码密码。 | 在 01/ (01/201 Azure AD创建的应用程序上) 所有非自定义密码。 |
| symmetricKeyAddition   | 限制应用程序上的对称密钥。                               | 在 01/01/2019 或之后创建的应用程序上阻止新的对称密钥。                                    |
| symmetricKeyLifetime   | 强制执行对称密钥的最长生存期范围。                      | 对于在 01/01/2019 之后创建的应用程序，将所有新的对称密钥限制为最多 30 天。          |
| asymmetricKeyLifetime  | 对非对称密钥和证书颁发机构强制执行 (生存期) 。      | 对于在 01/01/2019 之后创建的应用程序，将所有新的非对称密钥密码限制为最多 30 天。  |

> [!Note]
> 所有生存期限制均以 ISO-8601 持续时间格式表示 (例如：P4DT12H30M5S) 。
>
> 应用 **customPasswordAddition** 限制将阻止任何将客户端生成的密码密码添加到应用程序或服务主体的旧 PowerShell 模块。 此限制不会阻止Azure AD应用程序或服务主体密码密码。

### <a name="single-vs-multi-tenant-apps"></a>单租户应用与多租户应用

根据应用是单租户应用还是多租户应用，对应用程序或服务主体对象应用策略，如下所示：

- 对于单个租户应用，将策略应用于应用程序对象。
- 若要限制客户租户中的多租户应用，请对应用程序对象应用策略。
- 若要限制从另一个租户预配的多租户应用，请对服务主体对象应用策略。

### <a name="summary-of-key-differences-between-the-tenant-default-policy-and-app-management-policies"></a>租户默认策略与应用管理策略之间主要差异的摘要

| 租户默认策略                                                              | 应用管理策略                                                                                                                               |
| ---------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| 策略始终存在。                                                              | 可以创建或更新策略对象以覆盖默认策略。                                                                                |
| 默认情况下，对 app/SP 禁用限制。                                   | 允许自定义家庭租户中的单个租户或 (或预配的应用支持) 。                                             |
| 仅允许所有资源的单个限制对象定义。                | 允许定义多个策略对象，但只能将一个策略对象应用于资源。                                                            |
| 允许区分应用程序对象和服务主体的限制。 | 策略可以应用于应用程序或服务主体对象。                                                                         |
| 将配置的所有限制应用于所有应用和服务主体。             | 仅将资源策略中配置的限制应用于指定的应用和服务主体，并且不会从默认策略继承。 |

## <a name="next-steps"></a>后续步骤

- [tenantAppManagementPolicy](tenantappmanagementpolicy.md) 资源类型。
- [appManagementPolicy](appmanagementpolicy.md) 资源类型。
