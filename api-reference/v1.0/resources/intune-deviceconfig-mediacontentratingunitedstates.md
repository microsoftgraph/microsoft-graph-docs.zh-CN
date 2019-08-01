---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6c6df674fc4cef174892d4cdb27303c3933fcdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031372"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="59429-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="59429-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="59429-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59429-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59429-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="59429-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="59429-106">属性</span><span class="sxs-lookup"><span data-stu-id="59429-106">Properties</span></span>
|<span data-ttu-id="59429-107">属性</span><span class="sxs-lookup"><span data-stu-id="59429-107">Property</span></span>|<span data-ttu-id="59429-108">类型</span><span class="sxs-lookup"><span data-stu-id="59429-108">Type</span></span>|<span data-ttu-id="59429-109">说明</span><span class="sxs-lookup"><span data-stu-id="59429-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59429-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="59429-110">movieRating</span></span>|[<span data-ttu-id="59429-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="59429-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="59429-112">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="59429-112">Movies rating selected for United States.</span></span> <span data-ttu-id="59429-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="59429-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="59429-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="59429-114">tvRating</span></span>|[<span data-ttu-id="59429-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="59429-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="59429-116">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="59429-116">TV rating selected for United States.</span></span> <span data-ttu-id="59429-117">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="59429-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59429-118">关系</span><span class="sxs-lookup"><span data-stu-id="59429-118">Relationships</span></span>
<span data-ttu-id="59429-119">无</span><span class="sxs-lookup"><span data-stu-id="59429-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59429-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59429-120">JSON Representation</span></span>
<span data-ttu-id="59429-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59429-121">Here is a JSON representation of the resource.</span></span>
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



