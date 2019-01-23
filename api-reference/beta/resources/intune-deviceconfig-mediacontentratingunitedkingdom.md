---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d21ac4650072c4523f9e120d5d73ad393686635
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408073"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="67783-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="67783-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="67783-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="67783-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67783-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67783-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67783-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67783-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67783-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="67783-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="67783-108">属性</span><span class="sxs-lookup"><span data-stu-id="67783-108">Properties</span></span>
|<span data-ttu-id="67783-109">属性</span><span class="sxs-lookup"><span data-stu-id="67783-109">Property</span></span>|<span data-ttu-id="67783-110">类型</span><span class="sxs-lookup"><span data-stu-id="67783-110">Type</span></span>|<span data-ttu-id="67783-111">说明</span><span class="sxs-lookup"><span data-stu-id="67783-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67783-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="67783-112">movieRating</span></span>|[<span data-ttu-id="67783-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="67783-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="67783-114">分级英国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="67783-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="67783-115">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="67783-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="67783-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="67783-116">tvRating</span></span>|[<span data-ttu-id="67783-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="67783-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="67783-118">选定用于英国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="67783-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="67783-119">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="67783-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67783-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="67783-120">Relationships</span></span>
<span data-ttu-id="67783-121">无</span><span class="sxs-lookup"><span data-stu-id="67783-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67783-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67783-122">JSON Representation</span></span>
<span data-ttu-id="67783-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67783-123">Here is a JSON representation of the resource.</span></span>
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




