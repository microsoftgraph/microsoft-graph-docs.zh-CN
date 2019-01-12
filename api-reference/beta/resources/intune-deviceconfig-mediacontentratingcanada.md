---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0e6b3c84801ecf1338a04e356d9141d4b45286de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980998"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="bf286-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf286-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="bf286-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf286-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf286-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf286-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf286-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bf286-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf286-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf286-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bf286-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf286-108">Properties</span></span>
|<span data-ttu-id="bf286-109">属性</span><span class="sxs-lookup"><span data-stu-id="bf286-109">Property</span></span>|<span data-ttu-id="bf286-110">类型</span><span class="sxs-lookup"><span data-stu-id="bf286-110">Type</span></span>|<span data-ttu-id="bf286-111">说明</span><span class="sxs-lookup"><span data-stu-id="bf286-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf286-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bf286-112">movieRating</span></span>|[<span data-ttu-id="bf286-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="bf286-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="bf286-114">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="bf286-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="bf286-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="bf286-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="bf286-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bf286-116">tvRating</span></span>|[<span data-ttu-id="bf286-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bf286-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="bf286-118">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="bf286-118">TV rating selected for Canada.</span></span> <span data-ttu-id="bf286-119">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="bf286-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf286-120">关系</span><span class="sxs-lookup"><span data-stu-id="bf286-120">Relationships</span></span>
<span data-ttu-id="bf286-121">无</span><span class="sxs-lookup"><span data-stu-id="bf286-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf286-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf286-122">JSON Representation</span></span>
<span data-ttu-id="bf286-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf286-123">Here is a JSON representation of the resource.</span></span>
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





