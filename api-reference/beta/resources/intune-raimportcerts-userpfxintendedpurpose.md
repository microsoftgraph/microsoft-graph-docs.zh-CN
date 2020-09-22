---
title: userPfxIntendedPurpose 枚举类型
description: 用户 PFX 证书的预期目的支持的值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: be8b798dfc79bd291f3ce91021ea15ff5d36639f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993285"
---
# <a name="userpfxintendedpurpose-enum-type"></a>userPfxIntendedPurpose 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户 PFX 证书的预期目的支持的值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|取消|0|未分配角色/用法。|
|smimeEncryption|1 |对 S/MIME 加密有效。|
|smimeSigning|2 |对 S/MIME 签名有效。|
|vpn|4 |在 VPN 中使用时有效。|
|wifi|8 |在 WiFi 中使用时有效。|






