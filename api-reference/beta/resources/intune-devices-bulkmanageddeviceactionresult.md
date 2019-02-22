---
title: bulkManagedDeviceActionResult 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199fe08b4eaf339f17fdb67bb6dbcc0243fd90f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168332"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="f8a7e-103">bulkManagedDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8a7e-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="f8a7e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8a7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8a7e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8a7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8a7e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f8a7e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f8a7e-107">属性</span><span class="sxs-lookup"><span data-stu-id="f8a7e-107">Properties</span></span>
|<span data-ttu-id="f8a7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8a7e-108">Property</span></span>|<span data-ttu-id="f8a7e-109">类型</span><span class="sxs-lookup"><span data-stu-id="f8a7e-109">Type</span></span>|<span data-ttu-id="f8a7e-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8a7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8a7e-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="f8a7e-111">successfulDeviceIds</span></span>|<span data-ttu-id="f8a7e-112">String collection</span><span class="sxs-lookup"><span data-stu-id="f8a7e-112">String collection</span></span>|<span data-ttu-id="f8a7e-113">成功的设备</span><span class="sxs-lookup"><span data-stu-id="f8a7e-113">Successful devices</span></span>|
|<span data-ttu-id="f8a7e-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="f8a7e-114">failedDeviceIds</span></span>|<span data-ttu-id="f8a7e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="f8a7e-115">String collection</span></span>|<span data-ttu-id="f8a7e-116">故障设备</span><span class="sxs-lookup"><span data-stu-id="f8a7e-116">Failed devices</span></span>|
|<span data-ttu-id="f8a7e-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="f8a7e-117">notFoundDeviceIds</span></span>|<span data-ttu-id="f8a7e-118">String collection</span><span class="sxs-lookup"><span data-stu-id="f8a7e-118">String collection</span></span>|<span data-ttu-id="f8a7e-119">找不到设备</span><span class="sxs-lookup"><span data-stu-id="f8a7e-119">Not found devices</span></span>|
|<span data-ttu-id="f8a7e-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="f8a7e-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="f8a7e-121">String collection</span><span class="sxs-lookup"><span data-stu-id="f8a7e-121">String collection</span></span>|<span data-ttu-id="f8a7e-122">不支持的设备</span><span class="sxs-lookup"><span data-stu-id="f8a7e-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8a7e-123">关系</span><span class="sxs-lookup"><span data-stu-id="f8a7e-123">Relationships</span></span>
<span data-ttu-id="f8a7e-124">无</span><span class="sxs-lookup"><span data-stu-id="f8a7e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8a7e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8a7e-125">JSON Representation</span></span>
<span data-ttu-id="f8a7e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8a7e-126">Here is a JSON representation of the resource.</span></span>
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




