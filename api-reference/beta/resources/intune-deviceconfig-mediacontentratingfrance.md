---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e149077493280145b2681cc2ad0111ec45534a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862312"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="0c4f4-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c4f4-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="0c4f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c4f4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c4f4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c4f4-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0c4f4-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0c4f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c4f4-108">Properties</span></span>
|<span data-ttu-id="0c4f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="0c4f4-109">Property</span></span>|<span data-ttu-id="0c4f4-110">类型</span><span class="sxs-lookup"><span data-stu-id="0c4f4-110">Type</span></span>|<span data-ttu-id="0c4f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="0c4f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c4f4-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0c4f4-112">movieRating</span></span>|[<span data-ttu-id="0c4f4-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="0c4f4-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="0c4f4-114">法国分级所选的影片。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-114">Movies rating selected for France.</span></span> <span data-ttu-id="0c4f4-115">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0c4f4-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0c4f4-116">tvRating</span></span>|[<span data-ttu-id="0c4f4-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0c4f4-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="0c4f4-118">选择法国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-118">TV rating selected for France.</span></span> <span data-ttu-id="0c4f4-119">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c4f4-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="0c4f4-120">Relationships</span></span>
<span data-ttu-id="0c4f4-121">无</span><span class="sxs-lookup"><span data-stu-id="0c4f4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c4f4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c4f4-122">JSON Representation</span></span>
<span data-ttu-id="0c4f4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c4f4-123">Here is a JSON representation of the resource.</span></span>
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





