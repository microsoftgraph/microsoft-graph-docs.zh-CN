---
title: bulkManagedDeviceActionResult 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0978367465fde92f9874e338a0de84da2a20403
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467346"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="edfb0-103">bulkManagedDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="edfb0-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="edfb0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edfb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edfb0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edfb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfb0-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="edfb0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="edfb0-107">属性</span><span class="sxs-lookup"><span data-stu-id="edfb0-107">Properties</span></span>
|<span data-ttu-id="edfb0-108">属性</span><span class="sxs-lookup"><span data-stu-id="edfb0-108">Property</span></span>|<span data-ttu-id="edfb0-109">类型</span><span class="sxs-lookup"><span data-stu-id="edfb0-109">Type</span></span>|<span data-ttu-id="edfb0-110">说明</span><span class="sxs-lookup"><span data-stu-id="edfb0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfb0-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="edfb0-111">successfulDeviceIds</span></span>|<span data-ttu-id="edfb0-112">String collection</span><span class="sxs-lookup"><span data-stu-id="edfb0-112">String collection</span></span>|<span data-ttu-id="edfb0-113">成功的设备</span><span class="sxs-lookup"><span data-stu-id="edfb0-113">Successful devices</span></span>|
|<span data-ttu-id="edfb0-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="edfb0-114">failedDeviceIds</span></span>|<span data-ttu-id="edfb0-115">String collection</span><span class="sxs-lookup"><span data-stu-id="edfb0-115">String collection</span></span>|<span data-ttu-id="edfb0-116">故障设备</span><span class="sxs-lookup"><span data-stu-id="edfb0-116">Failed devices</span></span>|
|<span data-ttu-id="edfb0-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="edfb0-117">notFoundDeviceIds</span></span>|<span data-ttu-id="edfb0-118">String collection</span><span class="sxs-lookup"><span data-stu-id="edfb0-118">String collection</span></span>|<span data-ttu-id="edfb0-119">找不到设备</span><span class="sxs-lookup"><span data-stu-id="edfb0-119">Not found devices</span></span>|
|<span data-ttu-id="edfb0-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="edfb0-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="edfb0-121">String collection</span><span class="sxs-lookup"><span data-stu-id="edfb0-121">String collection</span></span>|<span data-ttu-id="edfb0-122">不支持的设备</span><span class="sxs-lookup"><span data-stu-id="edfb0-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="edfb0-123">关系</span><span class="sxs-lookup"><span data-stu-id="edfb0-123">Relationships</span></span>
<span data-ttu-id="edfb0-124">无</span><span class="sxs-lookup"><span data-stu-id="edfb0-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edfb0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edfb0-125">JSON Representation</span></span>
<span data-ttu-id="edfb0-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edfb0-126">Here is a JSON representation of the resource.</span></span>
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





