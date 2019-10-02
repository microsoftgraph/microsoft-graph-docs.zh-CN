---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7aa885ddf964e11cd5cd6c364b98501b5f67c1ff
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359955"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="8f1e8-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f1e8-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="8f1e8-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f1e8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f1e8-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8f1e8-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8f1e8-106">属性</span><span class="sxs-lookup"><span data-stu-id="8f1e8-106">Properties</span></span>
|<span data-ttu-id="8f1e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="8f1e8-107">Property</span></span>|<span data-ttu-id="8f1e8-108">类型</span><span class="sxs-lookup"><span data-stu-id="8f1e8-108">Type</span></span>|<span data-ttu-id="8f1e8-109">说明</span><span class="sxs-lookup"><span data-stu-id="8f1e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f1e8-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8f1e8-110">movieRating</span></span>|[<span data-ttu-id="8f1e8-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="8f1e8-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="8f1e8-112">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="8f1e8-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="8f1e8-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="8f1e8-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="8f1e8-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8f1e8-114">tvRating</span></span>|[<span data-ttu-id="8f1e8-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8f1e8-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="8f1e8-116">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="8f1e8-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="8f1e8-117">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="8f1e8-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f1e8-118">关系</span><span class="sxs-lookup"><span data-stu-id="8f1e8-118">Relationships</span></span>
<span data-ttu-id="8f1e8-119">无</span><span class="sxs-lookup"><span data-stu-id="8f1e8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f1e8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f1e8-120">JSON Representation</span></span>
<span data-ttu-id="8f1e8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f1e8-121">Here is a JSON representation of the resource.</span></span>
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




