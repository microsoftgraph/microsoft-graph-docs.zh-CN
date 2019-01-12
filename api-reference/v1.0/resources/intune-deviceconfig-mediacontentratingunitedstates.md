---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e37a707b7ad190ddc1f3206f149d0dcc3c1aad3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959221"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="28b3a-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="28b3a-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="28b3a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="28b3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28b3a-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="28b3a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="28b3a-106">属性</span><span class="sxs-lookup"><span data-stu-id="28b3a-106">Properties</span></span>
|<span data-ttu-id="28b3a-107">属性</span><span class="sxs-lookup"><span data-stu-id="28b3a-107">Property</span></span>|<span data-ttu-id="28b3a-108">类型</span><span class="sxs-lookup"><span data-stu-id="28b3a-108">Type</span></span>|<span data-ttu-id="28b3a-109">说明</span><span class="sxs-lookup"><span data-stu-id="28b3a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b3a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="28b3a-110">movieRating</span></span>|[<span data-ttu-id="28b3a-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="28b3a-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="28b3a-112">分级美国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="28b3a-112">Movies rating selected for United States.</span></span> <span data-ttu-id="28b3a-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="28b3a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="28b3a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="28b3a-114">tvRating</span></span>|[<span data-ttu-id="28b3a-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="28b3a-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="28b3a-116">美国的所选 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="28b3a-116">TV rating selected for United States.</span></span> <span data-ttu-id="28b3a-117">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="28b3a-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28b3a-118">关系</span><span class="sxs-lookup"><span data-stu-id="28b3a-118">Relationships</span></span>
<span data-ttu-id="28b3a-119">无</span><span class="sxs-lookup"><span data-stu-id="28b3a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28b3a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28b3a-120">JSON Representation</span></span>
<span data-ttu-id="28b3a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28b3a-121">Here is a JSON representation of the resource.</span></span>
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



