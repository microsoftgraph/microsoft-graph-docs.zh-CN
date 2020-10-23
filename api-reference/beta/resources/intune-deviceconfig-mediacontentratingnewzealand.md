---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cad2826c4b3197a7d0ccba850fa1bf14464daf2c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707169"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="1f192-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f192-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="1f192-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f192-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f192-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f192-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f192-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f192-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f192-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1f192-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1f192-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f192-108">Properties</span></span>
|<span data-ttu-id="1f192-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f192-109">Property</span></span>|<span data-ttu-id="1f192-110">类型</span><span class="sxs-lookup"><span data-stu-id="1f192-110">Type</span></span>|<span data-ttu-id="1f192-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f192-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f192-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="1f192-112">movieRating</span></span>|[<span data-ttu-id="1f192-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="1f192-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="1f192-114">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="1f192-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="1f192-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="1f192-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="1f192-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="1f192-116">tvRating</span></span>|[<span data-ttu-id="1f192-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1f192-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="1f192-118">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="1f192-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="1f192-119">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="1f192-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f192-120">关系</span><span class="sxs-lookup"><span data-stu-id="1f192-120">Relationships</span></span>
<span data-ttu-id="1f192-121">无</span><span class="sxs-lookup"><span data-stu-id="1f192-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f192-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f192-122">JSON Representation</span></span>
<span data-ttu-id="1f192-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f192-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





