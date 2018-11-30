---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
ms.openlocfilehash: dabadb4d03181d3cd66db582005c4ec58f28aa9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043397"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="49868-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="49868-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="49868-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49868-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49868-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49868-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49868-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49868-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49868-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49868-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="49868-108">属性</span><span class="sxs-lookup"><span data-stu-id="49868-108">Properties</span></span>
|<span data-ttu-id="49868-109">属性</span><span class="sxs-lookup"><span data-stu-id="49868-109">Property</span></span>|<span data-ttu-id="49868-110">类型</span><span class="sxs-lookup"><span data-stu-id="49868-110">Type</span></span>|<span data-ttu-id="49868-111">说明</span><span class="sxs-lookup"><span data-stu-id="49868-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49868-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="49868-112">movieRating</span></span>|[<span data-ttu-id="49868-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="49868-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="49868-114">法国分级所选的影片。</span><span class="sxs-lookup"><span data-stu-id="49868-114">Movies rating selected for France.</span></span> <span data-ttu-id="49868-115">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="49868-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="49868-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="49868-116">tvRating</span></span>|[<span data-ttu-id="49868-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="49868-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="49868-118">选择法国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="49868-118">TV rating selected for France.</span></span> <span data-ttu-id="49868-119">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="49868-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49868-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="49868-120">Relationships</span></span>
<span data-ttu-id="49868-121">无</span><span class="sxs-lookup"><span data-stu-id="49868-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49868-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49868-122">JSON Representation</span></span>
<span data-ttu-id="49868-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49868-123">Here is a JSON representation of the resource.</span></span>
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





