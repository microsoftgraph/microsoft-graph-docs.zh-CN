---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 505383227d1014f779cb558d43c18da29d3989aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395515"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="61d18-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="61d18-103">rgbColor resource type</span></span>

> <span data-ttu-id="61d18-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="61d18-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61d18-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="61d18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61d18-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61d18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61d18-107">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="61d18-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="61d18-108">属性</span><span class="sxs-lookup"><span data-stu-id="61d18-108">Properties</span></span>
|<span data-ttu-id="61d18-109">属性</span><span class="sxs-lookup"><span data-stu-id="61d18-109">Property</span></span>|<span data-ttu-id="61d18-110">类型</span><span class="sxs-lookup"><span data-stu-id="61d18-110">Type</span></span>|<span data-ttu-id="61d18-111">说明</span><span class="sxs-lookup"><span data-stu-id="61d18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d18-112">r</span><span class="sxs-lookup"><span data-stu-id="61d18-112">r</span></span>|<span data-ttu-id="61d18-113">字节</span><span class="sxs-lookup"><span data-stu-id="61d18-113">Byte</span></span>|<span data-ttu-id="61d18-114">红色值</span><span class="sxs-lookup"><span data-stu-id="61d18-114">Red value</span></span>|
|<span data-ttu-id="61d18-115">g</span><span class="sxs-lookup"><span data-stu-id="61d18-115">g</span></span>|<span data-ttu-id="61d18-116">字节</span><span class="sxs-lookup"><span data-stu-id="61d18-116">Byte</span></span>|<span data-ttu-id="61d18-117">绿色值</span><span class="sxs-lookup"><span data-stu-id="61d18-117">Green value</span></span>|
|<span data-ttu-id="61d18-118">b</span><span class="sxs-lookup"><span data-stu-id="61d18-118">b</span></span>|<span data-ttu-id="61d18-119">字节</span><span class="sxs-lookup"><span data-stu-id="61d18-119">Byte</span></span>|<span data-ttu-id="61d18-120">蓝色值</span><span class="sxs-lookup"><span data-stu-id="61d18-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d18-121">关系</span><span class="sxs-lookup"><span data-stu-id="61d18-121">Relationships</span></span>
<span data-ttu-id="61d18-122">无</span><span class="sxs-lookup"><span data-stu-id="61d18-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61d18-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61d18-123">JSON Representation</span></span>
<span data-ttu-id="61d18-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61d18-124">Here is a JSON representation of the resource.</span></span>
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




