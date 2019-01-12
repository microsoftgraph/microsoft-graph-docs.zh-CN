---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3593c743d0b65d761abf18b7fdb4783d126c19f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928855"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="6f182-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f182-103">rgbColor resource type</span></span>

> <span data-ttu-id="6f182-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f182-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f182-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f182-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f182-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f182-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f182-107">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="6f182-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="6f182-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f182-108">Properties</span></span>
|<span data-ttu-id="6f182-109">属性</span><span class="sxs-lookup"><span data-stu-id="6f182-109">Property</span></span>|<span data-ttu-id="6f182-110">类型</span><span class="sxs-lookup"><span data-stu-id="6f182-110">Type</span></span>|<span data-ttu-id="6f182-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f182-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f182-112">r</span><span class="sxs-lookup"><span data-stu-id="6f182-112">r</span></span>|<span data-ttu-id="6f182-113">字节</span><span class="sxs-lookup"><span data-stu-id="6f182-113">Byte</span></span>|<span data-ttu-id="6f182-114">红色值</span><span class="sxs-lookup"><span data-stu-id="6f182-114">Red value</span></span>|
|<span data-ttu-id="6f182-115">g</span><span class="sxs-lookup"><span data-stu-id="6f182-115">g</span></span>|<span data-ttu-id="6f182-116">字节</span><span class="sxs-lookup"><span data-stu-id="6f182-116">Byte</span></span>|<span data-ttu-id="6f182-117">绿色值</span><span class="sxs-lookup"><span data-stu-id="6f182-117">Green value</span></span>|
|<span data-ttu-id="6f182-118">b</span><span class="sxs-lookup"><span data-stu-id="6f182-118">b</span></span>|<span data-ttu-id="6f182-119">字节</span><span class="sxs-lookup"><span data-stu-id="6f182-119">Byte</span></span>|<span data-ttu-id="6f182-120">蓝色值</span><span class="sxs-lookup"><span data-stu-id="6f182-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f182-121">关系</span><span class="sxs-lookup"><span data-stu-id="6f182-121">Relationships</span></span>
<span data-ttu-id="6f182-122">无</span><span class="sxs-lookup"><span data-stu-id="6f182-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f182-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f182-123">JSON Representation</span></span>
<span data-ttu-id="6f182-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f182-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```





