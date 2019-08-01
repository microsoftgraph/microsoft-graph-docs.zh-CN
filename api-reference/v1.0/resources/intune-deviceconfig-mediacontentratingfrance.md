---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1376cab9e33cec0bd22c88907d7af6bd05b32c73
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031414"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="19c0c-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="19c0c-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="19c0c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19c0c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c0c-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="19c0c-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="19c0c-106">属性</span><span class="sxs-lookup"><span data-stu-id="19c0c-106">Properties</span></span>
|<span data-ttu-id="19c0c-107">属性</span><span class="sxs-lookup"><span data-stu-id="19c0c-107">Property</span></span>|<span data-ttu-id="19c0c-108">类型</span><span class="sxs-lookup"><span data-stu-id="19c0c-108">Type</span></span>|<span data-ttu-id="19c0c-109">说明</span><span class="sxs-lookup"><span data-stu-id="19c0c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c0c-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="19c0c-110">movieRating</span></span>|[<span data-ttu-id="19c0c-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="19c0c-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="19c0c-112">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="19c0c-112">Movies rating selected for France.</span></span> <span data-ttu-id="19c0c-113">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="19c0c-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="19c0c-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="19c0c-114">tvRating</span></span>|[<span data-ttu-id="19c0c-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="19c0c-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="19c0c-116">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="19c0c-116">TV rating selected for France.</span></span> <span data-ttu-id="19c0c-117">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="19c0c-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19c0c-118">关系</span><span class="sxs-lookup"><span data-stu-id="19c0c-118">Relationships</span></span>
<span data-ttu-id="19c0c-119">无</span><span class="sxs-lookup"><span data-stu-id="19c0c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19c0c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19c0c-120">JSON Representation</span></span>
<span data-ttu-id="19c0c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19c0c-121">Here is a JSON representation of the resource.</span></span>
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



