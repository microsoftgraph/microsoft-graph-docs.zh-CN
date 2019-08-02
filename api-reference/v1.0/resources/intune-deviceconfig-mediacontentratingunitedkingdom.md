---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e19ac4fd5fdc63d1635b3f831ebb0f96f934038b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031365"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="ddfca-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="ddfca-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="ddfca-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddfca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddfca-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ddfca-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ddfca-106">属性</span><span class="sxs-lookup"><span data-stu-id="ddfca-106">Properties</span></span>
|<span data-ttu-id="ddfca-107">属性</span><span class="sxs-lookup"><span data-stu-id="ddfca-107">Property</span></span>|<span data-ttu-id="ddfca-108">类型</span><span class="sxs-lookup"><span data-stu-id="ddfca-108">Type</span></span>|<span data-ttu-id="ddfca-109">说明</span><span class="sxs-lookup"><span data-stu-id="ddfca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddfca-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ddfca-110">movieRating</span></span>|[<span data-ttu-id="ddfca-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="ddfca-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="ddfca-112">为英国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="ddfca-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="ddfca-113">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="ddfca-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="ddfca-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ddfca-114">tvRating</span></span>|[<span data-ttu-id="ddfca-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ddfca-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="ddfca-116">为英国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="ddfca-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="ddfca-117">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="ddfca-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddfca-118">关系</span><span class="sxs-lookup"><span data-stu-id="ddfca-118">Relationships</span></span>
<span data-ttu-id="ddfca-119">无</span><span class="sxs-lookup"><span data-stu-id="ddfca-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddfca-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ddfca-120">JSON Representation</span></span>
<span data-ttu-id="ddfca-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddfca-121">Here is a JSON representation of the resource.</span></span>
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



