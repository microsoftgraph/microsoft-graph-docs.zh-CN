---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9af3916d29bfc3f48ee3d4c04dc17ab1f0fa3045
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707162"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="9bdd6-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="9bdd6-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="9bdd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bdd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bdd6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bdd6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bdd6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9bdd6-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9bdd6-108">属性</span><span class="sxs-lookup"><span data-stu-id="9bdd6-108">Properties</span></span>
|<span data-ttu-id="9bdd6-109">属性</span><span class="sxs-lookup"><span data-stu-id="9bdd6-109">Property</span></span>|<span data-ttu-id="9bdd6-110">类型</span><span class="sxs-lookup"><span data-stu-id="9bdd6-110">Type</span></span>|<span data-ttu-id="9bdd6-111">说明</span><span class="sxs-lookup"><span data-stu-id="9bdd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bdd6-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="9bdd6-112">movieRating</span></span>|[<span data-ttu-id="9bdd6-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="9bdd6-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="9bdd6-114">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-114">Movies rating selected for United States.</span></span> <span data-ttu-id="9bdd6-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="9bdd6-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="9bdd6-116">tvRating</span></span>|[<span data-ttu-id="9bdd6-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9bdd6-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="9bdd6-118">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-118">TV rating selected for United States.</span></span> <span data-ttu-id="9bdd6-119">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bdd6-120">关系</span><span class="sxs-lookup"><span data-stu-id="9bdd6-120">Relationships</span></span>
<span data-ttu-id="9bdd6-121">无</span><span class="sxs-lookup"><span data-stu-id="9bdd6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bdd6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9bdd6-122">JSON Representation</span></span>
<span data-ttu-id="9bdd6-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bdd6-123">Here is a JSON representation of the resource.</span></span>
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





