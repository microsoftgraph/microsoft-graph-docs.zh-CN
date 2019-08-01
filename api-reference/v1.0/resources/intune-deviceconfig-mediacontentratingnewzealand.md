---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d06658905a5a6e5aaab79bb159a87fe4cb5cf7a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031393"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="85e7a-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="85e7a-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="85e7a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85e7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e7a-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85e7a-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="85e7a-106">属性</span><span class="sxs-lookup"><span data-stu-id="85e7a-106">Properties</span></span>
|<span data-ttu-id="85e7a-107">属性</span><span class="sxs-lookup"><span data-stu-id="85e7a-107">Property</span></span>|<span data-ttu-id="85e7a-108">类型</span><span class="sxs-lookup"><span data-stu-id="85e7a-108">Type</span></span>|<span data-ttu-id="85e7a-109">说明</span><span class="sxs-lookup"><span data-stu-id="85e7a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e7a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="85e7a-110">movieRating</span></span>|[<span data-ttu-id="85e7a-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="85e7a-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="85e7a-112">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="85e7a-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="85e7a-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="85e7a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="85e7a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="85e7a-114">tvRating</span></span>|[<span data-ttu-id="85e7a-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="85e7a-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="85e7a-116">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="85e7a-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="85e7a-117">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="85e7a-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e7a-118">关系</span><span class="sxs-lookup"><span data-stu-id="85e7a-118">Relationships</span></span>
<span data-ttu-id="85e7a-119">无</span><span class="sxs-lookup"><span data-stu-id="85e7a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85e7a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85e7a-120">JSON Representation</span></span>
<span data-ttu-id="85e7a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85e7a-121">Here is a JSON representation of the resource.</span></span>
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



