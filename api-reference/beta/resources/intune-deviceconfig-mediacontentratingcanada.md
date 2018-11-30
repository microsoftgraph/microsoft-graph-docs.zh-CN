---
title: mediaContentRatingCanada 资源类型
description: 尚未记录
ms.openlocfilehash: e44af4a72aee8c97a12b3d8dcad767bba08ad005
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041822"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="f9160-103">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9160-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="f9160-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9160-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9160-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9160-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9160-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f9160-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9160-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9160-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f9160-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9160-108">Properties</span></span>
|<span data-ttu-id="f9160-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9160-109">Property</span></span>|<span data-ttu-id="f9160-110">类型</span><span class="sxs-lookup"><span data-stu-id="f9160-110">Type</span></span>|<span data-ttu-id="f9160-111">说明</span><span class="sxs-lookup"><span data-stu-id="f9160-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9160-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f9160-112">movieRating</span></span>|[<span data-ttu-id="f9160-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="f9160-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="f9160-114">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="f9160-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="f9160-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="f9160-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="f9160-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f9160-116">tvRating</span></span>|[<span data-ttu-id="f9160-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f9160-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="f9160-118">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="f9160-118">TV rating selected for Canada.</span></span> <span data-ttu-id="f9160-119">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f9160-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9160-120">关系</span><span class="sxs-lookup"><span data-stu-id="f9160-120">Relationships</span></span>
<span data-ttu-id="f9160-121">无</span><span class="sxs-lookup"><span data-stu-id="f9160-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9160-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9160-122">JSON Representation</span></span>
<span data-ttu-id="f9160-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9160-123">Here is a JSON representation of the resource.</span></span>
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





