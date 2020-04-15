---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b25b309e011645c376a23c08b8673a7579ae69ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410132"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="bba10-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="bba10-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="bba10-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bba10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bba10-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bba10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba10-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bba10-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bba10-107">属性</span><span class="sxs-lookup"><span data-stu-id="bba10-107">Properties</span></span>
|<span data-ttu-id="bba10-108">属性</span><span class="sxs-lookup"><span data-stu-id="bba10-108">Property</span></span>|<span data-ttu-id="bba10-109">类型</span><span class="sxs-lookup"><span data-stu-id="bba10-109">Type</span></span>|<span data-ttu-id="bba10-110">说明</span><span class="sxs-lookup"><span data-stu-id="bba10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba10-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="bba10-111">movieRating</span></span>|[<span data-ttu-id="bba10-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="bba10-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="bba10-113">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="bba10-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="bba10-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15` 或 `agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="bba10-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="bba10-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="bba10-115">tvRating</span></span>|[<span data-ttu-id="bba10-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bba10-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="bba10-117">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="bba10-117">TV rating selected for Australia.</span></span> <span data-ttu-id="bba10-118">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="bba10-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bba10-119">关系</span><span class="sxs-lookup"><span data-stu-id="bba10-119">Relationships</span></span>
<span data-ttu-id="bba10-120">无</span><span class="sxs-lookup"><span data-stu-id="bba10-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bba10-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bba10-121">JSON Representation</span></span>
<span data-ttu-id="bba10-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bba10-122">Here is a JSON representation of the resource.</span></span>
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







