---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3ffc71fa17385ad1e0d00dd77958e65fb7a4aed9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276313"
---
# <a name="vpnauthenticationmethod-enum-type"></a>vpnAuthenticationMethod 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 身份验证方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|证书|0|使用证书进行身份验证。|
|usernameAndPassword|1|使用用户名和密码进行身份验证。|
|sharedSecret|双面|使用共享密钥进行身份验证。  仅对 iOS IKEv2 有效。|
|derivedCredential|第三章|使用派生的凭据进行身份验证。|
|azureAD|4 |使用 Azure AD 进行身份验证。|




