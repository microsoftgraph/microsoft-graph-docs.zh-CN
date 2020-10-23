---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53ae5d7686bd8f9820c227441b34d898d4a9db4e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692462"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="c06e9-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="c06e9-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="c06e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c06e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c06e9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c06e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c06e9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c06e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c06e9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c06e9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c06e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="c06e9-108">Properties</span></span>
|<span data-ttu-id="c06e9-109">属性</span><span class="sxs-lookup"><span data-stu-id="c06e9-109">Property</span></span>|<span data-ttu-id="c06e9-110">类型</span><span class="sxs-lookup"><span data-stu-id="c06e9-110">Type</span></span>|<span data-ttu-id="c06e9-111">说明</span><span class="sxs-lookup"><span data-stu-id="c06e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c06e9-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c06e9-112">movieRating</span></span>|[<span data-ttu-id="c06e9-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="c06e9-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="c06e9-114">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="c06e9-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="c06e9-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c06e9-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c06e9-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c06e9-116">tvRating</span></span>|[<span data-ttu-id="c06e9-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c06e9-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="c06e9-118">为爱尔兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="c06e9-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="c06e9-119">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="c06e9-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c06e9-120">关系</span><span class="sxs-lookup"><span data-stu-id="c06e9-120">Relationships</span></span>
<span data-ttu-id="c06e9-121">无</span><span class="sxs-lookup"><span data-stu-id="c06e9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c06e9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c06e9-122">JSON Representation</span></span>
<span data-ttu-id="c06e9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c06e9-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```





