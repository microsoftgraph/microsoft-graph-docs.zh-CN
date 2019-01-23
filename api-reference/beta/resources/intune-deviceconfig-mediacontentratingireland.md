---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3efd96cc8ad015989365dff10b1659ef50c4fb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422598"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="fb661-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb661-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="fb661-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fb661-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb661-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb661-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb661-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb661-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb661-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fb661-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fb661-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb661-108">Properties</span></span>
|<span data-ttu-id="fb661-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb661-109">Property</span></span>|<span data-ttu-id="fb661-110">类型</span><span class="sxs-lookup"><span data-stu-id="fb661-110">Type</span></span>|<span data-ttu-id="fb661-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb661-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb661-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="fb661-112">movieRating</span></span>|[<span data-ttu-id="fb661-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="fb661-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="fb661-114">分级爱尔兰的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="fb661-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="fb661-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="fb661-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="fb661-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="fb661-116">tvRating</span></span>|[<span data-ttu-id="fb661-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fb661-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="fb661-118">选择爱尔兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="fb661-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="fb661-119">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="fb661-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb661-120">关系</span><span class="sxs-lookup"><span data-stu-id="fb661-120">Relationships</span></span>
<span data-ttu-id="fb661-121">无</span><span class="sxs-lookup"><span data-stu-id="fb661-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb661-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb661-122">JSON Representation</span></span>
<span data-ttu-id="fb661-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb661-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```




