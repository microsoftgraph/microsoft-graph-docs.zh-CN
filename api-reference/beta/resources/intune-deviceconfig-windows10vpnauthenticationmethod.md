---
title: windows10VpnAuthenticationMethod 枚举类型
description: Windows 10 VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b38ffba54a45bc573e7c6031a6e5aa2aa31d9e49
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124140"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a>windows10VpnAuthenticationMethod 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10 VPN 连接类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|证书|0|使用证书进行身份验证。|
|usernameAndPassword|1 |使用用户名和密码进行身份验证。|
|customEapXml|2 |在自定义 EAP XML 中指定身份验证方法。|
|derivedCredential|3 |使用派生的凭据进行身份验证。|



