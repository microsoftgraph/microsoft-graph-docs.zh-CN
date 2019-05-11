---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8deeae69bb4d828cc2e0178c79aba200f8a4709e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946810"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

EAP 快速配置的可用设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST (无保护性访问凭据 (PAC))。|
|useProtectedAccessCredential|1|使用受保护的访问凭据 (PAC)。|
|useProtectedAccessCredentialAndProvision|双面|使用保护性接入身分凭证 (PAC) 和预配 PAC。|
|useProtectedAccessCredentialAndProvisionAnonymously|第三章|使用受保护的访问凭据 (PAC)、预配 PAC, 并以匿名方式执行此操作。|




