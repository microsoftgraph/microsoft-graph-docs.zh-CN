---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d9887ee7d2375a9b954a7f62f84701b997d9b7a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473090"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="2ab34-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ab34-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="2ab34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ab34-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ab34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab34-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ab34-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2ab34-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ab34-107">Properties</span></span>
|<span data-ttu-id="2ab34-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ab34-108">Property</span></span>|<span data-ttu-id="2ab34-109">类型</span><span class="sxs-lookup"><span data-stu-id="2ab34-109">Type</span></span>|<span data-ttu-id="2ab34-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ab34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab34-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="2ab34-111">movieRating</span></span>|[<span data-ttu-id="2ab34-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="2ab34-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="2ab34-113">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="2ab34-113">Movies rating selected for United States.</span></span> <span data-ttu-id="2ab34-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="2ab34-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="2ab34-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="2ab34-115">tvRating</span></span>|[<span data-ttu-id="2ab34-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2ab34-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="2ab34-117">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="2ab34-117">TV rating selected for United States.</span></span> <span data-ttu-id="2ab34-118">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="2ab34-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab34-119">关系</span><span class="sxs-lookup"><span data-stu-id="2ab34-119">Relationships</span></span>
<span data-ttu-id="2ab34-120">无</span><span class="sxs-lookup"><span data-stu-id="2ab34-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ab34-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ab34-121">JSON Representation</span></span>
<span data-ttu-id="2ab34-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ab34-122">Here is a JSON representation of the resource.</span></span>
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







