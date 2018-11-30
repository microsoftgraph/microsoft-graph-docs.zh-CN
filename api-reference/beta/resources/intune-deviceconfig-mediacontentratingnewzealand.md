---
title: mediaContentRatingNewZealand 资源类型
description: 尚未记录
ms.openlocfilehash: e7650d7155c06ff30b541d873830865bed1d92ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048772"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="99945-103">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="99945-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="99945-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99945-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99945-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99945-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99945-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99945-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99945-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99945-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="99945-108">属性</span><span class="sxs-lookup"><span data-stu-id="99945-108">Properties</span></span>
|<span data-ttu-id="99945-109">属性</span><span class="sxs-lookup"><span data-stu-id="99945-109">Property</span></span>|<span data-ttu-id="99945-110">类型</span><span class="sxs-lookup"><span data-stu-id="99945-110">Type</span></span>|<span data-ttu-id="99945-111">说明</span><span class="sxs-lookup"><span data-stu-id="99945-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99945-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="99945-112">movieRating</span></span>|[<span data-ttu-id="99945-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="99945-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="99945-114">分级新西兰所选的影片。</span><span class="sxs-lookup"><span data-stu-id="99945-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="99945-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="99945-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="99945-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="99945-116">tvRating</span></span>|[<span data-ttu-id="99945-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="99945-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="99945-118">选择新西兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="99945-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="99945-119">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="99945-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99945-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="99945-120">Relationships</span></span>
<span data-ttu-id="99945-121">无</span><span class="sxs-lookup"><span data-stu-id="99945-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99945-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99945-122">JSON Representation</span></span>
<span data-ttu-id="99945-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99945-123">Here is a JSON representation of the resource.</span></span>
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





