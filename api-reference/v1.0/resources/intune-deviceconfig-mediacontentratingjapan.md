---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0f394b85af0fd1f1c85a8db34025b2e1f139521
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822132"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="f563d-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="f563d-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="f563d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f563d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f563d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f563d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f563d-106">属性</span><span class="sxs-lookup"><span data-stu-id="f563d-106">Properties</span></span>
|<span data-ttu-id="f563d-107">属性</span><span class="sxs-lookup"><span data-stu-id="f563d-107">Property</span></span>|<span data-ttu-id="f563d-108">类型</span><span class="sxs-lookup"><span data-stu-id="f563d-108">Type</span></span>|<span data-ttu-id="f563d-109">说明</span><span class="sxs-lookup"><span data-stu-id="f563d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f563d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="f563d-110">movieRating</span></span>|[<span data-ttu-id="f563d-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="f563d-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="f563d-112">分级日本所选的影片。</span><span class="sxs-lookup"><span data-stu-id="f563d-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="f563d-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f563d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f563d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="f563d-114">tvRating</span></span>|[<span data-ttu-id="f563d-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f563d-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="f563d-116">日本选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="f563d-116">TV rating selected for Japan.</span></span> <span data-ttu-id="f563d-117">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="f563d-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f563d-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="f563d-118">Relationships</span></span>
<span data-ttu-id="f563d-119">无</span><span class="sxs-lookup"><span data-stu-id="f563d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f563d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f563d-120">JSON Representation</span></span>
<span data-ttu-id="f563d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f563d-121">Here is a JSON representation of the resource.</span></span>
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



