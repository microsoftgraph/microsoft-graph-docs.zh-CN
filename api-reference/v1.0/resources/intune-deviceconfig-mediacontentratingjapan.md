---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2b1ab45a91fb617412742481639a0203624bc11d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945921"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="8fb78-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fb78-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="8fb78-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8fb78-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fb78-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8fb78-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8fb78-106">属性</span><span class="sxs-lookup"><span data-stu-id="8fb78-106">Properties</span></span>
|<span data-ttu-id="8fb78-107">属性</span><span class="sxs-lookup"><span data-stu-id="8fb78-107">Property</span></span>|<span data-ttu-id="8fb78-108">类型</span><span class="sxs-lookup"><span data-stu-id="8fb78-108">Type</span></span>|<span data-ttu-id="8fb78-109">说明</span><span class="sxs-lookup"><span data-stu-id="8fb78-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fb78-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8fb78-110">movieRating</span></span>|[<span data-ttu-id="8fb78-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="8fb78-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="8fb78-112">分级日本所选的影片。</span><span class="sxs-lookup"><span data-stu-id="8fb78-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="8fb78-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="8fb78-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8fb78-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8fb78-114">tvRating</span></span>|[<span data-ttu-id="8fb78-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8fb78-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="8fb78-116">日本选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="8fb78-116">TV rating selected for Japan.</span></span> <span data-ttu-id="8fb78-117">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="8fb78-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fb78-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="8fb78-118">Relationships</span></span>
<span data-ttu-id="8fb78-119">无</span><span class="sxs-lookup"><span data-stu-id="8fb78-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fb78-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fb78-120">JSON Representation</span></span>
<span data-ttu-id="8fb78-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fb78-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



