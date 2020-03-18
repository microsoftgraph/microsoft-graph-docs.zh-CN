---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 49698243aed27af3897bc48b8d78e8195fb7fb53
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788595"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="29316-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="29316-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="29316-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29316-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29316-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29316-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29316-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="29316-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="29316-107">属性</span><span class="sxs-lookup"><span data-stu-id="29316-107">Properties</span></span>
|<span data-ttu-id="29316-108">属性</span><span class="sxs-lookup"><span data-stu-id="29316-108">Property</span></span>|<span data-ttu-id="29316-109">类型</span><span class="sxs-lookup"><span data-stu-id="29316-109">Type</span></span>|<span data-ttu-id="29316-110">说明</span><span class="sxs-lookup"><span data-stu-id="29316-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29316-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="29316-111">movieRating</span></span>|[<span data-ttu-id="29316-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="29316-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="29316-113">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="29316-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="29316-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="29316-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="29316-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="29316-115">tvRating</span></span>|[<span data-ttu-id="29316-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="29316-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="29316-117">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="29316-117">TV rating selected for Canada.</span></span> <span data-ttu-id="29316-118">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="29316-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29316-119">关系</span><span class="sxs-lookup"><span data-stu-id="29316-119">Relationships</span></span>
<span data-ttu-id="29316-120">无</span><span class="sxs-lookup"><span data-stu-id="29316-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29316-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29316-121">JSON Representation</span></span>
<span data-ttu-id="29316-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29316-122">Here is a JSON representation of the resource.</span></span>
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



