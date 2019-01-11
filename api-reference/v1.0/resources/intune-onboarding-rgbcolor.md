---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74845224469c824b54090994e39288aba57bb8d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873057"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="3dd26-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="3dd26-103">rgbColor resource type</span></span>

> <span data-ttu-id="3dd26-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3dd26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3dd26-105">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="3dd26-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="3dd26-106">属性</span><span class="sxs-lookup"><span data-stu-id="3dd26-106">Properties</span></span>
|<span data-ttu-id="3dd26-107">属性</span><span class="sxs-lookup"><span data-stu-id="3dd26-107">Property</span></span>|<span data-ttu-id="3dd26-108">类型</span><span class="sxs-lookup"><span data-stu-id="3dd26-108">Type</span></span>|<span data-ttu-id="3dd26-109">说明</span><span class="sxs-lookup"><span data-stu-id="3dd26-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dd26-110">r</span><span class="sxs-lookup"><span data-stu-id="3dd26-110">r</span></span>|<span data-ttu-id="3dd26-111">字节</span><span class="sxs-lookup"><span data-stu-id="3dd26-111">Byte</span></span>|<span data-ttu-id="3dd26-112">红色值</span><span class="sxs-lookup"><span data-stu-id="3dd26-112">Red value</span></span>|
|<span data-ttu-id="3dd26-113">g</span><span class="sxs-lookup"><span data-stu-id="3dd26-113">g</span></span>|<span data-ttu-id="3dd26-114">字节</span><span class="sxs-lookup"><span data-stu-id="3dd26-114">Byte</span></span>|<span data-ttu-id="3dd26-115">绿色值</span><span class="sxs-lookup"><span data-stu-id="3dd26-115">Green value</span></span>|
|<span data-ttu-id="3dd26-116">b</span><span class="sxs-lookup"><span data-stu-id="3dd26-116">b</span></span>|<span data-ttu-id="3dd26-117">字节</span><span class="sxs-lookup"><span data-stu-id="3dd26-117">Byte</span></span>|<span data-ttu-id="3dd26-118">蓝色值</span><span class="sxs-lookup"><span data-stu-id="3dd26-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dd26-119">关系</span><span class="sxs-lookup"><span data-stu-id="3dd26-119">Relationships</span></span>
<span data-ttu-id="3dd26-120">无</span><span class="sxs-lookup"><span data-stu-id="3dd26-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3dd26-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3dd26-121">JSON Representation</span></span>
<span data-ttu-id="3dd26-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dd26-122">Here is a JSON representation of the resource.</span></span>
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



