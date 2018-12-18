---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: b69e09684097ffbd85cf8117e4dd17779cbc5c67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319451"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="80a10-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="80a10-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="80a10-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80a10-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a10-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="80a10-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="80a10-106">属性</span><span class="sxs-lookup"><span data-stu-id="80a10-106">Properties</span></span>
|<span data-ttu-id="80a10-107">属性</span><span class="sxs-lookup"><span data-stu-id="80a10-107">Property</span></span>|<span data-ttu-id="80a10-108">类型</span><span class="sxs-lookup"><span data-stu-id="80a10-108">Type</span></span>|<span data-ttu-id="80a10-109">说明</span><span class="sxs-lookup"><span data-stu-id="80a10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a10-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="80a10-110">movieRating</span></span>|[<span data-ttu-id="80a10-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="80a10-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="80a10-112">分级美国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="80a10-112">Movies rating selected for United States.</span></span> <span data-ttu-id="80a10-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="80a10-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="80a10-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="80a10-114">tvRating</span></span>|[<span data-ttu-id="80a10-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="80a10-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="80a10-116">美国的所选 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="80a10-116">TV rating selected for United States.</span></span> <span data-ttu-id="80a10-117">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="80a10-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80a10-118">关系</span><span class="sxs-lookup"><span data-stu-id="80a10-118">Relationships</span></span>
<span data-ttu-id="80a10-119">无</span><span class="sxs-lookup"><span data-stu-id="80a10-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80a10-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80a10-120">JSON Representation</span></span>
<span data-ttu-id="80a10-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80a10-121">Here is a JSON representation of the resource.</span></span>
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



