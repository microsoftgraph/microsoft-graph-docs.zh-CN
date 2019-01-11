---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c40691556e9a8f674256c040a98f22e6ef9d717f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857307"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="aa003-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa003-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="aa003-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aa003-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa003-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aa003-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="aa003-106">属性</span><span class="sxs-lookup"><span data-stu-id="aa003-106">Properties</span></span>
|<span data-ttu-id="aa003-107">属性</span><span class="sxs-lookup"><span data-stu-id="aa003-107">Property</span></span>|<span data-ttu-id="aa003-108">类型</span><span class="sxs-lookup"><span data-stu-id="aa003-108">Type</span></span>|<span data-ttu-id="aa003-109">说明</span><span class="sxs-lookup"><span data-stu-id="aa003-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa003-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="aa003-110">movieRating</span></span>|[<span data-ttu-id="aa003-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="aa003-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="aa003-112">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="aa003-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="aa003-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="aa003-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="aa003-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="aa003-114">tvRating</span></span>|[<span data-ttu-id="aa003-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="aa003-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="aa003-116">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="aa003-116">TV rating selected for Canada.</span></span> <span data-ttu-id="aa003-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="aa003-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa003-118">关系</span><span class="sxs-lookup"><span data-stu-id="aa003-118">Relationships</span></span>
<span data-ttu-id="aa003-119">无</span><span class="sxs-lookup"><span data-stu-id="aa003-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aa003-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa003-120">JSON Representation</span></span>
<span data-ttu-id="aa003-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa003-121">Here is a JSON representation of the resource.</span></span>
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



