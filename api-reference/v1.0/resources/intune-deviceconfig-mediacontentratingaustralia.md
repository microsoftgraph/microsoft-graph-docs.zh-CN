---
title: mediaContentRatingAustralia 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5f3f12cc233c1accfad05ccec92d412c75426d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952844"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="25c24-103">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="25c24-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="25c24-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="25c24-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25c24-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25c24-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="25c24-106">属性</span><span class="sxs-lookup"><span data-stu-id="25c24-106">Properties</span></span>
|<span data-ttu-id="25c24-107">属性</span><span class="sxs-lookup"><span data-stu-id="25c24-107">Property</span></span>|<span data-ttu-id="25c24-108">类型</span><span class="sxs-lookup"><span data-stu-id="25c24-108">Type</span></span>|<span data-ttu-id="25c24-109">说明</span><span class="sxs-lookup"><span data-stu-id="25c24-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c24-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="25c24-110">movieRating</span></span>|[<span data-ttu-id="25c24-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="25c24-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="25c24-112">分级澳大利亚的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="25c24-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="25c24-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="25c24-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="25c24-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="25c24-114">tvRating</span></span>|[<span data-ttu-id="25c24-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="25c24-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="25c24-116">澳大利亚选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="25c24-116">TV rating selected for Australia.</span></span> <span data-ttu-id="25c24-117">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="25c24-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25c24-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="25c24-118">Relationships</span></span>
<span data-ttu-id="25c24-119">无</span><span class="sxs-lookup"><span data-stu-id="25c24-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25c24-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25c24-120">JSON Representation</span></span>
<span data-ttu-id="25c24-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25c24-121">Here is a JSON representation of the resource.</span></span>
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



