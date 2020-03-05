---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b63183914de4bf0fd2903142003f77359e9bb2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529636"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="ccc86-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccc86-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="ccc86-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ccc86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccc86-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ccc86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccc86-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccc86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc86-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ccc86-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ccc86-108">属性</span><span class="sxs-lookup"><span data-stu-id="ccc86-108">Properties</span></span>
|<span data-ttu-id="ccc86-109">属性</span><span class="sxs-lookup"><span data-stu-id="ccc86-109">Property</span></span>|<span data-ttu-id="ccc86-110">类型</span><span class="sxs-lookup"><span data-stu-id="ccc86-110">Type</span></span>|<span data-ttu-id="ccc86-111">说明</span><span class="sxs-lookup"><span data-stu-id="ccc86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc86-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="ccc86-112">movieRating</span></span>|[<span data-ttu-id="ccc86-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="ccc86-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="ccc86-114">为澳大利亚选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="ccc86-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="ccc86-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15` 或 `agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="ccc86-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="ccc86-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="ccc86-116">tvRating</span></span>|[<span data-ttu-id="ccc86-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ccc86-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="ccc86-118">为澳大利亚选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="ccc86-118">TV rating selected for Australia.</span></span> <span data-ttu-id="ccc86-119">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="ccc86-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccc86-120">关系</span><span class="sxs-lookup"><span data-stu-id="ccc86-120">Relationships</span></span>
<span data-ttu-id="ccc86-121">无</span><span class="sxs-lookup"><span data-stu-id="ccc86-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccc86-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccc86-122">JSON Representation</span></span>
<span data-ttu-id="ccc86-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccc86-123">Here is a JSON representation of the resource.</span></span>
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



