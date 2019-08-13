---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 892daf67977086b647d74567660d3b4c3d4eec53
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368749"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="98b7e-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="98b7e-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="98b7e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98b7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98b7e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98b7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98b7e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="98b7e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="98b7e-107">属性</span><span class="sxs-lookup"><span data-stu-id="98b7e-107">Properties</span></span>
|<span data-ttu-id="98b7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="98b7e-108">Property</span></span>|<span data-ttu-id="98b7e-109">类型</span><span class="sxs-lookup"><span data-stu-id="98b7e-109">Type</span></span>|<span data-ttu-id="98b7e-110">说明</span><span class="sxs-lookup"><span data-stu-id="98b7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b7e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="98b7e-111">movieRating</span></span>|[<span data-ttu-id="98b7e-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="98b7e-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="98b7e-113">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="98b7e-113">Movies rating selected for France.</span></span> <span data-ttu-id="98b7e-114">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="98b7e-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="98b7e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="98b7e-115">tvRating</span></span>|[<span data-ttu-id="98b7e-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="98b7e-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="98b7e-117">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="98b7e-117">TV rating selected for France.</span></span> <span data-ttu-id="98b7e-118">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="98b7e-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98b7e-119">关系</span><span class="sxs-lookup"><span data-stu-id="98b7e-119">Relationships</span></span>
<span data-ttu-id="98b7e-120">无</span><span class="sxs-lookup"><span data-stu-id="98b7e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98b7e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98b7e-121">JSON Representation</span></span>
<span data-ttu-id="98b7e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98b7e-122">Here is a JSON representation of the resource.</span></span>
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



