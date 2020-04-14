---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e146adc4b2d2e550701a6f152efcdefb41758644
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437213"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="91fce-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="91fce-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="91fce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91fce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91fce-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91fce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91fce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91fce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91fce-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="91fce-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="91fce-108">属性</span><span class="sxs-lookup"><span data-stu-id="91fce-108">Properties</span></span>
|<span data-ttu-id="91fce-109">属性</span><span class="sxs-lookup"><span data-stu-id="91fce-109">Property</span></span>|<span data-ttu-id="91fce-110">类型</span><span class="sxs-lookup"><span data-stu-id="91fce-110">Type</span></span>|<span data-ttu-id="91fce-111">说明</span><span class="sxs-lookup"><span data-stu-id="91fce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91fce-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="91fce-112">movieRating</span></span>|[<span data-ttu-id="91fce-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="91fce-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="91fce-114">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="91fce-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="91fce-115">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="91fce-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="91fce-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="91fce-116">tvRating</span></span>|[<span data-ttu-id="91fce-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="91fce-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="91fce-118">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="91fce-118">TV rating selected for Germany.</span></span> <span data-ttu-id="91fce-119">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="91fce-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91fce-120">关系</span><span class="sxs-lookup"><span data-stu-id="91fce-120">Relationships</span></span>
<span data-ttu-id="91fce-121">无</span><span class="sxs-lookup"><span data-stu-id="91fce-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91fce-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91fce-122">JSON Representation</span></span>
<span data-ttu-id="91fce-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91fce-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



