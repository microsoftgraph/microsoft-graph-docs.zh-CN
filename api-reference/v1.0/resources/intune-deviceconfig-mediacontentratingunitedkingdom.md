---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c9cfdabacee761800d782de379f2a7fe22d799c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367404"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="edff5-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="edff5-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="edff5-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edff5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edff5-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="edff5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="edff5-106">属性</span><span class="sxs-lookup"><span data-stu-id="edff5-106">Properties</span></span>
|<span data-ttu-id="edff5-107">属性</span><span class="sxs-lookup"><span data-stu-id="edff5-107">Property</span></span>|<span data-ttu-id="edff5-108">类型</span><span class="sxs-lookup"><span data-stu-id="edff5-108">Type</span></span>|<span data-ttu-id="edff5-109">说明</span><span class="sxs-lookup"><span data-stu-id="edff5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edff5-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="edff5-110">movieRating</span></span>|[<span data-ttu-id="edff5-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="edff5-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="edff5-112">为英国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="edff5-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="edff5-113">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="edff5-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="edff5-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="edff5-114">tvRating</span></span>|[<span data-ttu-id="edff5-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="edff5-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="edff5-116">为英国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="edff5-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="edff5-117">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="edff5-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edff5-118">关系</span><span class="sxs-lookup"><span data-stu-id="edff5-118">Relationships</span></span>
<span data-ttu-id="edff5-119">无</span><span class="sxs-lookup"><span data-stu-id="edff5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edff5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edff5-120">JSON Representation</span></span>
<span data-ttu-id="edff5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edff5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```




