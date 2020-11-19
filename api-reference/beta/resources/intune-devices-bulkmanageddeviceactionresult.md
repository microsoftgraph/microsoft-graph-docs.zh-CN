---
title: bulkManagedDeviceActionResult 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae016986f8c3216156a4855f06aa77929e6acefc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299499"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="56745-103">bulkManagedDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="56745-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="56745-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56745-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56745-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56745-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56745-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56745-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56745-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="56745-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="56745-108">属性</span><span class="sxs-lookup"><span data-stu-id="56745-108">Properties</span></span>
|<span data-ttu-id="56745-109">属性</span><span class="sxs-lookup"><span data-stu-id="56745-109">Property</span></span>|<span data-ttu-id="56745-110">类型</span><span class="sxs-lookup"><span data-stu-id="56745-110">Type</span></span>|<span data-ttu-id="56745-111">Description</span><span class="sxs-lookup"><span data-stu-id="56745-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56745-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="56745-112">successfulDeviceIds</span></span>|<span data-ttu-id="56745-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="56745-113">String collection</span></span>|<span data-ttu-id="56745-114">成功的设备</span><span class="sxs-lookup"><span data-stu-id="56745-114">Successful devices</span></span>|
|<span data-ttu-id="56745-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="56745-115">failedDeviceIds</span></span>|<span data-ttu-id="56745-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="56745-116">String collection</span></span>|<span data-ttu-id="56745-117">故障设备</span><span class="sxs-lookup"><span data-stu-id="56745-117">Failed devices</span></span>|
|<span data-ttu-id="56745-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="56745-118">notFoundDeviceIds</span></span>|<span data-ttu-id="56745-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="56745-119">String collection</span></span>|<span data-ttu-id="56745-120">找不到设备</span><span class="sxs-lookup"><span data-stu-id="56745-120">Not found devices</span></span>|
|<span data-ttu-id="56745-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="56745-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="56745-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="56745-122">String collection</span></span>|<span data-ttu-id="56745-123">不支持的设备</span><span class="sxs-lookup"><span data-stu-id="56745-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="56745-124">关系</span><span class="sxs-lookup"><span data-stu-id="56745-124">Relationships</span></span>
<span data-ttu-id="56745-125">无</span><span class="sxs-lookup"><span data-stu-id="56745-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56745-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56745-126">JSON Representation</span></span>
<span data-ttu-id="56745-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56745-127">Here is a JSON representation of the resource.</span></span>
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




