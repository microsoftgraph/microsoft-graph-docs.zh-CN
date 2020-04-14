---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d0d5c8cd8a38589cef548d03c290015bd4368e12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439860"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|elevateWithoutPrompting|1|在不提示的情况下提升。|
|promptForCredentialsOnTheSecureDesktop|双面|在安全桌面上提示凭据|
|promptForConsentOnTheSecureDesktop|第三章|安全桌面上的同意提示|
|promptForCredentials|4 |提示输入凭据|
|promptForConsent|5 |同意提示|
|promptForConsentForNonWindowsBinaries|6 |非 Windows 二进制文件的同意提示|



