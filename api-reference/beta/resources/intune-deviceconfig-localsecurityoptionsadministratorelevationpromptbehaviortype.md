---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460525"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|elevateWithoutPrompting|1|在不提示的情况下提升。|
|promptForCredentialsOnTheSecureDesktop|2 |在安全桌面上提示凭据|
|promptForConsentOnTheSecureDesktop|3 |安全桌面上的同意提示|
|promptForCredentials|4 |提示输入凭据|
|promptForConsent|5|同意提示|
|promptForConsentForNonWindowsBinaries|6 |非 Windows 二进制文件的同意提示|





