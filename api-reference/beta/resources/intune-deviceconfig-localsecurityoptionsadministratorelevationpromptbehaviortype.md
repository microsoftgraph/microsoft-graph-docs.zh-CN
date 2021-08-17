---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e0b338fd8fec863185dce90e9de8d1b849310977c6a7e5f6ee0cfe070ef2d0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185843"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|elevateWithoutPrompting|1 |提升而不提示。|
|promptForCredentialsOnTheSecureDesktop|2 |在安全桌面上提示输入凭据|
|promptForConsentOnTheSecureDesktop|3 |在安全桌面上提示同意|
|promptForCredentials|4 |凭据提示|
|promptForConsent|5 |提示同意|
|promptForConsentForNonWindowsBinaries|6 |提示同意非二Windows二进制文件|




