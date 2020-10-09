---
title: 使用身份验证方法使用情况报告 API
description: 身份验证方法使用情况报告可帮助组织了解其最终用户如何使用 Azure Active Directory 功能，如自助密码重置和多重身份验证 (MFA) 。
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 6d626c558dd7728d08682e5eebce138a5197f5b6
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402295"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>使用身份验证方法使用情况报告 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

身份验证方法使用情况报告可帮助你了解组织中的用户如何使用 Azure Active Directory (Azure AD) 功能，如自助密码重置和多重身份验证 (MFA)。

这些报告提供如下信息：

- 您的组织更成功的身份验证方法。 
- 最终用户正在运行的错误类型。
- 您需要运行什么市场活动，以帮助最终用户采用自助密码 rest 和 MFA 的使用。

## <a name="common-requests"></a>常见请求

下表列出了可与此 API 一起使用的一些常见请求。

| 操作 | 在 Graph 浏览器中试用 | 说明 |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | [获取/credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | 获取注册了自助密码重置和 MFA 的用户数。 |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [获取/credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | 获取使用自助密码重置的用户数量。 |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [获取/credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | 获取自服务密码重置和 MFA 注册活动的用户详细信息。 |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [获取/usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | 获取所有自助密码重置活动的用户详细信息。 |

## <a name="licenses"></a>许可证

使用情况报告可用于在租户中利用自助密码重置和 MFA 的许可功能。

## <a name="next-steps"></a>后续步骤

- 了解如何 [部署 Azure Active Directory 自助服务密码重置](/azure/active-directory/authentication/howto-sspr-deployment)。
- 了解如何部署 [Azure Active DIRECTORY MFA](/azure/active-directory/authentication/howto-mfa-getstarted)。
- 了解如何启用 [组合的安全信息注册](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)。