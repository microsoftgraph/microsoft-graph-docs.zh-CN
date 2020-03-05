---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9c55acb14d9e1d184da95a343edac6b3a6dcf4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526032"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="7f655-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f655-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="7f655-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7f655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f655-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f655-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f655-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f655-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f655-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f655-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7f655-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f655-108">Properties</span></span>
|<span data-ttu-id="7f655-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f655-109">Property</span></span>|<span data-ttu-id="7f655-110">类型</span><span class="sxs-lookup"><span data-stu-id="7f655-110">Type</span></span>|<span data-ttu-id="7f655-111">说明</span><span class="sxs-lookup"><span data-stu-id="7f655-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f655-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="7f655-112">movieRating</span></span>|[<span data-ttu-id="7f655-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="7f655-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="7f655-114">为德国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="7f655-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="7f655-115">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="7f655-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="7f655-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="7f655-116">tvRating</span></span>|[<span data-ttu-id="7f655-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7f655-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="7f655-118">为德国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="7f655-118">TV rating selected for Germany.</span></span> <span data-ttu-id="7f655-119">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="7f655-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f655-120">关系</span><span class="sxs-lookup"><span data-stu-id="7f655-120">Relationships</span></span>
<span data-ttu-id="7f655-121">无</span><span class="sxs-lookup"><span data-stu-id="7f655-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f655-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f655-122">JSON Representation</span></span>
<span data-ttu-id="7f655-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f655-123">Here is a JSON representation of the resource.</span></span>
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



