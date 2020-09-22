---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccfd31d7e47d4a4e08a63e163661c4a2a82da7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052696"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="a4e09-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4e09-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="a4e09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4e09-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4e09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4e09-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4e09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4e09-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a4e09-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a4e09-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4e09-108">Properties</span></span>
|<span data-ttu-id="a4e09-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4e09-109">Property</span></span>|<span data-ttu-id="a4e09-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4e09-110">Type</span></span>|<span data-ttu-id="a4e09-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4e09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4e09-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="a4e09-112">movieRating</span></span>|[<span data-ttu-id="a4e09-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="a4e09-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="a4e09-114">为美国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="a4e09-114">Movies rating selected for United States.</span></span> <span data-ttu-id="a4e09-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted` 或 `adults`。</span><span class="sxs-lookup"><span data-stu-id="a4e09-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="a4e09-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="a4e09-116">tvRating</span></span>|[<span data-ttu-id="a4e09-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a4e09-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="a4e09-118">为美国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="a4e09-118">TV rating selected for United States.</span></span> <span data-ttu-id="a4e09-119">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="a4e09-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4e09-120">关系</span><span class="sxs-lookup"><span data-stu-id="a4e09-120">Relationships</span></span>
<span data-ttu-id="a4e09-121">无</span><span class="sxs-lookup"><span data-stu-id="a4e09-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4e09-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4e09-122">JSON Representation</span></span>
<span data-ttu-id="a4e09-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4e09-123">Here is a JSON representation of the resource.</span></span>
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






