---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 724fe7a511616b457d29cd804c19d69705bfb42b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757771"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="d8b73-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8b73-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="d8b73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8b73-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8b73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8b73-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d8b73-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d8b73-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8b73-107">Properties</span></span>
|<span data-ttu-id="d8b73-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8b73-108">Property</span></span>|<span data-ttu-id="d8b73-109">类型</span><span class="sxs-lookup"><span data-stu-id="d8b73-109">Type</span></span>|<span data-ttu-id="d8b73-110">Description</span><span class="sxs-lookup"><span data-stu-id="d8b73-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b73-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="d8b73-111">movieRating</span></span>|[<span data-ttu-id="d8b73-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="d8b73-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="d8b73-113">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="d8b73-113">Movies rating selected for France.</span></span> <span data-ttu-id="d8b73-114">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d8b73-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d8b73-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="d8b73-115">tvRating</span></span>|[<span data-ttu-id="d8b73-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d8b73-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="d8b73-117">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="d8b73-117">TV rating selected for France.</span></span> <span data-ttu-id="d8b73-118">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d8b73-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8b73-119">关系</span><span class="sxs-lookup"><span data-stu-id="d8b73-119">Relationships</span></span>
<span data-ttu-id="d8b73-120">无</span><span class="sxs-lookup"><span data-stu-id="d8b73-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8b73-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8b73-121">JSON Representation</span></span>
<span data-ttu-id="d8b73-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8b73-122">Here is a JSON representation of the resource.</span></span>
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




