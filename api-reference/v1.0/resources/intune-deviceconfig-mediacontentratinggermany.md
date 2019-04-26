---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572379"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="9ac7d-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ac7d-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="9ac7d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ac7d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac7d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ac7d-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9ac7d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ac7d-106">Properties</span></span>
|<span data-ttu-id="9ac7d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ac7d-107">Property</span></span>|<span data-ttu-id="9ac7d-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ac7d-108">Type</span></span>|<span data-ttu-id="9ac7d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ac7d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac7d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9ac7d-110">movieRating</span></span>|[<span data-ttu-id="9ac7d-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="9ac7d-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="9ac7d-112">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="9ac7d-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="9ac7d-113">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="9ac7d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="9ac7d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9ac7d-114">tvRating</span></span>|[<span data-ttu-id="9ac7d-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9ac7d-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="9ac7d-116">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="9ac7d-116">TV rating selected for Germany.</span></span> <span data-ttu-id="9ac7d-117">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="9ac7d-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac7d-118">关系</span><span class="sxs-lookup"><span data-stu-id="9ac7d-118">Relationships</span></span>
<span data-ttu-id="9ac7d-119">无</span><span class="sxs-lookup"><span data-stu-id="9ac7d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ac7d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ac7d-120">JSON Representation</span></span>
<span data-ttu-id="9ac7d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ac7d-121">Here is a JSON representation of the resource.</span></span>
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



