---
title: macOSContentCachingType 枚举类型
description: 指示 Apple 的内容缓存服务允许缓存的内容类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0bb0859eb7b409849341b03f51abb838c62f2a18
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783538"
---
# <a name="macoscontentcachingtype-enum-type"></a>macOSContentCachingType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示 Apple 的内容缓存服务允许缓存的内容类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值。 将缓存用户 iCloud 数据和非 iCloud 数据。|
|userContentOnly|1|允许 Apple 的内容缓存服务缓存用户 iCloud 数据。|
|sharedContentOnly|2|允许 Apple 的内容缓存服务缓存非 iCloud (，例如应用和软件更新) 。|



