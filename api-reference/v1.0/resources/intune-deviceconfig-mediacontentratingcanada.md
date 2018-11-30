---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
ms.openlocfilehash: 764bea688c5c7d86f675caafdc47fa42d4a7d37a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010617"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="5b5a0-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b5a0-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="5b5a0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b5a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b5a0-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5b5a0-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="5b5a0-106">属性</span><span class="sxs-lookup"><span data-stu-id="5b5a0-106">Properties</span></span>
|<span data-ttu-id="5b5a0-107">属性</span><span class="sxs-lookup"><span data-stu-id="5b5a0-107">Property</span></span>|<span data-ttu-id="5b5a0-108">类型</span><span class="sxs-lookup"><span data-stu-id="5b5a0-108">Type</span></span>|<span data-ttu-id="5b5a0-109">说明</span><span class="sxs-lookup"><span data-stu-id="5b5a0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b5a0-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="5b5a0-110">movieRating</span></span>|[<span data-ttu-id="5b5a0-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="5b5a0-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="5b5a0-112">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="5b5a0-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="5b5a0-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="5b5a0-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="5b5a0-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="5b5a0-114">tvRating</span></span>|[<span data-ttu-id="5b5a0-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5b5a0-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="5b5a0-116">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="5b5a0-116">TV rating selected for Canada.</span></span> <span data-ttu-id="5b5a0-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="5b5a0-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b5a0-118">关系</span><span class="sxs-lookup"><span data-stu-id="5b5a0-118">Relationships</span></span>
<span data-ttu-id="5b5a0-119">无</span><span class="sxs-lookup"><span data-stu-id="5b5a0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b5a0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b5a0-120">JSON Representation</span></span>
<span data-ttu-id="5b5a0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b5a0-121">Here is a JSON representation of the resource.</span></span>
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



