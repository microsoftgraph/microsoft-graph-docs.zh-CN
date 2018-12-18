---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 0fcd17f27d999f933ce6824f8a49018013341c7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315531"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="b9025-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9025-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="b9025-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b9025-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9025-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b9025-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b9025-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9025-106">Properties</span></span>
|<span data-ttu-id="b9025-107">属性</span><span class="sxs-lookup"><span data-stu-id="b9025-107">Property</span></span>|<span data-ttu-id="b9025-108">类型</span><span class="sxs-lookup"><span data-stu-id="b9025-108">Type</span></span>|<span data-ttu-id="b9025-109">说明</span><span class="sxs-lookup"><span data-stu-id="b9025-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9025-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b9025-110">movieRating</span></span>|[<span data-ttu-id="b9025-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="b9025-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="b9025-112">分级英国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="b9025-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="b9025-113">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="b9025-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="b9025-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b9025-114">tvRating</span></span>|[<span data-ttu-id="b9025-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b9025-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="b9025-116">选定用于英国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="b9025-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="b9025-117">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="b9025-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9025-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="b9025-118">Relationships</span></span>
<span data-ttu-id="b9025-119">无</span><span class="sxs-lookup"><span data-stu-id="b9025-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9025-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9025-120">JSON Representation</span></span>
<span data-ttu-id="b9025-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9025-121">Here is a JSON representation of the resource.</span></span>
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



