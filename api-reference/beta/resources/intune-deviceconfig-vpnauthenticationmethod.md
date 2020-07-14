---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef477b17b8ae7e8aedc3b95ce70b66115a3c8712
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123888"
---
# <a name="vpnauthenticationmethod-enum-type"></a>vpnAuthenticationMethod 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 身份验证方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|证书|0|使用证书进行身份验证。|
|usernameAndPassword|1 |使用用户名和密码进行身份验证。|
|sharedSecret|2 |使用共享密钥进行身份验证。  仅对 iOS IKEv2 有效。|
|derivedCredential|3 |使用派生的凭据进行身份验证。|
|azureAD|4 |使用 Azure AD 进行身份验证。|



