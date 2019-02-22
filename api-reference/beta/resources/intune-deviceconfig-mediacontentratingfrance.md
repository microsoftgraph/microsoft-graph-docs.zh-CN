---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40883571c2c17b466dbc6740280c34f8efa55282
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165665"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="9e37f-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e37f-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="9e37f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e37f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e37f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e37f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e37f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9e37f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9e37f-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e37f-107">Properties</span></span>
|<span data-ttu-id="9e37f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e37f-108">Property</span></span>|<span data-ttu-id="9e37f-109">类型</span><span class="sxs-lookup"><span data-stu-id="9e37f-109">Type</span></span>|<span data-ttu-id="9e37f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9e37f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e37f-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9e37f-111">movieRating</span></span>|[<span data-ttu-id="9e37f-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="9e37f-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="9e37f-113">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="9e37f-113">Movies rating selected for France.</span></span> <span data-ttu-id="9e37f-114">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="9e37f-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9e37f-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9e37f-115">tvRating</span></span>|[<span data-ttu-id="9e37f-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9e37f-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="9e37f-117">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="9e37f-117">TV rating selected for France.</span></span> <span data-ttu-id="9e37f-118">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="9e37f-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e37f-119">关系</span><span class="sxs-lookup"><span data-stu-id="9e37f-119">Relationships</span></span>
<span data-ttu-id="9e37f-120">无</span><span class="sxs-lookup"><span data-stu-id="9e37f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e37f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e37f-121">JSON Representation</span></span>
<span data-ttu-id="9e37f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e37f-122">Here is a JSON representation of the resource.</span></span>
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




