---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d7b4efd96b766eef9104baaa694d166eb22df340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530618"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="bc749-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc749-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="bc749-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc749-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc749-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc749-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc749-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc749-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bc749-107">属性</span><span class="sxs-lookup"><span data-stu-id="bc749-107">Properties</span></span>
|<span data-ttu-id="bc749-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc749-108">Property</span></span>|<span data-ttu-id="bc749-109">类型</span><span class="sxs-lookup"><span data-stu-id="bc749-109">Type</span></span>|<span data-ttu-id="bc749-110">说明</span><span class="sxs-lookup"><span data-stu-id="bc749-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc749-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="bc749-111">movieRating</span></span>|[<span data-ttu-id="bc749-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="bc749-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="bc749-113">为日本选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="bc749-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="bc749-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="bc749-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="bc749-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="bc749-115">tvRating</span></span>|[<span data-ttu-id="bc749-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bc749-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="bc749-117">为日本选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="bc749-117">TV rating selected for Japan.</span></span> <span data-ttu-id="bc749-118">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="bc749-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc749-119">关系</span><span class="sxs-lookup"><span data-stu-id="bc749-119">Relationships</span></span>
<span data-ttu-id="bc749-120">无</span><span class="sxs-lookup"><span data-stu-id="bc749-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc749-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc749-121">JSON Representation</span></span>
<span data-ttu-id="bc749-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc749-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```




