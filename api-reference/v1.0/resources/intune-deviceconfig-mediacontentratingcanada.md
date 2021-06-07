---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eff3a957e242dfad4840ad5d616cec54f9a3c344
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755040"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="f510f-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="f510f-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="f510f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f510f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f510f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f510f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f510f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f510f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f510f-107">属性</span><span class="sxs-lookup"><span data-stu-id="f510f-107">Properties</span></span>
|<span data-ttu-id="f510f-108">属性</span><span class="sxs-lookup"><span data-stu-id="f510f-108">Property</span></span>|<span data-ttu-id="f510f-109">类型</span><span class="sxs-lookup"><span data-stu-id="f510f-109">Type</span></span>|<span data-ttu-id="f510f-110">Description</span><span class="sxs-lookup"><span data-stu-id="f510f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f510f-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f510f-111">movieRating</span></span>|[<span data-ttu-id="f510f-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="f510f-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="f510f-113">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="f510f-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="f510f-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="f510f-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="f510f-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f510f-115">tvRating</span></span>|[<span data-ttu-id="f510f-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f510f-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="f510f-117">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="f510f-117">TV rating selected for Canada.</span></span> <span data-ttu-id="f510f-118">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f510f-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f510f-119">关系</span><span class="sxs-lookup"><span data-stu-id="f510f-119">Relationships</span></span>
<span data-ttu-id="f510f-120">无</span><span class="sxs-lookup"><span data-stu-id="f510f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f510f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f510f-121">JSON Representation</span></span>
<span data-ttu-id="f510f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f510f-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```




