---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b6b90142c50237706ac7e9c887d3a848224c1ec9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356665"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="e36ce-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="e36ce-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="e36ce-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e36ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e36ce-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e36ce-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e36ce-106">属性</span><span class="sxs-lookup"><span data-stu-id="e36ce-106">Properties</span></span>
|<span data-ttu-id="e36ce-107">属性</span><span class="sxs-lookup"><span data-stu-id="e36ce-107">Property</span></span>|<span data-ttu-id="e36ce-108">类型</span><span class="sxs-lookup"><span data-stu-id="e36ce-108">Type</span></span>|<span data-ttu-id="e36ce-109">说明</span><span class="sxs-lookup"><span data-stu-id="e36ce-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e36ce-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e36ce-110">movieRating</span></span>|[<span data-ttu-id="e36ce-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="e36ce-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="e36ce-112">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e36ce-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="e36ce-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="e36ce-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="e36ce-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e36ce-114">tvRating</span></span>|[<span data-ttu-id="e36ce-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e36ce-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="e36ce-116">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e36ce-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="e36ce-117">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e36ce-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e36ce-118">关系</span><span class="sxs-lookup"><span data-stu-id="e36ce-118">Relationships</span></span>
<span data-ttu-id="e36ce-119">无</span><span class="sxs-lookup"><span data-stu-id="e36ce-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e36ce-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e36ce-120">JSON Representation</span></span>
<span data-ttu-id="e36ce-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e36ce-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```




