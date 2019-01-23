---
title: bulkManagedDeviceActionResult 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d1b23efdb5b8eed16c6c66d72a13efaef9e38d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425839"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="2ce58-103">bulkManagedDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ce58-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="2ce58-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2ce58-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ce58-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2ce58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ce58-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ce58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ce58-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ce58-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2ce58-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ce58-108">Properties</span></span>
|<span data-ttu-id="2ce58-109">属性</span><span class="sxs-lookup"><span data-stu-id="2ce58-109">Property</span></span>|<span data-ttu-id="2ce58-110">类型</span><span class="sxs-lookup"><span data-stu-id="2ce58-110">Type</span></span>|<span data-ttu-id="2ce58-111">说明</span><span class="sxs-lookup"><span data-stu-id="2ce58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ce58-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2ce58-112">successfulDeviceIds</span></span>|<span data-ttu-id="2ce58-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="2ce58-113">String collection</span></span>|<span data-ttu-id="2ce58-114">成功的设备</span><span class="sxs-lookup"><span data-stu-id="2ce58-114">Successful devices</span></span>|
|<span data-ttu-id="2ce58-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2ce58-115">failedDeviceIds</span></span>|<span data-ttu-id="2ce58-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="2ce58-116">String collection</span></span>|<span data-ttu-id="2ce58-117">失败的设备</span><span class="sxs-lookup"><span data-stu-id="2ce58-117">Failed devices</span></span>|
|<span data-ttu-id="2ce58-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2ce58-118">notFoundDeviceIds</span></span>|<span data-ttu-id="2ce58-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="2ce58-119">String collection</span></span>|<span data-ttu-id="2ce58-120">未找到设备</span><span class="sxs-lookup"><span data-stu-id="2ce58-120">Not found devices</span></span>|
|<span data-ttu-id="2ce58-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2ce58-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="2ce58-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="2ce58-122">String collection</span></span>|<span data-ttu-id="2ce58-123">不受支持的设备</span><span class="sxs-lookup"><span data-stu-id="2ce58-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ce58-124">关系</span><span class="sxs-lookup"><span data-stu-id="2ce58-124">Relationships</span></span>
<span data-ttu-id="2ce58-125">无</span><span class="sxs-lookup"><span data-stu-id="2ce58-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ce58-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ce58-126">JSON Representation</span></span>
<span data-ttu-id="2ce58-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ce58-127">Here is a JSON representation of the resource.</span></span>
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




