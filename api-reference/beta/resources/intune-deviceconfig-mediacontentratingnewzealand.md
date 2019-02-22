---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9328ccc8b3c6b7ce6af220d8f798497e00448a8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159274"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="46184-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="46184-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="46184-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46184-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46184-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46184-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46184-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="46184-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="46184-107">属性</span><span class="sxs-lookup"><span data-stu-id="46184-107">Properties</span></span>
|<span data-ttu-id="46184-108">属性</span><span class="sxs-lookup"><span data-stu-id="46184-108">Property</span></span>|<span data-ttu-id="46184-109">类型</span><span class="sxs-lookup"><span data-stu-id="46184-109">Type</span></span>|<span data-ttu-id="46184-110">说明</span><span class="sxs-lookup"><span data-stu-id="46184-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46184-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="46184-111">movieRating</span></span>|[<span data-ttu-id="46184-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="46184-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="46184-113">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="46184-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="46184-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="46184-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="46184-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="46184-115">tvRating</span></span>|[<span data-ttu-id="46184-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="46184-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="46184-117">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="46184-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="46184-118">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="46184-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46184-119">关系</span><span class="sxs-lookup"><span data-stu-id="46184-119">Relationships</span></span>
<span data-ttu-id="46184-120">无</span><span class="sxs-lookup"><span data-stu-id="46184-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46184-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46184-121">JSON Representation</span></span>
<span data-ttu-id="46184-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46184-122">Here is a JSON representation of the resource.</span></span>
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




