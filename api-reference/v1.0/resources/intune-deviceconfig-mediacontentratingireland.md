---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7c808cd6c614837acbb863e92323429d5b4a110
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003120"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="9d099-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d099-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="9d099-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d099-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d099-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d099-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d099-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9d099-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9d099-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d099-107">Properties</span></span>
|<span data-ttu-id="9d099-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d099-108">Property</span></span>|<span data-ttu-id="9d099-109">类型</span><span class="sxs-lookup"><span data-stu-id="9d099-109">Type</span></span>|<span data-ttu-id="9d099-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d099-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d099-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9d099-111">movieRating</span></span>|[<span data-ttu-id="9d099-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="9d099-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="9d099-113">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="9d099-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="9d099-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="9d099-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="9d099-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9d099-115">tvRating</span></span>|[<span data-ttu-id="9d099-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9d099-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="9d099-117">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="9d099-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="9d099-118">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="9d099-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d099-119">关系</span><span class="sxs-lookup"><span data-stu-id="9d099-119">Relationships</span></span>
<span data-ttu-id="9d099-120">无</span><span class="sxs-lookup"><span data-stu-id="9d099-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d099-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d099-121">JSON Representation</span></span>
<span data-ttu-id="9d099-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d099-122">Here is a JSON representation of the resource.</span></span>
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









