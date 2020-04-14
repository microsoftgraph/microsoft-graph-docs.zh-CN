---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 878aa40d55f9c902e8f243d4839ea62cecfe1809
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437242"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b3cb0-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3cb0-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="b3cb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3cb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3cb0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3cb0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3cb0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3cb0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b3cb0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3cb0-108">Properties</span></span>
|<span data-ttu-id="b3cb0-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3cb0-109">Property</span></span>|<span data-ttu-id="b3cb0-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3cb0-110">Type</span></span>|<span data-ttu-id="b3cb0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3cb0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3cb0-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b3cb0-112">movieRating</span></span>|[<span data-ttu-id="b3cb0-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b3cb0-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b3cb0-114">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="b3cb0-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15` 或 `agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b3cb0-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b3cb0-116">tvRating</span></span>|[<span data-ttu-id="b3cb0-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b3cb0-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b3cb0-118">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-118">TV rating selected for Australia.</span></span> <span data-ttu-id="b3cb0-119">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3cb0-120">关系</span><span class="sxs-lookup"><span data-stu-id="b3cb0-120">Relationships</span></span>
<span data-ttu-id="b3cb0-121">无</span><span class="sxs-lookup"><span data-stu-id="b3cb0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3cb0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3cb0-122">JSON Representation</span></span>
<span data-ttu-id="b3cb0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3cb0-123">Here is a JSON representation of the resource.</span></span>
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



