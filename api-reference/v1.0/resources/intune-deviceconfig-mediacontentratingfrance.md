---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
ms.openlocfilehash: bd2f4933ea05c7db193d700799cdcbdc79490356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008248"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="f12f6-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="f12f6-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="f12f6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f12f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f12f6-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f12f6-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f12f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="f12f6-106">Properties</span></span>
|<span data-ttu-id="f12f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="f12f6-107">Property</span></span>|<span data-ttu-id="f12f6-108">类型</span><span class="sxs-lookup"><span data-stu-id="f12f6-108">Type</span></span>|<span data-ttu-id="f12f6-109">说明</span><span class="sxs-lookup"><span data-stu-id="f12f6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f12f6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="f12f6-110">movieRating</span></span>|[<span data-ttu-id="f12f6-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="f12f6-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="f12f6-112">法国分级所选的影片。</span><span class="sxs-lookup"><span data-stu-id="f12f6-112">Movies rating selected for France.</span></span> <span data-ttu-id="f12f6-113">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f12f6-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f12f6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="f12f6-114">tvRating</span></span>|[<span data-ttu-id="f12f6-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f12f6-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="f12f6-116">选择法国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="f12f6-116">TV rating selected for France.</span></span> <span data-ttu-id="f12f6-117">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f12f6-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f12f6-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="f12f6-118">Relationships</span></span>
<span data-ttu-id="f12f6-119">无</span><span class="sxs-lookup"><span data-stu-id="f12f6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f12f6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f12f6-120">JSON Representation</span></span>
<span data-ttu-id="f12f6-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f12f6-121">Here is a JSON representation of the resource.</span></span>
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



