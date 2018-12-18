---
title: mediaContentRatingJapan 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 98af9a6678b26c2cef15950cae769f3057009479
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337427"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="03426-103">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="03426-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="03426-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03426-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03426-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03426-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03426-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="03426-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03426-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03426-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="03426-108">属性</span><span class="sxs-lookup"><span data-stu-id="03426-108">Properties</span></span>
|<span data-ttu-id="03426-109">属性</span><span class="sxs-lookup"><span data-stu-id="03426-109">Property</span></span>|<span data-ttu-id="03426-110">类型</span><span class="sxs-lookup"><span data-stu-id="03426-110">Type</span></span>|<span data-ttu-id="03426-111">说明</span><span class="sxs-lookup"><span data-stu-id="03426-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03426-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="03426-112">movieRating</span></span>|[<span data-ttu-id="03426-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="03426-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="03426-114">分级日本所选的影片。</span><span class="sxs-lookup"><span data-stu-id="03426-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="03426-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="03426-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="03426-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="03426-116">tvRating</span></span>|[<span data-ttu-id="03426-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="03426-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="03426-118">日本选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="03426-118">TV rating selected for Japan.</span></span> <span data-ttu-id="03426-119">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="03426-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03426-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="03426-120">Relationships</span></span>
<span data-ttu-id="03426-121">无</span><span class="sxs-lookup"><span data-stu-id="03426-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03426-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03426-122">JSON Representation</span></span>
<span data-ttu-id="03426-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03426-123">Here is a JSON representation of the resource.</span></span>
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





