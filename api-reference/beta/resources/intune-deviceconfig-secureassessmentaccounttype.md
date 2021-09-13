---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3c7d5577c322db4f980c008f3fbc72d4756733a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081232"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|azureADAccount|0|以 AzureAD\username@tenant.com 格式指示 Azure AD 帐户。|
|domainAccount|1|以 domain\user 或 user@domain.com 格式指示域帐户。|
|localAccount|2|以用户名格式指示本地帐户。|
|localGuestAccount|3|以测试名称的格式指示本地来宾帐户。|



