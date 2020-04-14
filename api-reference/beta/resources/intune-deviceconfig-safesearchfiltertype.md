---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索（筛选成人内容）
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8585745d2f4e9c529e6ef56c9ce209b1da67f2ac
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444875"
---
# <a name="safesearchfiltertype-enum-type"></a>safeSearchFilterType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定需要哪个级别的安全搜索（筛选成人内容）

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义，默认值，无意向。|
|全|1|对成人内容严格、最高的筛选。|
|从中|双面|针对成人内容的中等筛选（将不会筛选有效的搜索结果）。|



