---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ad3ff24cc902a943fd9c146310d58cd1f1bfbd8d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088117"
---
# <a name="vpnauthenticationmethod-enum-type"></a>vpnAuthenticationMethod 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 身份验证方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|证书|0|使用证书进行身份验证。|
|usernameAndPassword|1|使用用户名和密码进行身份验证。|
|sharedSecret|双面|使用共享密钥进行身份验证。  仅对 iOS IKEv2 有效。|
|derivedCredential|第三章|使用派生的凭据进行身份验证。|



