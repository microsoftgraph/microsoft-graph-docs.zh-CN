---
title: mediaContentRatingGermany 资源类型
description: 尚未记录
ms.openlocfilehash: 40ad8d4794b44a41614d9ed02341a00bdb4df86d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009426"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="806f9-103">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="806f9-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="806f9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="806f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="806f9-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="806f9-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="806f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="806f9-106">Properties</span></span>
|<span data-ttu-id="806f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="806f9-107">Property</span></span>|<span data-ttu-id="806f9-108">类型</span><span class="sxs-lookup"><span data-stu-id="806f9-108">Type</span></span>|<span data-ttu-id="806f9-109">说明</span><span class="sxs-lookup"><span data-stu-id="806f9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="806f9-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="806f9-110">movieRating</span></span>|[<span data-ttu-id="806f9-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="806f9-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="806f9-112">分级德国所选的影片。</span><span class="sxs-lookup"><span data-stu-id="806f9-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="806f9-113">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="806f9-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="806f9-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="806f9-114">tvRating</span></span>|[<span data-ttu-id="806f9-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="806f9-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="806f9-116">德国选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="806f9-116">TV rating selected for Germany.</span></span> <span data-ttu-id="806f9-117">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="806f9-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="806f9-118">关系</span><span class="sxs-lookup"><span data-stu-id="806f9-118">Relationships</span></span>
<span data-ttu-id="806f9-119">无</span><span class="sxs-lookup"><span data-stu-id="806f9-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="806f9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="806f9-120">JSON Representation</span></span>
<span data-ttu-id="806f9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806f9-121">Here is a JSON representation of the resource.</span></span>
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



