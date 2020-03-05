---
title: reportRoot 资源类型
description: 表示一个历史记录报告实例的资源。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09d8e31be500151a36e8f365915ed8f08c5aae98
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447806"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="9830d-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="9830d-103">reportRoot resource type</span></span>

<span data-ttu-id="9830d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9830d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9830d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9830d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9830d-106">表示一个历史记录报告实例的资源。</span><span class="sxs-lookup"><span data-stu-id="9830d-106">The resource that represents an instance of History Reports.</span></span>

## <a name="methods"></a><span data-ttu-id="9830d-107">方法</span><span class="sxs-lookup"><span data-stu-id="9830d-107">Methods</span></span>
|<span data-ttu-id="9830d-108">方法</span><span class="sxs-lookup"><span data-stu-id="9830d-108">Method</span></span>|<span data-ttu-id="9830d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9830d-109">Return Type</span></span>|<span data-ttu-id="9830d-110">说明</span><span class="sxs-lookup"><span data-stu-id="9830d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9830d-111">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="9830d-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="9830d-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="9830d-112">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="9830d-113">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9830d-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="9830d-114">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="9830d-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="9830d-115">reportRoot</span><span class="sxs-lookup"><span data-stu-id="9830d-115">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="9830d-116">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9830d-116">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="9830d-117">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="9830d-117">**Device configuration**</span></span>|
|[<span data-ttu-id="9830d-118">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="9830d-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="9830d-119">报告</span><span class="sxs-lookup"><span data-stu-id="9830d-119">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="9830d-120">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="9830d-120">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="9830d-121">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="9830d-121">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="9830d-122">报告</span><span class="sxs-lookup"><span data-stu-id="9830d-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="9830d-123">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="9830d-123">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="9830d-124">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="9830d-124">**Troubleshooting**</span></span>|
|[<span data-ttu-id="9830d-125">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="9830d-125">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="9830d-126">报告</span><span class="sxs-lookup"><span data-stu-id="9830d-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="9830d-127">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="9830d-127">Not yet documented.</span></span>|
|[<span data-ttu-id="9830d-128">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="9830d-128">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="9830d-129">报告</span><span class="sxs-lookup"><span data-stu-id="9830d-129">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="9830d-130">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="9830d-130">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="9830d-131">属性</span><span class="sxs-lookup"><span data-stu-id="9830d-131">Properties</span></span>
|<span data-ttu-id="9830d-132">属性</span><span class="sxs-lookup"><span data-stu-id="9830d-132">Property</span></span>|<span data-ttu-id="9830d-133">类型</span><span class="sxs-lookup"><span data-stu-id="9830d-133">Type</span></span>|<span data-ttu-id="9830d-134">说明</span><span class="sxs-lookup"><span data-stu-id="9830d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9830d-135">id</span><span class="sxs-lookup"><span data-stu-id="9830d-135">id</span></span>|<span data-ttu-id="9830d-136">String</span><span class="sxs-lookup"><span data-stu-id="9830d-136">String</span></span>|<span data-ttu-id="9830d-137">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9830d-137">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9830d-138">关系</span><span class="sxs-lookup"><span data-stu-id="9830d-138">Relationships</span></span>
<span data-ttu-id="9830d-139">无</span><span class="sxs-lookup"><span data-stu-id="9830d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9830d-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9830d-140">JSON Representation</span></span>
<span data-ttu-id="9830d-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9830d-141">Here is a JSON representation of the resource.</span></span>
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

## <a name="example"></a><span data-ttu-id="9830d-142">示例</span><span class="sxs-lookup"><span data-stu-id="9830d-142">Example</span></span>

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

