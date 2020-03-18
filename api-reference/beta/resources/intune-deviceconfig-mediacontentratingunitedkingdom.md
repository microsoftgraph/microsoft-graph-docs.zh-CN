---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc6be04b245e07d9dea11dae750ff5e56b68a5e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788553"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="90da1-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="90da1-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="90da1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90da1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90da1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90da1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90da1-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="90da1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="90da1-107">属性</span><span class="sxs-lookup"><span data-stu-id="90da1-107">Properties</span></span>
|<span data-ttu-id="90da1-108">属性</span><span class="sxs-lookup"><span data-stu-id="90da1-108">Property</span></span>|<span data-ttu-id="90da1-109">类型</span><span class="sxs-lookup"><span data-stu-id="90da1-109">Type</span></span>|<span data-ttu-id="90da1-110">说明</span><span class="sxs-lookup"><span data-stu-id="90da1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90da1-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="90da1-111">movieRating</span></span>|[<span data-ttu-id="90da1-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="90da1-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="90da1-113">为英国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="90da1-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="90da1-114">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="90da1-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="90da1-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="90da1-115">tvRating</span></span>|[<span data-ttu-id="90da1-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="90da1-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="90da1-117">为英国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="90da1-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="90da1-118">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="90da1-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90da1-119">关系</span><span class="sxs-lookup"><span data-stu-id="90da1-119">Relationships</span></span>
<span data-ttu-id="90da1-120">无</span><span class="sxs-lookup"><span data-stu-id="90da1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90da1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90da1-121">JSON Representation</span></span>
<span data-ttu-id="90da1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90da1-122">Here is a JSON representation of the resource.</span></span>
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



