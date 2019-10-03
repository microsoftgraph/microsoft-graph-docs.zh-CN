---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee961024a526300b1bbf7ebb186df69ce0337f78
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366585"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="1b9f2-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b9f2-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="1b9f2-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b9f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b9f2-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b9f2-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1b9f2-106">属性</span><span class="sxs-lookup"><span data-stu-id="1b9f2-106">Properties</span></span>
|<span data-ttu-id="1b9f2-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b9f2-107">Property</span></span>|<span data-ttu-id="1b9f2-108">类型</span><span class="sxs-lookup"><span data-stu-id="1b9f2-108">Type</span></span>|<span data-ttu-id="1b9f2-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b9f2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b9f2-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1b9f2-110">movieRating</span></span>|[<span data-ttu-id="1b9f2-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="1b9f2-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="1b9f2-112">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="1b9f2-112">Movies rating selected for United States.</span></span> <span data-ttu-id="1b9f2-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="1b9f2-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="1b9f2-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1b9f2-114">tvRating</span></span>|[<span data-ttu-id="1b9f2-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1b9f2-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="1b9f2-116">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="1b9f2-116">TV rating selected for United States.</span></span> <span data-ttu-id="1b9f2-117">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="1b9f2-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b9f2-118">关系</span><span class="sxs-lookup"><span data-stu-id="1b9f2-118">Relationships</span></span>
<span data-ttu-id="1b9f2-119">无</span><span class="sxs-lookup"><span data-stu-id="1b9f2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b9f2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b9f2-120">JSON Representation</span></span>
<span data-ttu-id="1b9f2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b9f2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```




