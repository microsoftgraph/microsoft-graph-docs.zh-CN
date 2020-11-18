---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5efd89490b83994ab9ce771a235fa2c8ab0e144
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198715"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="5e29a-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e29a-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="5e29a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e29a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e29a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e29a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e29a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e29a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e29a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5e29a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5e29a-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e29a-108">Properties</span></span>
|<span data-ttu-id="5e29a-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e29a-109">Property</span></span>|<span data-ttu-id="5e29a-110">类型</span><span class="sxs-lookup"><span data-stu-id="5e29a-110">Type</span></span>|<span data-ttu-id="5e29a-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e29a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e29a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="5e29a-112">movieRating</span></span>|[<span data-ttu-id="5e29a-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="5e29a-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="5e29a-114">为日本选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="5e29a-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="5e29a-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="5e29a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5e29a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="5e29a-116">tvRating</span></span>|[<span data-ttu-id="5e29a-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5e29a-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="5e29a-118">为日本选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="5e29a-118">TV rating selected for Japan.</span></span> <span data-ttu-id="5e29a-119">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="5e29a-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e29a-120">关系</span><span class="sxs-lookup"><span data-stu-id="5e29a-120">Relationships</span></span>
<span data-ttu-id="5e29a-121">无</span><span class="sxs-lookup"><span data-stu-id="5e29a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e29a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e29a-122">JSON Representation</span></span>
<span data-ttu-id="5e29a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e29a-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```




