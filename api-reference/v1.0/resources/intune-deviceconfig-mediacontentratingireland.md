---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e281a233b000adc189c071148959e058f9cfa5fa
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451890"
---
# <a name="mediacontentratingireland-resource-type"></a>mediaContentRatingIreland 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|movieRating|[ratingIrelandMoviesType](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|为爱尔兰选择的电影评级。 可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。|
|tvRating|[ratingIrelandTelevisionType](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|为爱尔兰选择的电视评级。 可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



