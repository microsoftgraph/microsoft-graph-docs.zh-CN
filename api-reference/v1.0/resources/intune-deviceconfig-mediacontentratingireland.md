---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb96a239ff31a0d6843b690d063361a65099e65e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760020"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="c820d-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="c820d-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="c820d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c820d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c820d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c820d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c820d-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c820d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c820d-107">属性</span><span class="sxs-lookup"><span data-stu-id="c820d-107">Properties</span></span>
|<span data-ttu-id="c820d-108">属性</span><span class="sxs-lookup"><span data-stu-id="c820d-108">Property</span></span>|<span data-ttu-id="c820d-109">类型</span><span class="sxs-lookup"><span data-stu-id="c820d-109">Type</span></span>|<span data-ttu-id="c820d-110">说明</span><span class="sxs-lookup"><span data-stu-id="c820d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c820d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c820d-111">movieRating</span></span>|[<span data-ttu-id="c820d-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="c820d-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="c820d-113">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="c820d-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="c820d-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c820d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c820d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c820d-115">tvRating</span></span>|[<span data-ttu-id="c820d-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c820d-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="c820d-117">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="c820d-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="c820d-118">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="c820d-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c820d-119">关系</span><span class="sxs-lookup"><span data-stu-id="c820d-119">Relationships</span></span>
<span data-ttu-id="c820d-120">无</span><span class="sxs-lookup"><span data-stu-id="c820d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c820d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c820d-121">JSON Representation</span></span>
<span data-ttu-id="c820d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c820d-122">Here is a JSON representation of the resource.</span></span>
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




