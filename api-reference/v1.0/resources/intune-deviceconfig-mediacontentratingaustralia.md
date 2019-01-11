---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0860a17671b2923c2be9b5b469f93d443e808f53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891481"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="4b557-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b557-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="4b557-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4b557-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b557-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4b557-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4b557-106">属性</span><span class="sxs-lookup"><span data-stu-id="4b557-106">Properties</span></span>
|<span data-ttu-id="4b557-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b557-107">Property</span></span>|<span data-ttu-id="4b557-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b557-108">Type</span></span>|<span data-ttu-id="4b557-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b557-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b557-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="4b557-110">movieRating</span></span>|[<span data-ttu-id="4b557-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4b557-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="4b557-112">分级澳大利亚的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="4b557-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="4b557-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="4b557-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="4b557-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="4b557-114">tvRating</span></span>|[<span data-ttu-id="4b557-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4b557-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="4b557-116">澳大利亚选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="4b557-116">TV rating selected for Australia.</span></span> <span data-ttu-id="4b557-117">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="4b557-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b557-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="4b557-118">Relationships</span></span>
<span data-ttu-id="4b557-119">无</span><span class="sxs-lookup"><span data-stu-id="4b557-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b557-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b557-120">JSON Representation</span></span>
<span data-ttu-id="4b557-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b557-121">Here is a JSON representation of the resource.</span></span>
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



