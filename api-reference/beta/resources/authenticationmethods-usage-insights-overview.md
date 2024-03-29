---
title: 使用身份验证方法使用情况报告 API
description: 身份验证方法使用情况报告可帮助组织了解其最终用户如何使用 Azure Active Directory 功能，如自助服务密码重置和多重身份验证 (MFA) 。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 6af5d1805b09add23cfc6c36c7d10acc1e31dc75
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201603"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>使用身份验证方法使用情况报告 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

身份验证方法使用情况报告可帮助您了解组织中用户使用 Azure Active Directory (Azure AD) 功能的方式，如多重身份验证 (MFA) 、Self-Service 密码重置 (SSPR) 和无密码身份验证。

这些报告提供以下信息：

- 每个身份验证方法注册的用户数
- 注册多重身份验证 (MFA) 、Self-Service 密码重置 (SSPR) 和无密码身份验证等功能的用户数。
- 每个身份验证方法的失败率 

## <a name="permissions"></a>权限
以下权限需要调用此 API。要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Reports.Read.All、AuditLog.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Reports.Read.All、AuditLog.Read.All|

若要访问 API， [需要以下角色之](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) 一：

* 报表阅读人员
* 安全读者
* 安全管理员
* 全局读取者
* 全局管理员

## <a name="licenses"></a>许可证

需要Azure AD Premium P1 P2 许可证才能访问使用情况和见解。 Azure AD SSPR) 网站中提供多重身份验证和自助服务密码重置 (SSPR Azure Active Directory[许可信息](https://azure.microsoft.com/pricing/details/active-directory/)。

## <a name="common-requests"></a>常见请求

下表列出了可用于此 API 的一些常见请求。

| 操作 | 在 Graph 浏览器中试用 | 说明 |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | 获取注册自助服务密码重置和 MFA 的用户数。 |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [GET /credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | 获取使用自助服务密码重置的用户数。 |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | 获取自助服务密码重置和 MFA 注册活动的用户详细信息。 |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [GET /usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | 获取所有自助服务密码重置活动的用户详细信息。 |
| [usersRegisteredByFeature](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta) | 获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数量。 |
| [usersRegisteredByMethod](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta) | 获取针对每个身份验证方法注册的用户数。 |
| [userRegistrationDetails](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/userRegistrationDetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/userRegistrationDetails&version=beta) | 获取所有用户的 MFA 注册详细信息。 |

## <a name="next-steps"></a>后续步骤

- 了解如何部署[Azure Active Directory密码重置。](/azure/active-directory/authentication/howto-sspr-deployment)
- 了解如何部署Azure Active Directory [MFA。](/azure/active-directory/authentication/howto-mfa-getstarted)
- 了解如何启用组合 [安全信息注册](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)。
