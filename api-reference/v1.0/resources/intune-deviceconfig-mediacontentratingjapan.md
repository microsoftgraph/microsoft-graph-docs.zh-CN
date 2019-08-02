---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c4e4268857f2d76e1dcf01e047a492f80492a89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031386"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="8c3b9-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c3b9-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="8c3b9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c3b9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c3b9-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c3b9-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8c3b9-106">属性</span><span class="sxs-lookup"><span data-stu-id="8c3b9-106">Properties</span></span>
|<span data-ttu-id="8c3b9-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c3b9-107">Property</span></span>|<span data-ttu-id="8c3b9-108">类型</span><span class="sxs-lookup"><span data-stu-id="8c3b9-108">Type</span></span>|<span data-ttu-id="8c3b9-109">说明</span><span class="sxs-lookup"><span data-stu-id="8c3b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c3b9-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8c3b9-110">movieRating</span></span>|[<span data-ttu-id="8c3b9-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="8c3b9-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="8c3b9-112">为日本选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="8c3b9-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="8c3b9-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="8c3b9-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8c3b9-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8c3b9-114">tvRating</span></span>|[<span data-ttu-id="8c3b9-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8c3b9-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="8c3b9-116">为日本选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="8c3b9-116">TV rating selected for Japan.</span></span> <span data-ttu-id="8c3b9-117">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="8c3b9-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c3b9-118">关系</span><span class="sxs-lookup"><span data-stu-id="8c3b9-118">Relationships</span></span>
<span data-ttu-id="8c3b9-119">无</span><span class="sxs-lookup"><span data-stu-id="8c3b9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c3b9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c3b9-120">JSON Representation</span></span>
<span data-ttu-id="8c3b9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c3b9-121">Here is a JSON representation of the resource.</span></span>
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



