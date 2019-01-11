---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 916257d83e28f3877773a6fcc7d7aefadab41af8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884222"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="fd3c9-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd3c9-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="fd3c9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd3c9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd3c9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd3c9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fd3c9-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fd3c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd3c9-108">Properties</span></span>
|<span data-ttu-id="fd3c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd3c9-109">Property</span></span>|<span data-ttu-id="fd3c9-110">类型</span><span class="sxs-lookup"><span data-stu-id="fd3c9-110">Type</span></span>|<span data-ttu-id="fd3c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd3c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd3c9-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="fd3c9-112">movieRating</span></span>|[<span data-ttu-id="fd3c9-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="fd3c9-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="fd3c9-114">分级澳大利亚的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="fd3c9-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="fd3c9-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="fd3c9-116">tvRating</span></span>|[<span data-ttu-id="fd3c9-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fd3c9-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="fd3c9-118">澳大利亚选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-118">TV rating selected for Australia.</span></span> <span data-ttu-id="fd3c9-119">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd3c9-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="fd3c9-120">Relationships</span></span>
<span data-ttu-id="fd3c9-121">无</span><span class="sxs-lookup"><span data-stu-id="fd3c9-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd3c9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd3c9-122">JSON Representation</span></span>
<span data-ttu-id="fd3c9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd3c9-123">Here is a JSON representation of the resource.</span></span>
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





