---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
ms.openlocfilehash: f60df6c4948d0e0208b545a8a25e31ca29247879
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009431"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="81eca-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="81eca-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="81eca-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="81eca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81eca-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="81eca-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="81eca-106">属性</span><span class="sxs-lookup"><span data-stu-id="81eca-106">Properties</span></span>
|<span data-ttu-id="81eca-107">属性</span><span class="sxs-lookup"><span data-stu-id="81eca-107">Property</span></span>|<span data-ttu-id="81eca-108">类型</span><span class="sxs-lookup"><span data-stu-id="81eca-108">Type</span></span>|<span data-ttu-id="81eca-109">说明</span><span class="sxs-lookup"><span data-stu-id="81eca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81eca-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="81eca-110">movieRating</span></span>|[<span data-ttu-id="81eca-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="81eca-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="81eca-112">分级澳大利亚的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="81eca-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="81eca-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="81eca-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="81eca-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="81eca-114">tvRating</span></span>|[<span data-ttu-id="81eca-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="81eca-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="81eca-116">澳大利亚选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="81eca-116">TV rating selected for Australia.</span></span> <span data-ttu-id="81eca-117">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="81eca-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81eca-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="81eca-118">Relationships</span></span>
<span data-ttu-id="81eca-119">无</span><span class="sxs-lookup"><span data-stu-id="81eca-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81eca-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81eca-120">JSON Representation</span></span>
<span data-ttu-id="81eca-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81eca-121">Here is a JSON representation of the resource.</span></span>
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



