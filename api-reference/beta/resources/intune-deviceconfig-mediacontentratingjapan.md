---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af5236ebf464300584525fbaebae271133134b0a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554378"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="c20c6-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="c20c6-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="c20c6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c20c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c20c6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c20c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c20c6-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c20c6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c20c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="c20c6-107">Properties</span></span>
|<span data-ttu-id="c20c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="c20c6-108">Property</span></span>|<span data-ttu-id="c20c6-109">类型</span><span class="sxs-lookup"><span data-stu-id="c20c6-109">Type</span></span>|<span data-ttu-id="c20c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="c20c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c20c6-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c20c6-111">movieRating</span></span>|[<span data-ttu-id="c20c6-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="c20c6-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="c20c6-113">为日本选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="c20c6-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="c20c6-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="c20c6-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c20c6-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c20c6-115">tvRating</span></span>|[<span data-ttu-id="c20c6-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c20c6-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="c20c6-117">为日本选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="c20c6-117">TV rating selected for Japan.</span></span> <span data-ttu-id="c20c6-118">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="c20c6-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c20c6-119">关系</span><span class="sxs-lookup"><span data-stu-id="c20c6-119">Relationships</span></span>
<span data-ttu-id="c20c6-120">无</span><span class="sxs-lookup"><span data-stu-id="c20c6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c20c6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c20c6-121">JSON Representation</span></span>
<span data-ttu-id="c20c6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c20c6-122">Here is a JSON representation of the resource.</span></span>
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





