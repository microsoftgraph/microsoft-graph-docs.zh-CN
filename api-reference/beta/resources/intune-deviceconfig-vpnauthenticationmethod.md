---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0fca9d52b09bdb19f85aa6fa06c166195263af39fbf143e956207f7a5e0a7b30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226341"
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
|usernameAndPassword|1 |使用用户名和密码进行身份验证。|
|sharedSecret|2 |使用共享密码进行身份验证。  仅对 iOS IKEv2 有效。|
|derivedCredential|3 |使用派生的凭据进行身份验证。|
|azureAD|4 |使用 Azure AD 进行身份验证。|




