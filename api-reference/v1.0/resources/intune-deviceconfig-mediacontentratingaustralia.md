---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572372"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="3c0c6-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c0c6-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="3c0c6-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c0c6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c0c6-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c0c6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3c0c6-106">属性</span><span class="sxs-lookup"><span data-stu-id="3c0c6-106">Properties</span></span>
|<span data-ttu-id="3c0c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="3c0c6-107">Property</span></span>|<span data-ttu-id="3c0c6-108">类型</span><span class="sxs-lookup"><span data-stu-id="3c0c6-108">Type</span></span>|<span data-ttu-id="3c0c6-109">说明</span><span class="sxs-lookup"><span data-stu-id="3c0c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c0c6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="3c0c6-110">movieRating</span></span>|[<span data-ttu-id="3c0c6-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="3c0c6-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="3c0c6-112">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="3c0c6-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="3c0c6-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15` 或 `agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="3c0c6-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="3c0c6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="3c0c6-114">tvRating</span></span>|[<span data-ttu-id="3c0c6-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3c0c6-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="3c0c6-116">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="3c0c6-116">TV rating selected for Australia.</span></span> <span data-ttu-id="3c0c6-117">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="3c0c6-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c0c6-118">关系</span><span class="sxs-lookup"><span data-stu-id="3c0c6-118">Relationships</span></span>
<span data-ttu-id="3c0c6-119">无</span><span class="sxs-lookup"><span data-stu-id="3c0c6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c0c6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c0c6-120">JSON Representation</span></span>
<span data-ttu-id="3c0c6-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c0c6-121">Here is a JSON representation of the resource.</span></span>
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



