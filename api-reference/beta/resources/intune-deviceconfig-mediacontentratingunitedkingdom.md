---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48cf2b491b8dc2cb9ad5234c8285d82a64350aac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829209"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="e1121-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1121-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="e1121-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e1121-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1121-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1121-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1121-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1121-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1121-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e1121-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e1121-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1121-108">Properties</span></span>
|<span data-ttu-id="e1121-109">属性</span><span class="sxs-lookup"><span data-stu-id="e1121-109">Property</span></span>|<span data-ttu-id="e1121-110">类型</span><span class="sxs-lookup"><span data-stu-id="e1121-110">Type</span></span>|<span data-ttu-id="e1121-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1121-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1121-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e1121-112">movieRating</span></span>|[<span data-ttu-id="e1121-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="e1121-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="e1121-114">分级英国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="e1121-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="e1121-115">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e1121-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="e1121-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e1121-116">tvRating</span></span>|[<span data-ttu-id="e1121-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e1121-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="e1121-118">选定用于英国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="e1121-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="e1121-119">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="e1121-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1121-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="e1121-120">Relationships</span></span>
<span data-ttu-id="e1121-121">无</span><span class="sxs-lookup"><span data-stu-id="e1121-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1121-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1121-122">JSON Representation</span></span>
<span data-ttu-id="e1121-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1121-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```





