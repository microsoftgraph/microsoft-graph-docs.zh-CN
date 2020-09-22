---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 658141a661bd46374c63a2c7eb9378a16d4135aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993796"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="9054f-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="9054f-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="9054f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9054f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9054f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9054f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9054f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9054f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9054f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9054f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9054f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9054f-108">Properties</span></span>
|<span data-ttu-id="9054f-109">属性</span><span class="sxs-lookup"><span data-stu-id="9054f-109">Property</span></span>|<span data-ttu-id="9054f-110">类型</span><span class="sxs-lookup"><span data-stu-id="9054f-110">Type</span></span>|<span data-ttu-id="9054f-111">说明</span><span class="sxs-lookup"><span data-stu-id="9054f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9054f-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="9054f-112">movieRating</span></span>|[<span data-ttu-id="9054f-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="9054f-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="9054f-114">为日本选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="9054f-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="9054f-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="9054f-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9054f-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="9054f-116">tvRating</span></span>|[<span data-ttu-id="9054f-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9054f-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="9054f-118">为日本选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="9054f-118">TV rating selected for Japan.</span></span> <span data-ttu-id="9054f-119">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="9054f-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9054f-120">关系</span><span class="sxs-lookup"><span data-stu-id="9054f-120">Relationships</span></span>
<span data-ttu-id="9054f-121">无</span><span class="sxs-lookup"><span data-stu-id="9054f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9054f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9054f-122">JSON Representation</span></span>
<span data-ttu-id="9054f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9054f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```






