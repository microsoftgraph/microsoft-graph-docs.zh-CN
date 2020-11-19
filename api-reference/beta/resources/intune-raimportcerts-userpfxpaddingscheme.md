---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案的受支持的值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0cbdc056c1dc0ea1aa73ae0cd96af428ce9f2bf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307168"
---
# <a name="userpfxpaddingscheme-enum-type"></a>userPfxPaddingScheme 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

加密提供程序使用的填充方案的受支持的值。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|未知的填充方案。|
|pkcs1|1|不再支持 Pkcs1|
|oaepSha1|双面|不再支持 OaepSha1|
|oaepSha256|第三章|使用 OAEP SHA-256 填充。|
|oaepSha384|4 |使用 OAEP SHA-384 填充。|
|oaepSha512|5 |使用 OAEP SHA-512 填充。|




