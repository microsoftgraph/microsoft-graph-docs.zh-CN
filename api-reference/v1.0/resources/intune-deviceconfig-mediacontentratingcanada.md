---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 310d68ea3ee0fa563b9fe413e26bace51251025a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312493"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="3687b-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="3687b-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="3687b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3687b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3687b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3687b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3687b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3687b-106">Properties</span></span>
|<span data-ttu-id="3687b-107">属性</span><span class="sxs-lookup"><span data-stu-id="3687b-107">Property</span></span>|<span data-ttu-id="3687b-108">类型</span><span class="sxs-lookup"><span data-stu-id="3687b-108">Type</span></span>|<span data-ttu-id="3687b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3687b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3687b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="3687b-110">movieRating</span></span>|[<span data-ttu-id="3687b-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="3687b-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="3687b-112">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="3687b-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="3687b-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="3687b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="3687b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="3687b-114">tvRating</span></span>|[<span data-ttu-id="3687b-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3687b-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="3687b-116">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="3687b-116">TV rating selected for Canada.</span></span> <span data-ttu-id="3687b-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="3687b-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3687b-118">关系</span><span class="sxs-lookup"><span data-stu-id="3687b-118">Relationships</span></span>
<span data-ttu-id="3687b-119">无</span><span class="sxs-lookup"><span data-stu-id="3687b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3687b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3687b-120">JSON Representation</span></span>
<span data-ttu-id="3687b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3687b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



