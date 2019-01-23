---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb199abfc350a8b88913e353d377745714368c95
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412364"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="76077-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="76077-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="76077-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="76077-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76077-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76077-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76077-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76077-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76077-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="76077-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="76077-108">属性</span><span class="sxs-lookup"><span data-stu-id="76077-108">Properties</span></span>
|<span data-ttu-id="76077-109">属性</span><span class="sxs-lookup"><span data-stu-id="76077-109">Property</span></span>|<span data-ttu-id="76077-110">类型</span><span class="sxs-lookup"><span data-stu-id="76077-110">Type</span></span>|<span data-ttu-id="76077-111">说明</span><span class="sxs-lookup"><span data-stu-id="76077-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76077-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="76077-112">movieRating</span></span>|[<span data-ttu-id="76077-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="76077-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="76077-114">法国分级所选的影片。</span><span class="sxs-lookup"><span data-stu-id="76077-114">Movies rating selected for France.</span></span> <span data-ttu-id="76077-115">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="76077-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="76077-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="76077-116">tvRating</span></span>|[<span data-ttu-id="76077-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="76077-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="76077-118">选择法国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="76077-118">TV rating selected for France.</span></span> <span data-ttu-id="76077-119">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="76077-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76077-120">关系</span><span class="sxs-lookup"><span data-stu-id="76077-120">Relationships</span></span>
<span data-ttu-id="76077-121">无</span><span class="sxs-lookup"><span data-stu-id="76077-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76077-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76077-122">JSON Representation</span></span>
<span data-ttu-id="76077-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76077-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```




