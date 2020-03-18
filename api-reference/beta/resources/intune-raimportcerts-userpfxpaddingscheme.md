---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案的受支持的值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 73cd96dcc01a99df657ca7f538046c7e5e7ed4a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42774223"
---
# <a name="userpfxpaddingscheme-enum-type"></a>userPfxPaddingScheme 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

加密提供程序使用的填充方案的受支持的值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未知的填充方案。|
|pkcs1|1|不再支持 Pkcs1|
|oaepSha1|双面|不再支持 OaepSha1|
|oaepSha256|第三章|使用 OAEP SHA-256 填充。|
|oaepSha384|4 |使用 OAEP SHA-384 填充。|
|oaepSha512|5 |使用 OAEP SHA-512 填充。|



