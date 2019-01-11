---
title: bulkManagedDeviceActionResult 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7aa0d49182908a960130e202fd4cf096c2c16c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872245"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="e0036-103">bulkManagedDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0036-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="e0036-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0036-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0036-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0036-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0036-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0036-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0036-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e0036-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e0036-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0036-108">Properties</span></span>
|<span data-ttu-id="e0036-109">属性</span><span class="sxs-lookup"><span data-stu-id="e0036-109">Property</span></span>|<span data-ttu-id="e0036-110">类型</span><span class="sxs-lookup"><span data-stu-id="e0036-110">Type</span></span>|<span data-ttu-id="e0036-111">Description</span><span class="sxs-lookup"><span data-stu-id="e0036-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0036-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e0036-112">successfulDeviceIds</span></span>|<span data-ttu-id="e0036-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="e0036-113">String collection</span></span>|<span data-ttu-id="e0036-114">成功的设备</span><span class="sxs-lookup"><span data-stu-id="e0036-114">Successful devices</span></span>|
|<span data-ttu-id="e0036-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e0036-115">failedDeviceIds</span></span>|<span data-ttu-id="e0036-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="e0036-116">String collection</span></span>|<span data-ttu-id="e0036-117">失败的设备</span><span class="sxs-lookup"><span data-stu-id="e0036-117">Failed devices</span></span>|
|<span data-ttu-id="e0036-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e0036-118">notFoundDeviceIds</span></span>|<span data-ttu-id="e0036-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="e0036-119">String collection</span></span>|<span data-ttu-id="e0036-120">未找到设备</span><span class="sxs-lookup"><span data-stu-id="e0036-120">Not found devices</span></span>|
|<span data-ttu-id="e0036-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e0036-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="e0036-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="e0036-122">String collection</span></span>|<span data-ttu-id="e0036-123">不受支持的设备</span><span class="sxs-lookup"><span data-stu-id="e0036-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0036-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="e0036-124">Relationships</span></span>
<span data-ttu-id="e0036-125">无</span><span class="sxs-lookup"><span data-stu-id="e0036-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0036-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0036-126">JSON Representation</span></span>
<span data-ttu-id="e0036-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0036-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```





