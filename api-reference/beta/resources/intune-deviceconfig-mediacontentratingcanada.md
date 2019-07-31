---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f7ca7461b24c065a1a62c089194d08165b371f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970120"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="d170e-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="d170e-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="d170e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d170e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d170e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d170e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d170e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d170e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d170e-107">属性</span><span class="sxs-lookup"><span data-stu-id="d170e-107">Properties</span></span>
|<span data-ttu-id="d170e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d170e-108">Property</span></span>|<span data-ttu-id="d170e-109">类型</span><span class="sxs-lookup"><span data-stu-id="d170e-109">Type</span></span>|<span data-ttu-id="d170e-110">说明</span><span class="sxs-lookup"><span data-stu-id="d170e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d170e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="d170e-111">movieRating</span></span>|[<span data-ttu-id="d170e-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="d170e-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="d170e-113">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="d170e-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="d170e-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="d170e-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="d170e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="d170e-115">tvRating</span></span>|[<span data-ttu-id="d170e-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d170e-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="d170e-117">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="d170e-117">TV rating selected for Canada.</span></span> <span data-ttu-id="d170e-118">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d170e-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d170e-119">关系</span><span class="sxs-lookup"><span data-stu-id="d170e-119">Relationships</span></span>
<span data-ttu-id="d170e-120">无</span><span class="sxs-lookup"><span data-stu-id="d170e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d170e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d170e-121">JSON Representation</span></span>
<span data-ttu-id="d170e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d170e-122">Here is a JSON representation of the resource.</span></span>
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





