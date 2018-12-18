---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
ms.openlocfilehash: b469533b8ee7e54e99b09be08870045d759f5322
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350958"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="a7609-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7609-103">rgbColor resource type</span></span>

> <span data-ttu-id="a7609-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7609-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7609-105">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="a7609-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="a7609-106">属性</span><span class="sxs-lookup"><span data-stu-id="a7609-106">Properties</span></span>
|<span data-ttu-id="a7609-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7609-107">Property</span></span>|<span data-ttu-id="a7609-108">类型</span><span class="sxs-lookup"><span data-stu-id="a7609-108">Type</span></span>|<span data-ttu-id="a7609-109">说明</span><span class="sxs-lookup"><span data-stu-id="a7609-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7609-110">r</span><span class="sxs-lookup"><span data-stu-id="a7609-110">r</span></span>|<span data-ttu-id="a7609-111">字节</span><span class="sxs-lookup"><span data-stu-id="a7609-111">Byte</span></span>|<span data-ttu-id="a7609-112">红色值</span><span class="sxs-lookup"><span data-stu-id="a7609-112">Red value</span></span>|
|<span data-ttu-id="a7609-113">g</span><span class="sxs-lookup"><span data-stu-id="a7609-113">g</span></span>|<span data-ttu-id="a7609-114">字节</span><span class="sxs-lookup"><span data-stu-id="a7609-114">Byte</span></span>|<span data-ttu-id="a7609-115">绿色值</span><span class="sxs-lookup"><span data-stu-id="a7609-115">Green value</span></span>|
|<span data-ttu-id="a7609-116">b</span><span class="sxs-lookup"><span data-stu-id="a7609-116">b</span></span>|<span data-ttu-id="a7609-117">字节</span><span class="sxs-lookup"><span data-stu-id="a7609-117">Byte</span></span>|<span data-ttu-id="a7609-118">蓝色值</span><span class="sxs-lookup"><span data-stu-id="a7609-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7609-119">关系</span><span class="sxs-lookup"><span data-stu-id="a7609-119">Relationships</span></span>
<span data-ttu-id="a7609-120">无</span><span class="sxs-lookup"><span data-stu-id="a7609-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7609-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7609-121">JSON Representation</span></span>
<span data-ttu-id="a7609-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7609-122">Here is a JSON representation of the resource.</span></span>
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



