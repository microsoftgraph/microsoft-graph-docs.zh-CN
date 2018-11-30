---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: 凭据 Guard 设置的可能值。
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041522"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

凭据 Guard 设置的可能值。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|关闭凭据 Guard 远程如果没有 UEFI 锁定之前配置。|
|enableWithUEFILock|1|打开与 UEFI 锁定凭据 Guard。|
|enableWithoutUEFILock|2|UEFI 锁定的情况下启用凭据 Guard。|





