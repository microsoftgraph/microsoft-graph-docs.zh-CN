---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
ms.openlocfilehash: 15e905355133545db2cdf0864fcbba7e9c226183
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009007"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="a808c-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="a808c-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="a808c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a808c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a808c-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a808c-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a808c-106">属性</span><span class="sxs-lookup"><span data-stu-id="a808c-106">Properties</span></span>
|<span data-ttu-id="a808c-107">属性</span><span class="sxs-lookup"><span data-stu-id="a808c-107">Property</span></span>|<span data-ttu-id="a808c-108">类型</span><span class="sxs-lookup"><span data-stu-id="a808c-108">Type</span></span>|<span data-ttu-id="a808c-109">说明</span><span class="sxs-lookup"><span data-stu-id="a808c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a808c-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a808c-110">movieRating</span></span>|[<span data-ttu-id="a808c-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="a808c-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="a808c-112">分级日本所选的影片。</span><span class="sxs-lookup"><span data-stu-id="a808c-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="a808c-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="a808c-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a808c-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a808c-114">tvRating</span></span>|[<span data-ttu-id="a808c-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a808c-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="a808c-116">日本选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="a808c-116">TV rating selected for Japan.</span></span> <span data-ttu-id="a808c-117">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="a808c-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a808c-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="a808c-118">Relationships</span></span>
<span data-ttu-id="a808c-119">无</span><span class="sxs-lookup"><span data-stu-id="a808c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a808c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a808c-120">JSON Representation</span></span>
<span data-ttu-id="a808c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a808c-121">Here is a JSON representation of the resource.</span></span>
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



