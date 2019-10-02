---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 419577efc7993479e8f378227d5f6c073e8e2492
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360725"
---
# <a name="rgbcolor-resource-type"></a>rgbColor 资源类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

以 RGB 表示的颜色。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|r|字节|红色值|
|g|字节|绿色值|
|b|字节|蓝色值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```




