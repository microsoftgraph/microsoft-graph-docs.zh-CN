---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb1cfcafca5b369d8c68103be0795c54842d083f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742872"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="e54c5-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="e54c5-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="e54c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e54c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e54c5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e54c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e54c5-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e54c5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e54c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="e54c5-107">Properties</span></span>
|<span data-ttu-id="e54c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="e54c5-108">Property</span></span>|<span data-ttu-id="e54c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="e54c5-109">Type</span></span>|<span data-ttu-id="e54c5-110">Description</span><span class="sxs-lookup"><span data-stu-id="e54c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e54c5-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e54c5-111">movieRating</span></span>|[<span data-ttu-id="e54c5-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="e54c5-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="e54c5-113">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e54c5-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="e54c5-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15` 或 `agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="e54c5-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e54c5-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e54c5-115">tvRating</span></span>|[<span data-ttu-id="e54c5-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e54c5-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="e54c5-117">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e54c5-117">TV rating selected for Australia.</span></span> <span data-ttu-id="e54c5-118">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="e54c5-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e54c5-119">关系</span><span class="sxs-lookup"><span data-stu-id="e54c5-119">Relationships</span></span>
<span data-ttu-id="e54c5-120">无</span><span class="sxs-lookup"><span data-stu-id="e54c5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e54c5-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e54c5-121">JSON Representation</span></span>
<span data-ttu-id="e54c5-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e54c5-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




