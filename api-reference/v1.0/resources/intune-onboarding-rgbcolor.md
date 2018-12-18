---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
ms.openlocfilehash: b469533b8ee7e54e99b09be08870045d759f5322
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350958"
---
# <a name="rgbcolor-resource-type"></a>rgbColor 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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



