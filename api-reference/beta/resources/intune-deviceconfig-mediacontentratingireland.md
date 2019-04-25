---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22b0ad3bc1e83ab0a15c9e2185a5c7586fe31979
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554371"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="919d4-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="919d4-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="919d4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="919d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="919d4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="919d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="919d4-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="919d4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="919d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="919d4-107">Properties</span></span>
|<span data-ttu-id="919d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="919d4-108">Property</span></span>|<span data-ttu-id="919d4-109">类型</span><span class="sxs-lookup"><span data-stu-id="919d4-109">Type</span></span>|<span data-ttu-id="919d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="919d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="919d4-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="919d4-111">movieRating</span></span>|[<span data-ttu-id="919d4-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="919d4-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="919d4-113">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="919d4-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="919d4-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="919d4-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="919d4-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="919d4-115">tvRating</span></span>|[<span data-ttu-id="919d4-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="919d4-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="919d4-117">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="919d4-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="919d4-118">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="919d4-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="919d4-119">关系</span><span class="sxs-lookup"><span data-stu-id="919d4-119">Relationships</span></span>
<span data-ttu-id="919d4-120">无</span><span class="sxs-lookup"><span data-stu-id="919d4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="919d4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="919d4-121">JSON Representation</span></span>
<span data-ttu-id="919d4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="919d4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```





