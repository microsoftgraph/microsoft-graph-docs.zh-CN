---
title: macOSContentCachingType 枚举类型
description: 指示 Apple 的内容缓存服务允许缓存的内容类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a79cd14a6bd765f260439a259c63106e6211cacc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268732"
---
# <a name="macoscontentcachingtype-enum-type"></a>macOSContentCachingType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示 Apple 的内容缓存服务允许缓存的内容类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值。 将缓存用户 iCloud 数据和非 iCloud 数据。|
|userContentOnly|1|允许 Apple 的内容缓存服务缓存用户 iCloud 数据。|
|sharedContentOnly|双面|允许 Apple 的内容缓存服务缓存非 iCloud 数据 (例如，应用程序和软件更新) 。|




