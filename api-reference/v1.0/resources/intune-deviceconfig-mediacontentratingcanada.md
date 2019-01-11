---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c40691556e9a8f674256c040a98f22e6ef9d717f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857307"
---
# <a name="mediacontentratingcanada-resource-type"></a>mediaContentRatingCanada 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|movieRating|[ratingCanadaMoviesType](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|分级加拿大所选的影片。 可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。|
|tvRating|[ratingCanadaTelevisionType](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|选定用于加拿大 TV 分级。 可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



