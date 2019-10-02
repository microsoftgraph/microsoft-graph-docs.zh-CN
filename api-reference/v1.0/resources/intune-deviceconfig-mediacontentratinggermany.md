---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3242ffabc3f0bdac7e013ad6ffec97f6dd49d2de
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359969"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="54885-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="54885-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="54885-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54885-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54885-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="54885-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="54885-106">属性</span><span class="sxs-lookup"><span data-stu-id="54885-106">Properties</span></span>
|<span data-ttu-id="54885-107">属性</span><span class="sxs-lookup"><span data-stu-id="54885-107">Property</span></span>|<span data-ttu-id="54885-108">类型</span><span class="sxs-lookup"><span data-stu-id="54885-108">Type</span></span>|<span data-ttu-id="54885-109">说明</span><span class="sxs-lookup"><span data-stu-id="54885-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54885-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="54885-110">movieRating</span></span>|[<span data-ttu-id="54885-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="54885-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="54885-112">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="54885-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="54885-113">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="54885-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="54885-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="54885-114">tvRating</span></span>|[<span data-ttu-id="54885-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="54885-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="54885-116">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="54885-116">TV rating selected for Germany.</span></span> <span data-ttu-id="54885-117">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="54885-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54885-118">关系</span><span class="sxs-lookup"><span data-stu-id="54885-118">Relationships</span></span>
<span data-ttu-id="54885-119">无</span><span class="sxs-lookup"><span data-stu-id="54885-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54885-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54885-120">JSON Representation</span></span>
<span data-ttu-id="54885-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54885-121">Here is a JSON representation of the resource.</span></span>
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




