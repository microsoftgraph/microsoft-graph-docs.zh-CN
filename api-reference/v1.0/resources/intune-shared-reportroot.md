---
title: reportRoot 资源类型
description: 表示一个历史记录报告实例的资源。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 98f29935304c5eac2262049f76a9bcf006aa694b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264090"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="f0167-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0167-103">reportRoot resource type</span></span>

> <span data-ttu-id="f0167-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0167-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0167-105">表示一个历史记录报告实例的资源。</span><span class="sxs-lookup"><span data-stu-id="f0167-105">The resource that represents an instance of History Reports.</span></span>

## <a name="methods"></a><span data-ttu-id="f0167-106">方法</span><span class="sxs-lookup"><span data-stu-id="f0167-106">Methods</span></span>
|<span data-ttu-id="f0167-107">方法</span><span class="sxs-lookup"><span data-stu-id="f0167-107">Method</span></span>|<span data-ttu-id="f0167-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f0167-108">Return Type</span></span>|<span data-ttu-id="f0167-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0167-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f0167-110">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="f0167-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="f0167-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="f0167-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="f0167-112">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0167-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="f0167-113">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="f0167-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="f0167-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="f0167-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="f0167-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0167-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="f0167-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="f0167-116">**Device configuration**</span></span>|
|[<span data-ttu-id="f0167-117">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="f0167-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="f0167-118">报告</span><span class="sxs-lookup"><span data-stu-id="f0167-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f0167-119">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f0167-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="f0167-120">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="f0167-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="f0167-121">报告</span><span class="sxs-lookup"><span data-stu-id="f0167-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f0167-122">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f0167-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="f0167-123">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="f0167-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="f0167-124">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="f0167-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="f0167-125">报告</span><span class="sxs-lookup"><span data-stu-id="f0167-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f0167-126">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="f0167-126">Not yet documented.</span></span>|
|[<span data-ttu-id="f0167-127">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="f0167-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="f0167-128">报告</span><span class="sxs-lookup"><span data-stu-id="f0167-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f0167-129">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="f0167-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="f0167-130">属性</span><span class="sxs-lookup"><span data-stu-id="f0167-130">Properties</span></span>
|<span data-ttu-id="f0167-131">属性</span><span class="sxs-lookup"><span data-stu-id="f0167-131">Property</span></span>|<span data-ttu-id="f0167-132">类型</span><span class="sxs-lookup"><span data-stu-id="f0167-132">Type</span></span>|<span data-ttu-id="f0167-133">说明</span><span class="sxs-lookup"><span data-stu-id="f0167-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0167-134">id</span><span class="sxs-lookup"><span data-stu-id="f0167-134">id</span></span>|<span data-ttu-id="f0167-135">String</span><span class="sxs-lookup"><span data-stu-id="f0167-135">String</span></span>|<span data-ttu-id="f0167-136">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f0167-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0167-137">关系</span><span class="sxs-lookup"><span data-stu-id="f0167-137">Relationships</span></span>
<span data-ttu-id="f0167-138">无</span><span class="sxs-lookup"><span data-stu-id="f0167-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0167-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0167-139">JSON Representation</span></span>
<span data-ttu-id="f0167-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0167-140">Here is a JSON representation of the resource.</span></span>
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

## <a name="example"></a><span data-ttu-id="f0167-141">示例</span><span class="sxs-lookup"><span data-stu-id="f0167-141">Example</span></span>

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
