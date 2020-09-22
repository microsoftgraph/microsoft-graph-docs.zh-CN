---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2860f308cb25b679ea12b2b2d978cf15dc87c40a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003092"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="8cd19-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cd19-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="8cd19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cd19-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8cd19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cd19-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8cd19-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8cd19-107">属性</span><span class="sxs-lookup"><span data-stu-id="8cd19-107">Properties</span></span>
|<span data-ttu-id="8cd19-108">属性</span><span class="sxs-lookup"><span data-stu-id="8cd19-108">Property</span></span>|<span data-ttu-id="8cd19-109">类型</span><span class="sxs-lookup"><span data-stu-id="8cd19-109">Type</span></span>|<span data-ttu-id="8cd19-110">说明</span><span class="sxs-lookup"><span data-stu-id="8cd19-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cd19-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="8cd19-111">movieRating</span></span>|[<span data-ttu-id="8cd19-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="8cd19-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="8cd19-113">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="8cd19-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="8cd19-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="8cd19-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="8cd19-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="8cd19-115">tvRating</span></span>|[<span data-ttu-id="8cd19-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8cd19-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="8cd19-117">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="8cd19-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="8cd19-118">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="8cd19-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cd19-119">关系</span><span class="sxs-lookup"><span data-stu-id="8cd19-119">Relationships</span></span>
<span data-ttu-id="8cd19-120">无</span><span class="sxs-lookup"><span data-stu-id="8cd19-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cd19-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cd19-121">JSON Representation</span></span>
<span data-ttu-id="8cd19-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cd19-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```









