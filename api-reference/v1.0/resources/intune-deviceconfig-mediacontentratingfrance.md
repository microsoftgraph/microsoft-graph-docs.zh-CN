---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40f4650a99c9914257e868ac7d84f34ed1369276
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359997"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="b7fcd-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7fcd-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="b7fcd-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7fcd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7fcd-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b7fcd-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b7fcd-106">属性</span><span class="sxs-lookup"><span data-stu-id="b7fcd-106">Properties</span></span>
|<span data-ttu-id="b7fcd-107">属性</span><span class="sxs-lookup"><span data-stu-id="b7fcd-107">Property</span></span>|<span data-ttu-id="b7fcd-108">类型</span><span class="sxs-lookup"><span data-stu-id="b7fcd-108">Type</span></span>|<span data-ttu-id="b7fcd-109">说明</span><span class="sxs-lookup"><span data-stu-id="b7fcd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7fcd-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7fcd-110">movieRating</span></span>|[<span data-ttu-id="b7fcd-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7fcd-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="b7fcd-112">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="b7fcd-112">Movies rating selected for France.</span></span> <span data-ttu-id="b7fcd-113">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b7fcd-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b7fcd-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7fcd-114">tvRating</span></span>|[<span data-ttu-id="b7fcd-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7fcd-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="b7fcd-116">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="b7fcd-116">TV rating selected for France.</span></span> <span data-ttu-id="b7fcd-117">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b7fcd-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7fcd-118">关系</span><span class="sxs-lookup"><span data-stu-id="b7fcd-118">Relationships</span></span>
<span data-ttu-id="b7fcd-119">无</span><span class="sxs-lookup"><span data-stu-id="b7fcd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7fcd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7fcd-120">JSON Representation</span></span>
<span data-ttu-id="b7fcd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7fcd-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```




