---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d25c61fe8ffc07de97332da9579abd3fdc433b7f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819162"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|未配置|
|elevateWithoutPrompting|1|提升而不提示。|
|promptForCredentialsOnTheSecureDesktop|2|在安全桌面上提示输入凭据|
|promptForConsentOnTheSecureDesktop|3|在安全桌面上提示同意|
|promptForCredentials|4 |凭据提示|
|promptForConsent|5 |提示同意|
|promptForConsentForNonWindowsBinaries|6 |提示同意非二Windows二进制文件|



