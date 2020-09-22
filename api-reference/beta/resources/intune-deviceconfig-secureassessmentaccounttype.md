---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1bfae831ad9e21bee9438c5b0c776775f6ed726b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049455"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|azureADAccount|0|指示 AzureAD\username@tenant.com 格式的 Azure AD 帐户。|
|domainAccount|1 |指示域帐户的格式为 domain\user 或 user@domain.com。|
|localAccount|2 |指示本地帐户的用户名格式。|
|localGuestAccount|第三章|以测试名称的格式指示本地来宾帐户。|






