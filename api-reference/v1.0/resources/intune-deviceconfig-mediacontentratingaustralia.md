---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259113"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="1148e-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="1148e-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="1148e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1148e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1148e-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1148e-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1148e-106">属性</span><span class="sxs-lookup"><span data-stu-id="1148e-106">Properties</span></span>
|<span data-ttu-id="1148e-107">属性</span><span class="sxs-lookup"><span data-stu-id="1148e-107">Property</span></span>|<span data-ttu-id="1148e-108">类型</span><span class="sxs-lookup"><span data-stu-id="1148e-108">Type</span></span>|<span data-ttu-id="1148e-109">说明</span><span class="sxs-lookup"><span data-stu-id="1148e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1148e-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1148e-110">movieRating</span></span>|[<span data-ttu-id="1148e-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="1148e-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="1148e-112">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="1148e-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="1148e-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="1148e-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="1148e-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1148e-114">tvRating</span></span>|[<span data-ttu-id="1148e-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1148e-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="1148e-116">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="1148e-116">TV rating selected for Australia.</span></span> <span data-ttu-id="1148e-117">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="1148e-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1148e-118">关系</span><span class="sxs-lookup"><span data-stu-id="1148e-118">Relationships</span></span>
<span data-ttu-id="1148e-119">无</span><span class="sxs-lookup"><span data-stu-id="1148e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1148e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1148e-120">JSON Representation</span></span>
<span data-ttu-id="1148e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1148e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



