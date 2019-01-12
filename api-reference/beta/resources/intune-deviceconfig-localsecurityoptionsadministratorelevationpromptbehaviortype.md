---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae886f6c7696150cb85a17cb2caa65823705e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916822"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|未配置|
|elevateWithoutPrompting|1|无提示提升。|
|promptForCredentialsOnTheSecureDesktop|2|在安全桌面上的凭据的提示|
|promptForConsentOnTheSecureDesktop|3|在安全桌面上的同意提示|
|promptForCredentials|4|提示输入凭据|
|promptForConsent|5|同意提示|
|promptForConsentForNonWindowsBinaries|6|非 Windows 二进制文件的同意提示|





