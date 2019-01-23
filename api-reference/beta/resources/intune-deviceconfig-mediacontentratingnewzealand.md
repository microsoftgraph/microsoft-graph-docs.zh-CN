---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: adfc34cf65104f0bf370a4e1ba22cfcb78bf250b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403446"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="bc998-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc998-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="bc998-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bc998-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc998-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc998-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc998-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc998-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc998-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc998-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bc998-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc998-108">Properties</span></span>
|<span data-ttu-id="bc998-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc998-109">Property</span></span>|<span data-ttu-id="bc998-110">类型</span><span class="sxs-lookup"><span data-stu-id="bc998-110">Type</span></span>|<span data-ttu-id="bc998-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc998-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc998-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bc998-112">movieRating</span></span>|[<span data-ttu-id="bc998-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="bc998-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="bc998-114">分级新西兰所选的影片。</span><span class="sxs-lookup"><span data-stu-id="bc998-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="bc998-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="bc998-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="bc998-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bc998-116">tvRating</span></span>|[<span data-ttu-id="bc998-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bc998-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="bc998-118">选择新西兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="bc998-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="bc998-119">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="bc998-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc998-120">关系</span><span class="sxs-lookup"><span data-stu-id="bc998-120">Relationships</span></span>
<span data-ttu-id="bc998-121">无</span><span class="sxs-lookup"><span data-stu-id="bc998-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc998-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc998-122">JSON Representation</span></span>
<span data-ttu-id="bc998-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc998-123">Here is a JSON representation of the resource.</span></span>
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




