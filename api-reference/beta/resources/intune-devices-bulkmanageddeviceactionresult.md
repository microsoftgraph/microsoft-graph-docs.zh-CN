---
title: bulkManagedDeviceActionResult 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a7b5e719e837dbd175fa634aea2082f5b0b142b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999988"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="875e2-103">bulkManagedDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="875e2-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="875e2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="875e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="875e2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="875e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="875e2-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="875e2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="875e2-107">属性</span><span class="sxs-lookup"><span data-stu-id="875e2-107">Properties</span></span>
|<span data-ttu-id="875e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="875e2-108">Property</span></span>|<span data-ttu-id="875e2-109">类型</span><span class="sxs-lookup"><span data-stu-id="875e2-109">Type</span></span>|<span data-ttu-id="875e2-110">说明</span><span class="sxs-lookup"><span data-stu-id="875e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="875e2-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="875e2-111">successfulDeviceIds</span></span>|<span data-ttu-id="875e2-112">String collection</span><span class="sxs-lookup"><span data-stu-id="875e2-112">String collection</span></span>|<span data-ttu-id="875e2-113">成功的设备</span><span class="sxs-lookup"><span data-stu-id="875e2-113">Successful devices</span></span>|
|<span data-ttu-id="875e2-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="875e2-114">failedDeviceIds</span></span>|<span data-ttu-id="875e2-115">String collection</span><span class="sxs-lookup"><span data-stu-id="875e2-115">String collection</span></span>|<span data-ttu-id="875e2-116">故障设备</span><span class="sxs-lookup"><span data-stu-id="875e2-116">Failed devices</span></span>|
|<span data-ttu-id="875e2-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="875e2-117">notFoundDeviceIds</span></span>|<span data-ttu-id="875e2-118">String collection</span><span class="sxs-lookup"><span data-stu-id="875e2-118">String collection</span></span>|<span data-ttu-id="875e2-119">找不到设备</span><span class="sxs-lookup"><span data-stu-id="875e2-119">Not found devices</span></span>|
|<span data-ttu-id="875e2-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="875e2-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="875e2-121">String collection</span><span class="sxs-lookup"><span data-stu-id="875e2-121">String collection</span></span>|<span data-ttu-id="875e2-122">不支持的设备</span><span class="sxs-lookup"><span data-stu-id="875e2-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="875e2-123">关系</span><span class="sxs-lookup"><span data-stu-id="875e2-123">Relationships</span></span>
<span data-ttu-id="875e2-124">无</span><span class="sxs-lookup"><span data-stu-id="875e2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="875e2-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="875e2-125">JSON Representation</span></span>
<span data-ttu-id="875e2-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="875e2-126">Here is a JSON representation of the resource.</span></span>
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





