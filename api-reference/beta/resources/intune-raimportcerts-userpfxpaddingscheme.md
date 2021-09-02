---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案支持的值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2bcc46dfe6bfdf96f996627f06215e5e7a4b6a9b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802724"
---
# <a name="userpfxpaddingscheme-enum-type"></a>userPfxPaddingScheme 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

加密提供程序使用的填充方案支持的值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未知的填充方案。|
|pkcs1|1|不再支持 Pkcs1|
|oaepSha1|2|不再支持 OaepSha1|
|oaepSha256|3|使用 OAEP SHA-256 填充。|
|oaepSha384|4 |使用 OAEP SHA-384 填充。|
|oaepSha512|5 |使用 OAEP SHA-512 填充。|



