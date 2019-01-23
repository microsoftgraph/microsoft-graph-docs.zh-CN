---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 292dc926a626a2aca96312133eb6c9a850db39af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398049"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="6e740-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e740-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="6e740-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6e740-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e740-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e740-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e740-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e740-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e740-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6e740-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e740-108">Properties</span></span>
|<span data-ttu-id="6e740-109">属性</span><span class="sxs-lookup"><span data-stu-id="6e740-109">Property</span></span>|<span data-ttu-id="6e740-110">类型</span><span class="sxs-lookup"><span data-stu-id="6e740-110">Type</span></span>|<span data-ttu-id="6e740-111">说明</span><span class="sxs-lookup"><span data-stu-id="6e740-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e740-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="6e740-112">movieRating</span></span>|[<span data-ttu-id="6e740-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="6e740-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="6e740-114">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="6e740-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="6e740-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="6e740-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="6e740-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="6e740-116">tvRating</span></span>|[<span data-ttu-id="6e740-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6e740-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="6e740-118">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="6e740-118">TV rating selected for Canada.</span></span> <span data-ttu-id="6e740-119">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="6e740-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e740-120">关系</span><span class="sxs-lookup"><span data-stu-id="6e740-120">Relationships</span></span>
<span data-ttu-id="6e740-121">无</span><span class="sxs-lookup"><span data-stu-id="6e740-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e740-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e740-122">JSON Representation</span></span>
<span data-ttu-id="6e740-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e740-123">Here is a JSON representation of the resource.</span></span>
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




