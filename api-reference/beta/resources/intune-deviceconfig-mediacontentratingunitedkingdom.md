---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4ab6731bc486918815efe0d3f4c7f6f2638329d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953299"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="23bf1-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="23bf1-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="23bf1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="23bf1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23bf1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23bf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23bf1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="23bf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23bf1-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="23bf1-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="23bf1-108">属性</span><span class="sxs-lookup"><span data-stu-id="23bf1-108">Properties</span></span>
|<span data-ttu-id="23bf1-109">属性</span><span class="sxs-lookup"><span data-stu-id="23bf1-109">Property</span></span>|<span data-ttu-id="23bf1-110">类型</span><span class="sxs-lookup"><span data-stu-id="23bf1-110">Type</span></span>|<span data-ttu-id="23bf1-111">说明</span><span class="sxs-lookup"><span data-stu-id="23bf1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23bf1-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="23bf1-112">movieRating</span></span>|[<span data-ttu-id="23bf1-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="23bf1-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="23bf1-114">分级英国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="23bf1-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="23bf1-115">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="23bf1-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="23bf1-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="23bf1-116">tvRating</span></span>|[<span data-ttu-id="23bf1-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="23bf1-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="23bf1-118">选定用于英国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="23bf1-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="23bf1-119">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="23bf1-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23bf1-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="23bf1-120">Relationships</span></span>
<span data-ttu-id="23bf1-121">无</span><span class="sxs-lookup"><span data-stu-id="23bf1-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23bf1-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23bf1-122">JSON Representation</span></span>
<span data-ttu-id="23bf1-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23bf1-123">Here is a JSON representation of the resource.</span></span>
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





