---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4f6fe2e4f4ca0f629ac0d4dbc387aab68122896c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913112"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="1a680-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a680-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="1a680-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a680-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a680-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1a680-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1a680-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a680-106">Properties</span></span>
|<span data-ttu-id="1a680-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a680-107">Property</span></span>|<span data-ttu-id="1a680-108">类型</span><span class="sxs-lookup"><span data-stu-id="1a680-108">Type</span></span>|<span data-ttu-id="1a680-109">说明</span><span class="sxs-lookup"><span data-stu-id="1a680-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a680-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1a680-110">movieRating</span></span>|[<span data-ttu-id="1a680-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="1a680-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="1a680-112">法国分级所选的影片。</span><span class="sxs-lookup"><span data-stu-id="1a680-112">Movies rating selected for France.</span></span> <span data-ttu-id="1a680-113">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="1a680-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="1a680-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1a680-114">tvRating</span></span>|[<span data-ttu-id="1a680-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1a680-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="1a680-116">选择法国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="1a680-116">TV rating selected for France.</span></span> <span data-ttu-id="1a680-117">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="1a680-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a680-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="1a680-118">Relationships</span></span>
<span data-ttu-id="1a680-119">无</span><span class="sxs-lookup"><span data-stu-id="1a680-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a680-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a680-120">JSON Representation</span></span>
<span data-ttu-id="1a680-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a680-121">Here is a JSON representation of the resource.</span></span>
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



