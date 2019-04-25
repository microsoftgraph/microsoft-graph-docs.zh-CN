---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 979a5996b655ba13847e52dc09b083169ff0815a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572344"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="751a8-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="751a8-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="751a8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="751a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="751a8-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="751a8-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="751a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="751a8-106">Properties</span></span>
|<span data-ttu-id="751a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="751a8-107">Property</span></span>|<span data-ttu-id="751a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="751a8-108">Type</span></span>|<span data-ttu-id="751a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="751a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751a8-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="751a8-110">movieRating</span></span>|[<span data-ttu-id="751a8-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="751a8-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="751a8-112">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="751a8-112">Movies rating selected for France.</span></span> <span data-ttu-id="751a8-113">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="751a8-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="751a8-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="751a8-114">tvRating</span></span>|[<span data-ttu-id="751a8-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="751a8-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="751a8-116">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="751a8-116">TV rating selected for France.</span></span> <span data-ttu-id="751a8-117">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="751a8-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="751a8-118">关系</span><span class="sxs-lookup"><span data-stu-id="751a8-118">Relationships</span></span>
<span data-ttu-id="751a8-119">无</span><span class="sxs-lookup"><span data-stu-id="751a8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="751a8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="751a8-120">JSON Representation</span></span>
<span data-ttu-id="751a8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="751a8-121">Here is a JSON representation of the resource.</span></span>
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



