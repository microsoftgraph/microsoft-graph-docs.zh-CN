---
title: reportRoot 资源类型
description: 表示 Azure Active Directory (Azure AD) 报告资源的容器。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 51816aef9b5b21732111206785057233c5144bc5
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855936"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory (Azure AD) 报告资源的容器。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
| [列出 applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) 集合 | 检索 **applicationSignInDetailedSummary** 对象。 |
| [获取 applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | 读取 **applicationSignInDetailedSummary** 对象的属性和关系。 |
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | 读取 **applicationSignInSummary** 对象的属性和关系。 |
|[列出 credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 集合|获取给定租户的 credentialUserRegistrationDetails 对象的详细信息。|
|[列出 userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 集合|获取给定租户的 userCredentialUsageDetails 对象。 详细信息包括用户信息、重置状态和失败原因。|
<!--Temporarily hide these functions until we document them and others.
|[getAzureADLicenseUsage](../api/reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/azureadlicenseusage.md) collection|**TODO: Add Description**|
|[getAzureADUserFeatureUsage](../api/reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADFeatureUsage](../api/reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|**TODO: Add Description**|
|[getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|**TODO: Add Description**|
|[getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/credentialusagesummary.md) collection|**TODO: Add -->

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|applicationSignInDetailedSummary|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) 集合|表示应用程序登录的详细摘要。|
|authenticationMethods|[authenticationMethodsRoot](../resources/authenticationmethodsroot.md)|用于 Azure AD 身份验证方法资源的导航属性的容器。|
|credentialUserRegistrationDetails|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 集合|所有已注册用户的自助密码重置和多重身份验证 (MFA) 的使用详细信息。|
|userCredentialUsageDetails|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 集合|表示给定租户的自助密码重置 (SSPR) 用法。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot"
}
```
