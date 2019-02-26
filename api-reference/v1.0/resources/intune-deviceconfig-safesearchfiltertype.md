---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82f80f6081f57a88fcdf26f7639277d72b5e0d8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250584"
---
# <a name="safesearchfiltertype-enum-type"></a>safeSearchFilterType 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定需要哪个级别的安全搜索 (筛选成人内容)

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义, 默认值, 无意向。|
|全|1|对成人内容严格、最高的筛选。|
|从中|双面|针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。|



