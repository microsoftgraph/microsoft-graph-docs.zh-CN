---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
ms.openlocfilehash: 821a648f839e531c2efaa3da4b4b1aead65c9673
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044931"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="1db3d-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="1db3d-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="1db3d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1db3d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1db3d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1db3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1db3d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1db3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1db3d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1db3d-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1db3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1db3d-108">Properties</span></span>
|<span data-ttu-id="1db3d-109">属性</span><span class="sxs-lookup"><span data-stu-id="1db3d-109">Property</span></span>|<span data-ttu-id="1db3d-110">类型</span><span class="sxs-lookup"><span data-stu-id="1db3d-110">Type</span></span>|<span data-ttu-id="1db3d-111">说明</span><span class="sxs-lookup"><span data-stu-id="1db3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1db3d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="1db3d-112">movieRating</span></span>|[<span data-ttu-id="1db3d-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="1db3d-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="1db3d-114">分级德国所选的影片。</span><span class="sxs-lookup"><span data-stu-id="1db3d-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="1db3d-115">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="1db3d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="1db3d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="1db3d-116">tvRating</span></span>|[<span data-ttu-id="1db3d-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1db3d-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="1db3d-118">德国选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="1db3d-118">TV rating selected for Germany.</span></span> <span data-ttu-id="1db3d-119">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="1db3d-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1db3d-120">关系</span><span class="sxs-lookup"><span data-stu-id="1db3d-120">Relationships</span></span>
<span data-ttu-id="1db3d-121">无</span><span class="sxs-lookup"><span data-stu-id="1db3d-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1db3d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1db3d-122">JSON Representation</span></span>
<span data-ttu-id="1db3d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1db3d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```





