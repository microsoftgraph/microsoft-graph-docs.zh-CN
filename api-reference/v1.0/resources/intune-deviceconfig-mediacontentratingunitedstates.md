---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0175f6f0894df0c859f9951f43c3bb4b857a2256
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760006"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="51d84-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="51d84-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="51d84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51d84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51d84-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51d84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51d84-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51d84-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="51d84-107">属性</span><span class="sxs-lookup"><span data-stu-id="51d84-107">Properties</span></span>
|<span data-ttu-id="51d84-108">属性</span><span class="sxs-lookup"><span data-stu-id="51d84-108">Property</span></span>|<span data-ttu-id="51d84-109">类型</span><span class="sxs-lookup"><span data-stu-id="51d84-109">Type</span></span>|<span data-ttu-id="51d84-110">说明</span><span class="sxs-lookup"><span data-stu-id="51d84-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51d84-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="51d84-111">movieRating</span></span>|[<span data-ttu-id="51d84-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="51d84-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="51d84-113">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="51d84-113">Movies rating selected for United States.</span></span> <span data-ttu-id="51d84-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="51d84-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="51d84-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="51d84-115">tvRating</span></span>|[<span data-ttu-id="51d84-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="51d84-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="51d84-117">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="51d84-117">TV rating selected for United States.</span></span> <span data-ttu-id="51d84-118">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="51d84-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51d84-119">关系</span><span class="sxs-lookup"><span data-stu-id="51d84-119">Relationships</span></span>
<span data-ttu-id="51d84-120">无</span><span class="sxs-lookup"><span data-stu-id="51d84-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51d84-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51d84-121">JSON Representation</span></span>
<span data-ttu-id="51d84-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51d84-122">Here is a JSON representation of the resource.</span></span>
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




