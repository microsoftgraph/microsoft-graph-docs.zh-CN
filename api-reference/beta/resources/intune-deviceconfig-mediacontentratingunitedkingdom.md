---
title: mediaContentRatingUnitedKingdom 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9173aec94ce24056fd8d6c7efffcf144509c5ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273443"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="e55b8-103">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="e55b8-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="e55b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e55b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e55b8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e55b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e55b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e55b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e55b8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e55b8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e55b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="e55b8-108">Properties</span></span>
|<span data-ttu-id="e55b8-109">属性</span><span class="sxs-lookup"><span data-stu-id="e55b8-109">Property</span></span>|<span data-ttu-id="e55b8-110">类型</span><span class="sxs-lookup"><span data-stu-id="e55b8-110">Type</span></span>|<span data-ttu-id="e55b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="e55b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e55b8-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e55b8-112">movieRating</span></span>|[<span data-ttu-id="e55b8-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="e55b8-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="e55b8-114">为英国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="e55b8-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="e55b8-115">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e55b8-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="e55b8-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e55b8-116">tvRating</span></span>|[<span data-ttu-id="e55b8-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e55b8-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="e55b8-118">为英国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="e55b8-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="e55b8-119">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="e55b8-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e55b8-120">关系</span><span class="sxs-lookup"><span data-stu-id="e55b8-120">Relationships</span></span>
<span data-ttu-id="e55b8-121">无</span><span class="sxs-lookup"><span data-stu-id="e55b8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e55b8-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e55b8-122">JSON Representation</span></span>
<span data-ttu-id="e55b8-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e55b8-123">Here is a JSON representation of the resource.</span></span>
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




