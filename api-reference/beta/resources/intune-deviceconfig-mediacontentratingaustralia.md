---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae1cb934af017c751ae2bcf05cd992668a452ed6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166764"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="4e723-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e723-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="4e723-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e723-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e723-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e723-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e723-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4e723-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4e723-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e723-107">Properties</span></span>
|<span data-ttu-id="4e723-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e723-108">Property</span></span>|<span data-ttu-id="4e723-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e723-109">Type</span></span>|<span data-ttu-id="4e723-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e723-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e723-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="4e723-111">movieRating</span></span>|[<span data-ttu-id="4e723-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4e723-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="4e723-113">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="4e723-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="4e723-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="4e723-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="4e723-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="4e723-115">tvRating</span></span>|[<span data-ttu-id="4e723-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4e723-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="4e723-117">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="4e723-117">TV rating selected for Australia.</span></span> <span data-ttu-id="4e723-118">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="4e723-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e723-119">关系</span><span class="sxs-lookup"><span data-stu-id="4e723-119">Relationships</span></span>
<span data-ttu-id="4e723-120">无</span><span class="sxs-lookup"><span data-stu-id="4e723-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e723-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e723-121">JSON Representation</span></span>
<span data-ttu-id="4e723-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e723-122">Here is a JSON representation of the resource.</span></span>
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




