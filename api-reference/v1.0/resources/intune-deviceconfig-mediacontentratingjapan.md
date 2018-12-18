---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 1913b28b3020ffdc51edea1a8d93dd726d70efdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328467"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="225b4-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="225b4-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="225b4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="225b4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="225b4-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="225b4-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="225b4-106">属性</span><span class="sxs-lookup"><span data-stu-id="225b4-106">Properties</span></span>
|<span data-ttu-id="225b4-107">属性</span><span class="sxs-lookup"><span data-stu-id="225b4-107">Property</span></span>|<span data-ttu-id="225b4-108">类型</span><span class="sxs-lookup"><span data-stu-id="225b4-108">Type</span></span>|<span data-ttu-id="225b4-109">说明</span><span class="sxs-lookup"><span data-stu-id="225b4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="225b4-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="225b4-110">movieRating</span></span>|[<span data-ttu-id="225b4-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="225b4-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="225b4-112">分级日本所选的影片。</span><span class="sxs-lookup"><span data-stu-id="225b4-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="225b4-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="225b4-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="225b4-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="225b4-114">tvRating</span></span>|[<span data-ttu-id="225b4-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="225b4-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="225b4-116">日本选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="225b4-116">TV rating selected for Japan.</span></span> <span data-ttu-id="225b4-117">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="225b4-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="225b4-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="225b4-118">Relationships</span></span>
<span data-ttu-id="225b4-119">无</span><span class="sxs-lookup"><span data-stu-id="225b4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="225b4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="225b4-120">JSON Representation</span></span>
<span data-ttu-id="225b4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="225b4-121">Here is a JSON representation of the resource.</span></span>
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



