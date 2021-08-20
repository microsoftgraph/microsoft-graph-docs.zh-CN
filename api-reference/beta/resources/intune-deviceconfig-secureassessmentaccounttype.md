---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 567de1b1d67cfb730ee5797e9c8b79f2ffe51d046dccfb8118bbcbc69ae1a6e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183041"
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
|domainAccount|1 |以 domain\user 或 user@domain.com 格式指示域帐户。|
|localAccount|2 |以用户名格式指示本地帐户。|
|localGuestAccount|3 |以测试名称的格式指示本地来宾帐户。|




