---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06cad29f595ecc1124344d2ad72bed50a71b4314
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757764"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="2933e-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="2933e-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="2933e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2933e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2933e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2933e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2933e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2933e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2933e-107">属性</span><span class="sxs-lookup"><span data-stu-id="2933e-107">Properties</span></span>
|<span data-ttu-id="2933e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2933e-108">Property</span></span>|<span data-ttu-id="2933e-109">类型</span><span class="sxs-lookup"><span data-stu-id="2933e-109">Type</span></span>|<span data-ttu-id="2933e-110">Description</span><span class="sxs-lookup"><span data-stu-id="2933e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2933e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="2933e-111">movieRating</span></span>|[<span data-ttu-id="2933e-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="2933e-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="2933e-113">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="2933e-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="2933e-114">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="2933e-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="2933e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="2933e-115">tvRating</span></span>|[<span data-ttu-id="2933e-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2933e-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="2933e-117">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="2933e-117">TV rating selected for Germany.</span></span> <span data-ttu-id="2933e-118">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="2933e-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2933e-119">关系</span><span class="sxs-lookup"><span data-stu-id="2933e-119">Relationships</span></span>
<span data-ttu-id="2933e-120">无</span><span class="sxs-lookup"><span data-stu-id="2933e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2933e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2933e-121">JSON Representation</span></span>
<span data-ttu-id="2933e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2933e-122">Here is a JSON representation of the resource.</span></span>
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




