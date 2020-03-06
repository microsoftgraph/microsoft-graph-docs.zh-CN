---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc67f39a0cbb42dc42d942bd17387ba1f4e99fd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530630"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="e8421-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8421-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="e8421-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8421-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8421-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8421-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8421-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e8421-107">属性</span><span class="sxs-lookup"><span data-stu-id="e8421-107">Properties</span></span>
|<span data-ttu-id="e8421-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8421-108">Property</span></span>|<span data-ttu-id="e8421-109">类型</span><span class="sxs-lookup"><span data-stu-id="e8421-109">Type</span></span>|<span data-ttu-id="e8421-110">说明</span><span class="sxs-lookup"><span data-stu-id="e8421-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8421-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e8421-111">movieRating</span></span>|[<span data-ttu-id="e8421-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="e8421-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="e8421-113">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e8421-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="e8421-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e8421-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e8421-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e8421-115">tvRating</span></span>|[<span data-ttu-id="e8421-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e8421-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="e8421-117">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e8421-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="e8421-118">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="e8421-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8421-119">关系</span><span class="sxs-lookup"><span data-stu-id="e8421-119">Relationships</span></span>
<span data-ttu-id="e8421-120">无</span><span class="sxs-lookup"><span data-stu-id="e8421-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8421-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8421-121">JSON Representation</span></span>
<span data-ttu-id="e8421-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8421-122">Here is a JSON representation of the resource.</span></span>
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




