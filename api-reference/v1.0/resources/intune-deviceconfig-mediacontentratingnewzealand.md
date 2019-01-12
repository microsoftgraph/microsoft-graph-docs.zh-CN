---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d6556409f0893430813d2e9dbd753f97fa76886
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932243"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="7120e-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="7120e-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="7120e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7120e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7120e-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7120e-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7120e-106">属性</span><span class="sxs-lookup"><span data-stu-id="7120e-106">Properties</span></span>
|<span data-ttu-id="7120e-107">属性</span><span class="sxs-lookup"><span data-stu-id="7120e-107">Property</span></span>|<span data-ttu-id="7120e-108">类型</span><span class="sxs-lookup"><span data-stu-id="7120e-108">Type</span></span>|<span data-ttu-id="7120e-109">说明</span><span class="sxs-lookup"><span data-stu-id="7120e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7120e-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="7120e-110">movieRating</span></span>|[<span data-ttu-id="7120e-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="7120e-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="7120e-112">分级新西兰所选的影片。</span><span class="sxs-lookup"><span data-stu-id="7120e-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="7120e-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="7120e-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="7120e-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="7120e-114">tvRating</span></span>|[<span data-ttu-id="7120e-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7120e-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="7120e-116">选择新西兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="7120e-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="7120e-117">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="7120e-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7120e-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="7120e-118">Relationships</span></span>
<span data-ttu-id="7120e-119">无</span><span class="sxs-lookup"><span data-stu-id="7120e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7120e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7120e-120">JSON Representation</span></span>
<span data-ttu-id="7120e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7120e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



