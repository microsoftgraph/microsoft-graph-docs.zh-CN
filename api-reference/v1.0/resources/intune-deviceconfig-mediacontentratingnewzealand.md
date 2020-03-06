---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 943a2d12ea1774bff6f12acd958b22f884cfa749
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532444"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="782f1-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="782f1-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="782f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="782f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="782f1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="782f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="782f1-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="782f1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="782f1-107">属性</span><span class="sxs-lookup"><span data-stu-id="782f1-107">Properties</span></span>
|<span data-ttu-id="782f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="782f1-108">Property</span></span>|<span data-ttu-id="782f1-109">类型</span><span class="sxs-lookup"><span data-stu-id="782f1-109">Type</span></span>|<span data-ttu-id="782f1-110">说明</span><span class="sxs-lookup"><span data-stu-id="782f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="782f1-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="782f1-111">movieRating</span></span>|[<span data-ttu-id="782f1-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="782f1-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="782f1-113">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="782f1-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="782f1-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="782f1-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="782f1-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="782f1-115">tvRating</span></span>|[<span data-ttu-id="782f1-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="782f1-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="782f1-117">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="782f1-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="782f1-118">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="782f1-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="782f1-119">关系</span><span class="sxs-lookup"><span data-stu-id="782f1-119">Relationships</span></span>
<span data-ttu-id="782f1-120">无</span><span class="sxs-lookup"><span data-stu-id="782f1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="782f1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="782f1-121">JSON Representation</span></span>
<span data-ttu-id="782f1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="782f1-122">Here is a JSON representation of the resource.</span></span>
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




