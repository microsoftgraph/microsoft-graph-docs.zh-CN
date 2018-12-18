---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 6ade4ea9d5f2236803a8515b94ebc57f32ce3cd7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337490"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="0a990-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a990-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="0a990-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a990-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a990-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a990-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a990-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0a990-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a990-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a990-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0a990-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a990-108">Properties</span></span>
|<span data-ttu-id="0a990-109">属性</span><span class="sxs-lookup"><span data-stu-id="0a990-109">Property</span></span>|<span data-ttu-id="0a990-110">类型</span><span class="sxs-lookup"><span data-stu-id="0a990-110">Type</span></span>|<span data-ttu-id="0a990-111">说明</span><span class="sxs-lookup"><span data-stu-id="0a990-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a990-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0a990-112">movieRating</span></span>|[<span data-ttu-id="0a990-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="0a990-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="0a990-114">分级爱尔兰的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="0a990-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="0a990-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="0a990-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="0a990-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0a990-116">tvRating</span></span>|[<span data-ttu-id="0a990-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0a990-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="0a990-118">选择爱尔兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="0a990-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="0a990-119">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="0a990-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a990-120">关系</span><span class="sxs-lookup"><span data-stu-id="0a990-120">Relationships</span></span>
<span data-ttu-id="0a990-121">无</span><span class="sxs-lookup"><span data-stu-id="0a990-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a990-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a990-122">JSON Representation</span></span>
<span data-ttu-id="0a990-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a990-123">Here is a JSON representation of the resource.</span></span>
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





