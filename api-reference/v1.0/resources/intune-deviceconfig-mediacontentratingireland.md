---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01135bb6c5a19ae837a834a51a5857b5f54baac0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473158"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="26633-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="26633-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="26633-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26633-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26633-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26633-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26633-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26633-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="26633-107">属性</span><span class="sxs-lookup"><span data-stu-id="26633-107">Properties</span></span>
|<span data-ttu-id="26633-108">属性</span><span class="sxs-lookup"><span data-stu-id="26633-108">Property</span></span>|<span data-ttu-id="26633-109">类型</span><span class="sxs-lookup"><span data-stu-id="26633-109">Type</span></span>|<span data-ttu-id="26633-110">说明</span><span class="sxs-lookup"><span data-stu-id="26633-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26633-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="26633-111">movieRating</span></span>|[<span data-ttu-id="26633-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="26633-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="26633-113">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="26633-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="26633-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="26633-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="26633-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="26633-115">tvRating</span></span>|[<span data-ttu-id="26633-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="26633-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="26633-117">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="26633-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="26633-118">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="26633-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26633-119">关系</span><span class="sxs-lookup"><span data-stu-id="26633-119">Relationships</span></span>
<span data-ttu-id="26633-120">无</span><span class="sxs-lookup"><span data-stu-id="26633-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26633-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26633-121">JSON Representation</span></span>
<span data-ttu-id="26633-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26633-122">Here is a JSON representation of the resource.</span></span>
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







