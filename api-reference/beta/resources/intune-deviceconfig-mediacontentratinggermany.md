---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a5a1b61069aa3568c8cb017c6c28bb3e992c38b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394514"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="e4b84-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4b84-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="e4b84-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e4b84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4b84-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e4b84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4b84-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4b84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4b84-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4b84-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e4b84-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4b84-108">Properties</span></span>
|<span data-ttu-id="e4b84-109">属性</span><span class="sxs-lookup"><span data-stu-id="e4b84-109">Property</span></span>|<span data-ttu-id="e4b84-110">类型</span><span class="sxs-lookup"><span data-stu-id="e4b84-110">Type</span></span>|<span data-ttu-id="e4b84-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4b84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b84-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e4b84-112">movieRating</span></span>|[<span data-ttu-id="e4b84-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="e4b84-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="e4b84-114">分级德国所选的影片。</span><span class="sxs-lookup"><span data-stu-id="e4b84-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="e4b84-115">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e4b84-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e4b84-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e4b84-116">tvRating</span></span>|[<span data-ttu-id="e4b84-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e4b84-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="e4b84-118">德国选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="e4b84-118">TV rating selected for Germany.</span></span> <span data-ttu-id="e4b84-119">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e4b84-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4b84-120">关系</span><span class="sxs-lookup"><span data-stu-id="e4b84-120">Relationships</span></span>
<span data-ttu-id="e4b84-121">无</span><span class="sxs-lookup"><span data-stu-id="e4b84-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4b84-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4b84-122">JSON Representation</span></span>
<span data-ttu-id="e4b84-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4b84-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```




