---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c91558168922c4b608d62add941b69a5749bc9f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795798"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="c1fcc-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1fcc-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="c1fcc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1fcc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1fcc-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c1fcc-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c1fcc-107">属性</span><span class="sxs-lookup"><span data-stu-id="c1fcc-107">Properties</span></span>
|<span data-ttu-id="c1fcc-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1fcc-108">Property</span></span>|<span data-ttu-id="c1fcc-109">类型</span><span class="sxs-lookup"><span data-stu-id="c1fcc-109">Type</span></span>|<span data-ttu-id="c1fcc-110">说明</span><span class="sxs-lookup"><span data-stu-id="c1fcc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1fcc-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c1fcc-111">movieRating</span></span>|[<span data-ttu-id="c1fcc-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="c1fcc-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="c1fcc-113">为英国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="c1fcc-114">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="c1fcc-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c1fcc-115">tvRating</span></span>|[<span data-ttu-id="c1fcc-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c1fcc-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="c1fcc-117">为英国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="c1fcc-118">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1fcc-119">关系</span><span class="sxs-lookup"><span data-stu-id="c1fcc-119">Relationships</span></span>
<span data-ttu-id="c1fcc-120">无</span><span class="sxs-lookup"><span data-stu-id="c1fcc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1fcc-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1fcc-121">JSON Representation</span></span>
<span data-ttu-id="c1fcc-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1fcc-122">Here is a JSON representation of the resource.</span></span>
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





