---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60208f2bace4826f06ff5a81f02bc087211d52a1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777898"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="356aa-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="356aa-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="356aa-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="356aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="356aa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="356aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="356aa-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="356aa-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="356aa-107">属性</span><span class="sxs-lookup"><span data-stu-id="356aa-107">Properties</span></span>
|<span data-ttu-id="356aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="356aa-108">Property</span></span>|<span data-ttu-id="356aa-109">类型</span><span class="sxs-lookup"><span data-stu-id="356aa-109">Type</span></span>|<span data-ttu-id="356aa-110">说明</span><span class="sxs-lookup"><span data-stu-id="356aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="356aa-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="356aa-111">movieRating</span></span>|[<span data-ttu-id="356aa-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="356aa-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="356aa-113">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="356aa-113">Movies rating selected for United States.</span></span> <span data-ttu-id="356aa-114">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="356aa-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="356aa-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="356aa-115">tvRating</span></span>|[<span data-ttu-id="356aa-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="356aa-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="356aa-117">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="356aa-117">TV rating selected for United States.</span></span> <span data-ttu-id="356aa-118">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="356aa-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="356aa-119">关系</span><span class="sxs-lookup"><span data-stu-id="356aa-119">Relationships</span></span>
<span data-ttu-id="356aa-120">无</span><span class="sxs-lookup"><span data-stu-id="356aa-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="356aa-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="356aa-121">JSON Representation</span></span>
<span data-ttu-id="356aa-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="356aa-122">Here is a JSON representation of the resource.</span></span>
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





