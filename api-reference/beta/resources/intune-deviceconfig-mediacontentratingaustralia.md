---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ee5d9bb60ac7b8b2e096f05480dc8764f448b06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010176"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="dd0c3-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd0c3-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="dd0c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd0c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd0c3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd0c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd0c3-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dd0c3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dd0c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd0c3-108">Properties</span></span>
|<span data-ttu-id="dd0c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="dd0c3-109">Property</span></span>|<span data-ttu-id="dd0c3-110">类型</span><span class="sxs-lookup"><span data-stu-id="dd0c3-110">Type</span></span>|<span data-ttu-id="dd0c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="dd0c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd0c3-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="dd0c3-112">movieRating</span></span>|[<span data-ttu-id="dd0c3-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="dd0c3-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="dd0c3-114">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="dd0c3-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15` 或 `agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="dd0c3-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="dd0c3-116">tvRating</span></span>|[<span data-ttu-id="dd0c3-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="dd0c3-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="dd0c3-118">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-118">TV rating selected for Australia.</span></span> <span data-ttu-id="dd0c3-119">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd0c3-120">关系</span><span class="sxs-lookup"><span data-stu-id="dd0c3-120">Relationships</span></span>
<span data-ttu-id="dd0c3-121">无</span><span class="sxs-lookup"><span data-stu-id="dd0c3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd0c3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd0c3-122">JSON Representation</span></span>
<span data-ttu-id="dd0c3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd0c3-123">Here is a JSON representation of the resource.</span></span>
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






