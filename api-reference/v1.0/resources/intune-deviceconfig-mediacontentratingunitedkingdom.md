---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e19ac4fd5fdc63d1635b3f831ebb0f96f934038b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031365"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a>mediaContentRatingUnitedKingdom 资源类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|movieRating|[ratingUnitedKingdomMoviesType](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|为英国选择的电影评级。 可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。|
|tvRating|[ratingUnitedKingdomTelevisionType](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|为英国选择的电视评级。 可取值为：`allAllowed`、`allBlocked`、`caution`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



