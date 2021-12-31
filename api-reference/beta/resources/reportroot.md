---
title: reportRoot 资源类型
description: 用于报告Azure AD的容器。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0cd17a6f8a06b9c5a4b263b06c3bb3ec71d7dc0c
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647052"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开报告资源的导航属性Azure AD容器。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
| [列出 applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) 集合 | 检索 **applicationSignInDetailedSummary** 对象。 |
| [获取 applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | 读取 **applicationSignInDetailedSummary 对象的属性和** 关系。 |
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | 读取 **applicationSignInSummary 对象的属性和** 关系。 |
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
|属性|类型|说明|
|:---|:---|:---|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|applicationSignInDetailedSummary|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) 集合|表示应用程序登录的详细摘要。|
|authenticationMethods|[authenticationMethodsRoot](../resources/authenticationmethodsroot.md)|用于身份验证方法资源的Azure AD属性的容器。|
|credentialUserRegistrationDetails|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 集合|有关针对所有注册用户的自助服务密码重置和多重身份验证 (MFA) 的详细信息。|
|userCredentialUsageDetails|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 集合|表示给定租户的 SSPR (密码) 重置密码。|

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
