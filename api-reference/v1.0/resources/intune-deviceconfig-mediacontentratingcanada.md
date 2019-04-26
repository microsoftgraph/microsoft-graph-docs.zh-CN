---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88975975b07eb2805ee5f73cc416e3803d5fe24f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572351"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="dd97b-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd97b-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="dd97b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd97b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd97b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dd97b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dd97b-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd97b-106">Properties</span></span>
|<span data-ttu-id="dd97b-107">属性</span><span class="sxs-lookup"><span data-stu-id="dd97b-107">Property</span></span>|<span data-ttu-id="dd97b-108">类型</span><span class="sxs-lookup"><span data-stu-id="dd97b-108">Type</span></span>|<span data-ttu-id="dd97b-109">说明</span><span class="sxs-lookup"><span data-stu-id="dd97b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd97b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="dd97b-110">movieRating</span></span>|[<span data-ttu-id="dd97b-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="dd97b-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="dd97b-112">为加拿大选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="dd97b-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="dd97b-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` 或 `restricted`。</span><span class="sxs-lookup"><span data-stu-id="dd97b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="dd97b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="dd97b-114">tvRating</span></span>|[<span data-ttu-id="dd97b-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="dd97b-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="dd97b-116">为加拿大选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="dd97b-116">TV rating selected for Canada.</span></span> <span data-ttu-id="dd97b-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="dd97b-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd97b-118">关系</span><span class="sxs-lookup"><span data-stu-id="dd97b-118">Relationships</span></span>
<span data-ttu-id="dd97b-119">无</span><span class="sxs-lookup"><span data-stu-id="dd97b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd97b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd97b-120">JSON Representation</span></span>
<span data-ttu-id="dd97b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd97b-121">Here is a JSON representation of the resource.</span></span>
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



