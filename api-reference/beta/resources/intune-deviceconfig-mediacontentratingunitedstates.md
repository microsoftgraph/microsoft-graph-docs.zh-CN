---
title: mediaContentRatingUnitedStates 资源类型
description: 尚未记录
ms.openlocfilehash: d62d656c4fbd8744560ab191786d71b732fe6c21
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041643"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="c35b0-103">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="c35b0-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="c35b0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c35b0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c35b0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c35b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c35b0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c35b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c35b0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c35b0-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c35b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="c35b0-108">Properties</span></span>
|<span data-ttu-id="c35b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="c35b0-109">Property</span></span>|<span data-ttu-id="c35b0-110">类型</span><span class="sxs-lookup"><span data-stu-id="c35b0-110">Type</span></span>|<span data-ttu-id="c35b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="c35b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c35b0-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c35b0-112">movieRating</span></span>|[<span data-ttu-id="c35b0-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="c35b0-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="c35b0-114">分级美国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="c35b0-114">Movies rating selected for United States.</span></span> <span data-ttu-id="c35b0-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c35b0-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="c35b0-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c35b0-116">tvRating</span></span>|[<span data-ttu-id="c35b0-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c35b0-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="c35b0-118">美国的所选 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="c35b0-118">TV rating selected for United States.</span></span> <span data-ttu-id="c35b0-119">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c35b0-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c35b0-120">关系</span><span class="sxs-lookup"><span data-stu-id="c35b0-120">Relationships</span></span>
<span data-ttu-id="c35b0-121">无</span><span class="sxs-lookup"><span data-stu-id="c35b0-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c35b0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c35b0-122">JSON Representation</span></span>
<span data-ttu-id="c35b0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c35b0-123">Here is a JSON representation of the resource.</span></span>
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





