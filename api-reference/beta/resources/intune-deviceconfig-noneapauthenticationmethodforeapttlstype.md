---
title: nonEapAuthenticationMethodForEapTtlsType 枚举类型
description: 用于身份验证的非 EAP 方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3eb4a4ed8663511900424038df621a62e75e109c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529586"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a>nonEapAuthenticationMethodForEapTtlsType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于身份验证的非 EAP 方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unencryptedPassword|0|未加密的密码（PAP）。|
|challengeHandshakeAuthenticationProtocol|1 |质询握手身份验证协议（CHAP）。|
|microsoftChap|2 | Microsoft CHAP （毫秒-CHAP）。|
|microsoftChapVersionTwo|3 |Microsoft CHAP 版本2（毫秒-CHAP v2）。|



