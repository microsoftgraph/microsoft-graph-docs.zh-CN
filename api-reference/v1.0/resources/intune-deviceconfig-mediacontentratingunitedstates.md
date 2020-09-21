---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30e41727b84e7f10b82917f4dc1dd23f296cc19f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003057"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="e04ba-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="e04ba-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="e04ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e04ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e04ba-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e04ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e04ba-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e04ba-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e04ba-107">属性</span><span class="sxs-lookup"><span data-stu-id="e04ba-107">Properties</span></span>
|<span data-ttu-id="e04ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="e04ba-108">Property</span></span>|<span data-ttu-id="e04ba-109">类型</span><span class="sxs-lookup"><span data-stu-id="e04ba-109">Type</span></span>|<span data-ttu-id="e04ba-110">说明</span><span class="sxs-lookup"><span data-stu-id="e04ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e04ba-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e04ba-111">movieRating</span></span>|[<span data-ttu-id="e04ba-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="e04ba-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="e04ba-113">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e04ba-113">Movies rating selected for United States.</span></span> <span data-ttu-id="e04ba-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="e04ba-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="e04ba-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e04ba-115">tvRating</span></span>|[<span data-ttu-id="e04ba-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e04ba-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="e04ba-117">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e04ba-117">TV rating selected for United States.</span></span> <span data-ttu-id="e04ba-118">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e04ba-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e04ba-119">关系</span><span class="sxs-lookup"><span data-stu-id="e04ba-119">Relationships</span></span>
<span data-ttu-id="e04ba-120">无</span><span class="sxs-lookup"><span data-stu-id="e04ba-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e04ba-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e04ba-121">JSON Representation</span></span>
<span data-ttu-id="e04ba-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e04ba-122">Here is a JSON representation of the resource.</span></span>
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









