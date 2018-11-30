---
title: mediaContentRatingIreland 资源类型
description: 尚未记录
ms.openlocfilehash: b4348e6f73730d59e6e67b3e102b9ad9caa98add
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007950"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="84008-103">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="84008-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="84008-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="84008-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84008-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="84008-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="84008-106">属性</span><span class="sxs-lookup"><span data-stu-id="84008-106">Properties</span></span>
|<span data-ttu-id="84008-107">属性</span><span class="sxs-lookup"><span data-stu-id="84008-107">Property</span></span>|<span data-ttu-id="84008-108">类型</span><span class="sxs-lookup"><span data-stu-id="84008-108">Type</span></span>|<span data-ttu-id="84008-109">说明</span><span class="sxs-lookup"><span data-stu-id="84008-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84008-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="84008-110">movieRating</span></span>|[<span data-ttu-id="84008-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="84008-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="84008-112">分级爱尔兰的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="84008-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="84008-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="84008-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="84008-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="84008-114">tvRating</span></span>|[<span data-ttu-id="84008-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="84008-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="84008-116">选择爱尔兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="84008-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="84008-117">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="84008-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84008-118">关系</span><span class="sxs-lookup"><span data-stu-id="84008-118">Relationships</span></span>
<span data-ttu-id="84008-119">无</span><span class="sxs-lookup"><span data-stu-id="84008-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84008-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84008-120">JSON Representation</span></span>
<span data-ttu-id="84008-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84008-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



