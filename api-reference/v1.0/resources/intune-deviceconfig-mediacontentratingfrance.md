---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44b6374d4831ca0b3b220f237a3c8d9938df18e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003141"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="16c8d-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="16c8d-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="16c8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16c8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16c8d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16c8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16c8d-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="16c8d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="16c8d-107">属性</span><span class="sxs-lookup"><span data-stu-id="16c8d-107">Properties</span></span>
|<span data-ttu-id="16c8d-108">属性</span><span class="sxs-lookup"><span data-stu-id="16c8d-108">Property</span></span>|<span data-ttu-id="16c8d-109">类型</span><span class="sxs-lookup"><span data-stu-id="16c8d-109">Type</span></span>|<span data-ttu-id="16c8d-110">说明</span><span class="sxs-lookup"><span data-stu-id="16c8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16c8d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="16c8d-111">movieRating</span></span>|[<span data-ttu-id="16c8d-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="16c8d-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="16c8d-113">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="16c8d-113">Movies rating selected for France.</span></span> <span data-ttu-id="16c8d-114">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="16c8d-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="16c8d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="16c8d-115">tvRating</span></span>|[<span data-ttu-id="16c8d-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="16c8d-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="16c8d-117">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="16c8d-117">TV rating selected for France.</span></span> <span data-ttu-id="16c8d-118">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="16c8d-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16c8d-119">关系</span><span class="sxs-lookup"><span data-stu-id="16c8d-119">Relationships</span></span>
<span data-ttu-id="16c8d-120">无</span><span class="sxs-lookup"><span data-stu-id="16c8d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16c8d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16c8d-121">JSON Representation</span></span>
<span data-ttu-id="16c8d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16c8d-122">Here is a JSON representation of the resource.</span></span>
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









