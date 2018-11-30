---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
ms.openlocfilehash: e44af4a72aee8c97a12b3d8dcad767bba08ad005
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041822"
---
# <a name="mediacontentratingcanada-resource-type"></a>mediaContentRatingCanada 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

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





