---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84f54697d5c6a05f03c28b70e7d6250fa5dd0e46
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360018"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="4d947-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d947-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="4d947-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d947-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d947-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4d947-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4d947-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d947-106">Properties</span></span>
|<span data-ttu-id="4d947-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d947-107">Property</span></span>|<span data-ttu-id="4d947-108">类型</span><span class="sxs-lookup"><span data-stu-id="4d947-108">Type</span></span>|<span data-ttu-id="4d947-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d947-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d947-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="4d947-110">movieRating</span></span>|[<span data-ttu-id="4d947-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4d947-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="4d947-112">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="4d947-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="4d947-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="4d947-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="4d947-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="4d947-114">tvRating</span></span>|[<span data-ttu-id="4d947-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4d947-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="4d947-116">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="4d947-116">TV rating selected for Canada.</span></span> <span data-ttu-id="4d947-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="4d947-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d947-118">关系</span><span class="sxs-lookup"><span data-stu-id="4d947-118">Relationships</span></span>
<span data-ttu-id="4d947-119">无</span><span class="sxs-lookup"><span data-stu-id="4d947-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d947-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d947-120">JSON Representation</span></span>
<span data-ttu-id="4d947-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d947-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```




