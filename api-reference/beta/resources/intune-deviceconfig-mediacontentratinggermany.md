---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f32a6ed59861dce47f5c38f7259b78879bf1681c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788581"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="eb31b-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb31b-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="eb31b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb31b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb31b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb31b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb31b-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eb31b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="eb31b-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb31b-107">Properties</span></span>
|<span data-ttu-id="eb31b-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb31b-108">Property</span></span>|<span data-ttu-id="eb31b-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb31b-109">Type</span></span>|<span data-ttu-id="eb31b-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb31b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb31b-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="eb31b-111">movieRating</span></span>|[<span data-ttu-id="eb31b-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="eb31b-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="eb31b-113">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="eb31b-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="eb31b-114">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="eb31b-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="eb31b-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="eb31b-115">tvRating</span></span>|[<span data-ttu-id="eb31b-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="eb31b-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="eb31b-117">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="eb31b-117">TV rating selected for Germany.</span></span> <span data-ttu-id="eb31b-118">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="eb31b-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb31b-119">关系</span><span class="sxs-lookup"><span data-stu-id="eb31b-119">Relationships</span></span>
<span data-ttu-id="eb31b-120">无</span><span class="sxs-lookup"><span data-stu-id="eb31b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb31b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb31b-121">JSON Representation</span></span>
<span data-ttu-id="eb31b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb31b-122">Here is a JSON representation of the resource.</span></span>
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



