---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 94d291f417ede3a4357372dddf19d3ad1e08f332
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709985"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="8452e-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="8452e-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="8452e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8452e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8452e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8452e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8452e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8452e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8452e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8452e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8452e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8452e-108">Properties</span></span>
|<span data-ttu-id="8452e-109">属性</span><span class="sxs-lookup"><span data-stu-id="8452e-109">Property</span></span>|<span data-ttu-id="8452e-110">类型</span><span class="sxs-lookup"><span data-stu-id="8452e-110">Type</span></span>|<span data-ttu-id="8452e-111">说明</span><span class="sxs-lookup"><span data-stu-id="8452e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8452e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="8452e-112">movieRating</span></span>|[<span data-ttu-id="8452e-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="8452e-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="8452e-114">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="8452e-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="8452e-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="8452e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="8452e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="8452e-116">tvRating</span></span>|[<span data-ttu-id="8452e-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8452e-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="8452e-118">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="8452e-118">TV rating selected for Canada.</span></span> <span data-ttu-id="8452e-119">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="8452e-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8452e-120">关系</span><span class="sxs-lookup"><span data-stu-id="8452e-120">Relationships</span></span>
<span data-ttu-id="8452e-121">无</span><span class="sxs-lookup"><span data-stu-id="8452e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8452e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8452e-122">JSON Representation</span></span>
<span data-ttu-id="8452e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8452e-123">Here is a JSON representation of the resource.</span></span>
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





