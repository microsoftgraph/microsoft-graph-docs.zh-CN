---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4f2eda6b9666d3b23ea48d96f7a7231e189b4f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028096"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="c8642-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8642-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="c8642-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8642-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8642-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c8642-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c8642-106">属性</span><span class="sxs-lookup"><span data-stu-id="c8642-106">Properties</span></span>
|<span data-ttu-id="c8642-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8642-107">Property</span></span>|<span data-ttu-id="c8642-108">类型</span><span class="sxs-lookup"><span data-stu-id="c8642-108">Type</span></span>|<span data-ttu-id="c8642-109">说明</span><span class="sxs-lookup"><span data-stu-id="c8642-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8642-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c8642-110">movieRating</span></span>|[<span data-ttu-id="c8642-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="c8642-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="c8642-112">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="c8642-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="c8642-113">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="c8642-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c8642-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c8642-114">tvRating</span></span>|[<span data-ttu-id="c8642-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c8642-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="c8642-116">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="c8642-116">TV rating selected for Germany.</span></span> <span data-ttu-id="c8642-117">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c8642-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8642-118">关系</span><span class="sxs-lookup"><span data-stu-id="c8642-118">Relationships</span></span>
<span data-ttu-id="c8642-119">无</span><span class="sxs-lookup"><span data-stu-id="c8642-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8642-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8642-120">JSON Representation</span></span>
<span data-ttu-id="c8642-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8642-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



