---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9c1733ca3c541709d77dae0b1d6193a7b706c0cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879560"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="33036-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="33036-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="33036-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="33036-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33036-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="33036-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="33036-106">属性</span><span class="sxs-lookup"><span data-stu-id="33036-106">Properties</span></span>
|<span data-ttu-id="33036-107">属性</span><span class="sxs-lookup"><span data-stu-id="33036-107">Property</span></span>|<span data-ttu-id="33036-108">类型</span><span class="sxs-lookup"><span data-stu-id="33036-108">Type</span></span>|<span data-ttu-id="33036-109">说明</span><span class="sxs-lookup"><span data-stu-id="33036-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33036-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="33036-110">movieRating</span></span>|[<span data-ttu-id="33036-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="33036-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="33036-112">分级爱尔兰的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="33036-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="33036-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="33036-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="33036-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="33036-114">tvRating</span></span>|[<span data-ttu-id="33036-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="33036-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="33036-116">选择爱尔兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="33036-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="33036-117">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="33036-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33036-118">关系</span><span class="sxs-lookup"><span data-stu-id="33036-118">Relationships</span></span>
<span data-ttu-id="33036-119">无</span><span class="sxs-lookup"><span data-stu-id="33036-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33036-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33036-120">JSON Representation</span></span>
<span data-ttu-id="33036-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33036-121">Here is a JSON representation of the resource.</span></span>
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



