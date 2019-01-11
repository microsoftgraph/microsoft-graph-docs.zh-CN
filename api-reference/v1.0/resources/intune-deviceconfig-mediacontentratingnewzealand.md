---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4a22f9510a615dab746912aed1de5123184ca3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850545"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="aebfd-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="aebfd-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="aebfd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aebfd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aebfd-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aebfd-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="aebfd-106">属性</span><span class="sxs-lookup"><span data-stu-id="aebfd-106">Properties</span></span>
|<span data-ttu-id="aebfd-107">属性</span><span class="sxs-lookup"><span data-stu-id="aebfd-107">Property</span></span>|<span data-ttu-id="aebfd-108">类型</span><span class="sxs-lookup"><span data-stu-id="aebfd-108">Type</span></span>|<span data-ttu-id="aebfd-109">说明</span><span class="sxs-lookup"><span data-stu-id="aebfd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aebfd-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="aebfd-110">movieRating</span></span>|[<span data-ttu-id="aebfd-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="aebfd-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="aebfd-112">分级新西兰所选的影片。</span><span class="sxs-lookup"><span data-stu-id="aebfd-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="aebfd-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="aebfd-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="aebfd-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="aebfd-114">tvRating</span></span>|[<span data-ttu-id="aebfd-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="aebfd-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="aebfd-116">选择新西兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="aebfd-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="aebfd-117">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="aebfd-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aebfd-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="aebfd-118">Relationships</span></span>
<span data-ttu-id="aebfd-119">无</span><span class="sxs-lookup"><span data-stu-id="aebfd-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aebfd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aebfd-120">JSON Representation</span></span>
<span data-ttu-id="aebfd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aebfd-121">Here is a JSON representation of the resource.</span></span>
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



