---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60f673e31014eb4da027a58ea29099d9d8aa18e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425832"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="69331-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="69331-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="69331-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="69331-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69331-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69331-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69331-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69331-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69331-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="69331-108">属性</span><span class="sxs-lookup"><span data-stu-id="69331-108">Properties</span></span>
|<span data-ttu-id="69331-109">属性</span><span class="sxs-lookup"><span data-stu-id="69331-109">Property</span></span>|<span data-ttu-id="69331-110">类型</span><span class="sxs-lookup"><span data-stu-id="69331-110">Type</span></span>|<span data-ttu-id="69331-111">说明</span><span class="sxs-lookup"><span data-stu-id="69331-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69331-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="69331-112">movieRating</span></span>|[<span data-ttu-id="69331-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="69331-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="69331-114">分级美国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="69331-114">Movies rating selected for United States.</span></span> <span data-ttu-id="69331-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="69331-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="69331-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="69331-116">tvRating</span></span>|[<span data-ttu-id="69331-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="69331-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="69331-118">美国的所选 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="69331-118">TV rating selected for United States.</span></span> <span data-ttu-id="69331-119">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="69331-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69331-120">关系</span><span class="sxs-lookup"><span data-stu-id="69331-120">Relationships</span></span>
<span data-ttu-id="69331-121">无</span><span class="sxs-lookup"><span data-stu-id="69331-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69331-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69331-122">JSON Representation</span></span>
<span data-ttu-id="69331-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69331-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```




