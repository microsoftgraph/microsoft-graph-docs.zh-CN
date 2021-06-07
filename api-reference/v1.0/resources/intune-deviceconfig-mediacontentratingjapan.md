---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 691b723f2140bbdda370bbf5b46330579ca0a871
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758832"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="57779-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="57779-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="57779-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57779-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57779-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57779-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57779-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="57779-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="57779-107">属性</span><span class="sxs-lookup"><span data-stu-id="57779-107">Properties</span></span>
|<span data-ttu-id="57779-108">属性</span><span class="sxs-lookup"><span data-stu-id="57779-108">Property</span></span>|<span data-ttu-id="57779-109">类型</span><span class="sxs-lookup"><span data-stu-id="57779-109">Type</span></span>|<span data-ttu-id="57779-110">说明</span><span class="sxs-lookup"><span data-stu-id="57779-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57779-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="57779-111">movieRating</span></span>|[<span data-ttu-id="57779-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="57779-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="57779-113">为日本选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="57779-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="57779-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="57779-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="57779-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="57779-115">tvRating</span></span>|[<span data-ttu-id="57779-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="57779-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="57779-117">为日本选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="57779-117">TV rating selected for Japan.</span></span> <span data-ttu-id="57779-118">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="57779-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57779-119">关系</span><span class="sxs-lookup"><span data-stu-id="57779-119">Relationships</span></span>
<span data-ttu-id="57779-120">无</span><span class="sxs-lookup"><span data-stu-id="57779-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57779-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57779-121">JSON Representation</span></span>
<span data-ttu-id="57779-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57779-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```




