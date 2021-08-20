---
title: userPfxIntendedPurpose 枚举类型
description: 用户 PFX 证书预期用途的支持值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 57b8c0cf50113827447c217ede2e1630b010dad5a97fb57d4aa0cc9dfd41ec8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150169"
---
# <a name="userpfxintendedpurpose-enum-type"></a>userPfxIntendedPurpose 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户 PFX 证书预期用途的支持值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unassigned|0|未分配角色/用法。|
|smimeEncryption|1 |对 S/MIME 加密有效。|
|smimeSigning|2 |对 S/MIME 签名有效。|
|vpn|4 |在 VPN 中有效。|
|wifi|8 |在 WiFi 中有效。|




