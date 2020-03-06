---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a08891428edd5fec07308e2ff7e44da49eaea93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530634"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="e5445-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5445-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="e5445-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5445-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5445-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5445-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5445-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e5445-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e5445-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5445-107">Properties</span></span>
|<span data-ttu-id="e5445-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5445-108">Property</span></span>|<span data-ttu-id="e5445-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5445-109">Type</span></span>|<span data-ttu-id="e5445-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5445-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5445-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e5445-111">movieRating</span></span>|[<span data-ttu-id="e5445-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="e5445-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="e5445-113">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e5445-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="e5445-114">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="e5445-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e5445-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e5445-115">tvRating</span></span>|[<span data-ttu-id="e5445-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e5445-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="e5445-117">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e5445-117">TV rating selected for Germany.</span></span> <span data-ttu-id="e5445-118">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e5445-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5445-119">关系</span><span class="sxs-lookup"><span data-stu-id="e5445-119">Relationships</span></span>
<span data-ttu-id="e5445-120">无</span><span class="sxs-lookup"><span data-stu-id="e5445-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5445-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5445-121">JSON Representation</span></span>
<span data-ttu-id="e5445-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5445-122">Here is a JSON representation of the resource.</span></span>
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




