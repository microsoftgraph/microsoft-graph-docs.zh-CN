---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9735497f3f2f71f28b8fe9847d2664bd4e65e959
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028110"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="e6a89-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6a89-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="e6a89-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6a89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6a89-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6a89-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e6a89-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6a89-106">Properties</span></span>
|<span data-ttu-id="e6a89-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6a89-107">Property</span></span>|<span data-ttu-id="e6a89-108">类型</span><span class="sxs-lookup"><span data-stu-id="e6a89-108">Type</span></span>|<span data-ttu-id="e6a89-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6a89-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6a89-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e6a89-110">movieRating</span></span>|[<span data-ttu-id="e6a89-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="e6a89-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="e6a89-112">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e6a89-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="e6a89-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="e6a89-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="e6a89-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e6a89-114">tvRating</span></span>|[<span data-ttu-id="e6a89-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e6a89-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="e6a89-116">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e6a89-116">TV rating selected for Canada.</span></span> <span data-ttu-id="e6a89-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="e6a89-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6a89-118">关系</span><span class="sxs-lookup"><span data-stu-id="e6a89-118">Relationships</span></span>
<span data-ttu-id="e6a89-119">无</span><span class="sxs-lookup"><span data-stu-id="e6a89-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6a89-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6a89-120">JSON Representation</span></span>
<span data-ttu-id="e6a89-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6a89-121">Here is a JSON representation of the resource.</span></span>
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



