---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 503218cf76d235f4122e36d1d358dce9a76e0fda
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799704"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="394fc-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="394fc-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="394fc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="394fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="394fc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="394fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="394fc-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="394fc-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="394fc-107">属性</span><span class="sxs-lookup"><span data-stu-id="394fc-107">Properties</span></span>
|<span data-ttu-id="394fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="394fc-108">Property</span></span>|<span data-ttu-id="394fc-109">类型</span><span class="sxs-lookup"><span data-stu-id="394fc-109">Type</span></span>|<span data-ttu-id="394fc-110">说明</span><span class="sxs-lookup"><span data-stu-id="394fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="394fc-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="394fc-111">movieRating</span></span>|[<span data-ttu-id="394fc-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="394fc-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="394fc-113">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="394fc-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="394fc-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="394fc-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="394fc-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="394fc-115">tvRating</span></span>|[<span data-ttu-id="394fc-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="394fc-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="394fc-117">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="394fc-117">TV rating selected for Canada.</span></span> <span data-ttu-id="394fc-118">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="394fc-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="394fc-119">关系</span><span class="sxs-lookup"><span data-stu-id="394fc-119">Relationships</span></span>
<span data-ttu-id="394fc-120">无</span><span class="sxs-lookup"><span data-stu-id="394fc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="394fc-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="394fc-121">JSON Representation</span></span>
<span data-ttu-id="394fc-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="394fc-122">Here is a JSON representation of the resource.</span></span>
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





