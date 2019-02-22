---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38f3bac4e8410a3c63bd07319888ab0a5fc7df19
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146345"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="d4be2-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4be2-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="d4be2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4be2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4be2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4be2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4be2-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4be2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d4be2-107">属性</span><span class="sxs-lookup"><span data-stu-id="d4be2-107">Properties</span></span>
|<span data-ttu-id="d4be2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4be2-108">Property</span></span>|<span data-ttu-id="d4be2-109">类型</span><span class="sxs-lookup"><span data-stu-id="d4be2-109">Type</span></span>|<span data-ttu-id="d4be2-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4be2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4be2-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="d4be2-111">movieRating</span></span>|[<span data-ttu-id="d4be2-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="d4be2-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="d4be2-113">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="d4be2-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="d4be2-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="d4be2-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="d4be2-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="d4be2-115">tvRating</span></span>|[<span data-ttu-id="d4be2-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d4be2-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="d4be2-117">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="d4be2-117">TV rating selected for Canada.</span></span> <span data-ttu-id="d4be2-118">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d4be2-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4be2-119">关系</span><span class="sxs-lookup"><span data-stu-id="d4be2-119">Relationships</span></span>
<span data-ttu-id="d4be2-120">无</span><span class="sxs-lookup"><span data-stu-id="d4be2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4be2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4be2-121">JSON Representation</span></span>
<span data-ttu-id="d4be2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4be2-122">Here is a JSON representation of the resource.</span></span>
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




