---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f9e620f87173708b852bd7eac79bee5a45e432c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409879"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows10SecureAssessment ConfigurationAccount 允许的帐户的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|azureADAccount|0|指示的 AzureAD\ username@tenant.com 格式中的 Azure AD 帐户。|
|domainAccount|1|指示以 domain\user 或 user@domain.com 格式为域帐户。|
|本地帐户|2|指示本地帐户的用户名的格式。|




