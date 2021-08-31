---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c0f007191f4ba450c957c2cf1921c7956110cea
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803754"
---
# <a name="rgbcolor-resource-type"></a>rgbColor 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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



