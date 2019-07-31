---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa07ae5ae5da66539da53a02e7d985be471228a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000856"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="037ee-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="037ee-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="037ee-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="037ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="037ee-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="037ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="037ee-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="037ee-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="037ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="037ee-107">Properties</span></span>
|<span data-ttu-id="037ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="037ee-108">Property</span></span>|<span data-ttu-id="037ee-109">类型</span><span class="sxs-lookup"><span data-stu-id="037ee-109">Type</span></span>|<span data-ttu-id="037ee-110">说明</span><span class="sxs-lookup"><span data-stu-id="037ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="037ee-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="037ee-111">movieRating</span></span>|[<span data-ttu-id="037ee-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="037ee-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="037ee-113">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="037ee-113">Movies rating selected for France.</span></span> <span data-ttu-id="037ee-114">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="037ee-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="037ee-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="037ee-115">tvRating</span></span>|[<span data-ttu-id="037ee-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="037ee-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="037ee-117">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="037ee-117">TV rating selected for France.</span></span> <span data-ttu-id="037ee-118">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="037ee-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="037ee-119">关系</span><span class="sxs-lookup"><span data-stu-id="037ee-119">Relationships</span></span>
<span data-ttu-id="037ee-120">无</span><span class="sxs-lookup"><span data-stu-id="037ee-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="037ee-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="037ee-121">JSON Representation</span></span>
<span data-ttu-id="037ee-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="037ee-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```





