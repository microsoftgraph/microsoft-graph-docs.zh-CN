---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22037a272e10c78c0d500bb20fb8955e20182170
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146560"
---
# <a name="vpnauthenticationmethod-enum-type"></a>vpnAuthenticationMethod 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 身份验证方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|证书|0|使用证书进行身份验证。|
|usernameAndPassword|1|使用用户名和密码进行身份验证。|
|sharedSecret|2|使用共享密码进行身份验证。  仅对 iOS IKEv2 有效。|
|derivedCredential|3|使用派生的凭据进行身份验证。|
|azureAD|4 |使用 Azure AD 进行身份验证。|



