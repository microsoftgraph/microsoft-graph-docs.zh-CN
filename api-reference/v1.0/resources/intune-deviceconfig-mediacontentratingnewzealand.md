---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
ms.openlocfilehash: 0d34843ef7cc624b222694cc8fbe0fa7a7c1b74c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009427"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="9789d-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="9789d-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="9789d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9789d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9789d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9789d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9789d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9789d-106">Properties</span></span>
|<span data-ttu-id="9789d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9789d-107">Property</span></span>|<span data-ttu-id="9789d-108">类型</span><span class="sxs-lookup"><span data-stu-id="9789d-108">Type</span></span>|<span data-ttu-id="9789d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9789d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9789d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9789d-110">movieRating</span></span>|[<span data-ttu-id="9789d-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="9789d-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="9789d-112">分级新西兰所选的影片。</span><span class="sxs-lookup"><span data-stu-id="9789d-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="9789d-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="9789d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="9789d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9789d-114">tvRating</span></span>|[<span data-ttu-id="9789d-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9789d-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="9789d-116">选择新西兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="9789d-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="9789d-117">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="9789d-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9789d-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="9789d-118">Relationships</span></span>
<span data-ttu-id="9789d-119">无</span><span class="sxs-lookup"><span data-stu-id="9789d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9789d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9789d-120">JSON Representation</span></span>
<span data-ttu-id="9789d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9789d-121">Here is a JSON representation of the resource.</span></span>
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



