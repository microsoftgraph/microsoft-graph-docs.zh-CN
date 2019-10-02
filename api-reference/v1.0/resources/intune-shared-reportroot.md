---
title: reportRoot 资源类型
description: 表示一个历史记录报告实例的资源。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9b2f70bb3286b47fb92985ec3055c0d3470fb23
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360158"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="33145-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="33145-103">reportRoot resource type</span></span>

> <span data-ttu-id="33145-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33145-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33145-105">表示一个历史记录报告实例的资源。</span><span class="sxs-lookup"><span data-stu-id="33145-105">The resource that represents an instance of History Reports.</span></span>

## <a name="methods"></a><span data-ttu-id="33145-106">方法</span><span class="sxs-lookup"><span data-stu-id="33145-106">Methods</span></span>
|<span data-ttu-id="33145-107">方法</span><span class="sxs-lookup"><span data-stu-id="33145-107">Method</span></span>|<span data-ttu-id="33145-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="33145-108">Return Type</span></span>|<span data-ttu-id="33145-109">说明</span><span class="sxs-lookup"><span data-stu-id="33145-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33145-110">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="33145-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="33145-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="33145-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="33145-112">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33145-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="33145-113">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="33145-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="33145-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="33145-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="33145-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="33145-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="33145-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="33145-116">**Device configuration**</span></span>|
|[<span data-ttu-id="33145-117">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="33145-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="33145-118">报告</span><span class="sxs-lookup"><span data-stu-id="33145-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="33145-119">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="33145-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="33145-120">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="33145-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="33145-121">报告</span><span class="sxs-lookup"><span data-stu-id="33145-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="33145-122">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="33145-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="33145-123">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="33145-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="33145-124">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="33145-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="33145-125">报告</span><span class="sxs-lookup"><span data-stu-id="33145-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="33145-126">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="33145-126">Not yet documented.</span></span>|
|[<span data-ttu-id="33145-127">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="33145-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="33145-128">报告</span><span class="sxs-lookup"><span data-stu-id="33145-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="33145-129">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="33145-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="33145-130">属性</span><span class="sxs-lookup"><span data-stu-id="33145-130">Properties</span></span>
|<span data-ttu-id="33145-131">属性</span><span class="sxs-lookup"><span data-stu-id="33145-131">Property</span></span>|<span data-ttu-id="33145-132">类型</span><span class="sxs-lookup"><span data-stu-id="33145-132">Type</span></span>|<span data-ttu-id="33145-133">说明</span><span class="sxs-lookup"><span data-stu-id="33145-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33145-134">id</span><span class="sxs-lookup"><span data-stu-id="33145-134">id</span></span>|<span data-ttu-id="33145-135">String</span><span class="sxs-lookup"><span data-stu-id="33145-135">String</span></span>|<span data-ttu-id="33145-136">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="33145-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33145-137">关系</span><span class="sxs-lookup"><span data-stu-id="33145-137">Relationships</span></span>
<span data-ttu-id="33145-138">无</span><span class="sxs-lookup"><span data-stu-id="33145-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33145-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33145-139">JSON Representation</span></span>
<span data-ttu-id="33145-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33145-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a><span data-ttu-id="33145-141">示例</span><span class="sxs-lookup"><span data-stu-id="33145-141">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```

