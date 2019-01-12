---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b4151b810fcfbc56c652492fff9fa1f3f841189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932180"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="4f524-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f524-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="4f524-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4f524-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f524-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4f524-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4f524-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f524-106">Properties</span></span>
|<span data-ttu-id="4f524-107">属性</span><span class="sxs-lookup"><span data-stu-id="4f524-107">Property</span></span>|<span data-ttu-id="4f524-108">类型</span><span class="sxs-lookup"><span data-stu-id="4f524-108">Type</span></span>|<span data-ttu-id="4f524-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f524-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f524-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="4f524-110">movieRating</span></span>|[<span data-ttu-id="4f524-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4f524-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="4f524-112">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="4f524-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="4f524-113">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="4f524-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="4f524-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="4f524-114">tvRating</span></span>|[<span data-ttu-id="4f524-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4f524-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="4f524-116">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="4f524-116">TV rating selected for Canada.</span></span> <span data-ttu-id="4f524-117">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="4f524-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f524-118">关系</span><span class="sxs-lookup"><span data-stu-id="4f524-118">Relationships</span></span>
<span data-ttu-id="4f524-119">无</span><span class="sxs-lookup"><span data-stu-id="4f524-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4f524-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f524-120">JSON Representation</span></span>
<span data-ttu-id="4f524-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f524-121">Here is a JSON representation of the resource.</span></span>
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



