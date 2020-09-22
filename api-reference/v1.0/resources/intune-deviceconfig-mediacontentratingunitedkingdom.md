---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e9fd03ebd0834ff63c129216833673255715f76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003085"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="3cf33-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="3cf33-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="3cf33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cf33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cf33-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cf33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cf33-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3cf33-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3cf33-107">属性</span><span class="sxs-lookup"><span data-stu-id="3cf33-107">Properties</span></span>
|<span data-ttu-id="3cf33-108">属性</span><span class="sxs-lookup"><span data-stu-id="3cf33-108">Property</span></span>|<span data-ttu-id="3cf33-109">类型</span><span class="sxs-lookup"><span data-stu-id="3cf33-109">Type</span></span>|<span data-ttu-id="3cf33-110">说明</span><span class="sxs-lookup"><span data-stu-id="3cf33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cf33-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="3cf33-111">movieRating</span></span>|[<span data-ttu-id="3cf33-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="3cf33-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="3cf33-113">为英国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="3cf33-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="3cf33-114">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="3cf33-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="3cf33-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="3cf33-115">tvRating</span></span>|[<span data-ttu-id="3cf33-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3cf33-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="3cf33-117">为英国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="3cf33-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="3cf33-118">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="3cf33-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cf33-119">关系</span><span class="sxs-lookup"><span data-stu-id="3cf33-119">Relationships</span></span>
<span data-ttu-id="3cf33-120">无</span><span class="sxs-lookup"><span data-stu-id="3cf33-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cf33-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cf33-121">JSON Representation</span></span>
<span data-ttu-id="3cf33-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cf33-122">Here is a JSON representation of the resource.</span></span>
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









