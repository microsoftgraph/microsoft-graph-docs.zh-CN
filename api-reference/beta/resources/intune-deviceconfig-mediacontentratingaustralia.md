---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259860387e005f7fe5bfd2d402be5c03ef21149f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396635"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b3e0d-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3e0d-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b3e0d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b3e0d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3e0d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3e0d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3e0d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b3e0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3e0d-108">Properties</span></span>
|<span data-ttu-id="b3e0d-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3e0d-109">Property</span></span>|<span data-ttu-id="b3e0d-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3e0d-110">Type</span></span>|<span data-ttu-id="b3e0d-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3e0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e0d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b3e0d-112">movieRating</span></span>|[<span data-ttu-id="b3e0d-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b3e0d-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b3e0d-114">分级澳大利亚的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="b3e0d-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b3e0d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b3e0d-116">tvRating</span></span>|[<span data-ttu-id="b3e0d-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b3e0d-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b3e0d-118">澳大利亚选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-118">TV rating selected for Australia.</span></span> <span data-ttu-id="b3e0d-119">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3e0d-120">关系</span><span class="sxs-lookup"><span data-stu-id="b3e0d-120">Relationships</span></span>
<span data-ttu-id="b3e0d-121">无</span><span class="sxs-lookup"><span data-stu-id="b3e0d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3e0d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3e0d-122">JSON Representation</span></span>
<span data-ttu-id="b3e0d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3e0d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




