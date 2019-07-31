---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ea4656e24afe5d78bac2b4a69f51c145de2708d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970085"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="4b787-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b787-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="4b787-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b787-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b787-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b787-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b787-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4b787-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4b787-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b787-107">Properties</span></span>
|<span data-ttu-id="4b787-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b787-108">Property</span></span>|<span data-ttu-id="4b787-109">类型</span><span class="sxs-lookup"><span data-stu-id="4b787-109">Type</span></span>|<span data-ttu-id="4b787-110">说明</span><span class="sxs-lookup"><span data-stu-id="4b787-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b787-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="4b787-111">movieRating</span></span>|[<span data-ttu-id="4b787-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="4b787-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="4b787-113">为新西兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="4b787-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="4b787-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="4b787-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="4b787-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="4b787-115">tvRating</span></span>|[<span data-ttu-id="4b787-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4b787-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="4b787-117">为新西兰选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="4b787-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="4b787-118">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="4b787-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b787-119">关系</span><span class="sxs-lookup"><span data-stu-id="4b787-119">Relationships</span></span>
<span data-ttu-id="4b787-120">无</span><span class="sxs-lookup"><span data-stu-id="4b787-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b787-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b787-121">JSON Representation</span></span>
<span data-ttu-id="4b787-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b787-122">Here is a JSON representation of the resource.</span></span>
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





