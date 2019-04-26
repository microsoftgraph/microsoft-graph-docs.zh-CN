---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 564e641fcdc7e0d06d48666881fc3bcedfe3505c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573212"
---
# <a name="safesearchfiltertype-enum-type"></a>safeSearchFilterType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定需要哪个级别的安全搜索 (筛选成人内容)

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义, 默认值, 无意向。|
|全|1|对成人内容严格、最高的筛选。|
|从中|2 |针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。|





