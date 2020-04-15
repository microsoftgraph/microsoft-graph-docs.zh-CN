---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3adb081f2b18bbf38327cd56adf90f29333ec146
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439447"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="85f69-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="85f69-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="85f69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85f69-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85f69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85f69-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85f69-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="85f69-107">属性</span><span class="sxs-lookup"><span data-stu-id="85f69-107">Properties</span></span>
|<span data-ttu-id="85f69-108">属性</span><span class="sxs-lookup"><span data-stu-id="85f69-108">Property</span></span>|<span data-ttu-id="85f69-109">类型</span><span class="sxs-lookup"><span data-stu-id="85f69-109">Type</span></span>|<span data-ttu-id="85f69-110">说明</span><span class="sxs-lookup"><span data-stu-id="85f69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85f69-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="85f69-111">movieRating</span></span>|[<span data-ttu-id="85f69-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="85f69-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="85f69-113">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="85f69-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="85f69-114">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="85f69-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="85f69-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="85f69-115">tvRating</span></span>|[<span data-ttu-id="85f69-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="85f69-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="85f69-117">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="85f69-117">TV rating selected for Germany.</span></span> <span data-ttu-id="85f69-118">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="85f69-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85f69-119">关系</span><span class="sxs-lookup"><span data-stu-id="85f69-119">Relationships</span></span>
<span data-ttu-id="85f69-120">无</span><span class="sxs-lookup"><span data-stu-id="85f69-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85f69-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85f69-121">JSON Representation</span></span>
<span data-ttu-id="85f69-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85f69-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```







