---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0e35a13285ffa1cb134ea4b87928fd690ca9c21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989316"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="2f6cb-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f6cb-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="2f6cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f6cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f6cb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f6cb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f6cb-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f6cb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2f6cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f6cb-108">Properties</span></span>
|<span data-ttu-id="2f6cb-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f6cb-109">Property</span></span>|<span data-ttu-id="2f6cb-110">类型</span><span class="sxs-lookup"><span data-stu-id="2f6cb-110">Type</span></span>|<span data-ttu-id="2f6cb-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f6cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f6cb-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="2f6cb-112">movieRating</span></span>|[<span data-ttu-id="2f6cb-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="2f6cb-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="2f6cb-114">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="2f6cb-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="2f6cb-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="2f6cb-116">tvRating</span></span>|[<span data-ttu-id="2f6cb-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2f6cb-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="2f6cb-118">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-118">TV rating selected for Canada.</span></span> <span data-ttu-id="2f6cb-119">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f6cb-120">关系</span><span class="sxs-lookup"><span data-stu-id="2f6cb-120">Relationships</span></span>
<span data-ttu-id="2f6cb-121">无</span><span class="sxs-lookup"><span data-stu-id="2f6cb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f6cb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f6cb-122">JSON Representation</span></span>
<span data-ttu-id="2f6cb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f6cb-123">Here is a JSON representation of the resource.</span></span>
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






