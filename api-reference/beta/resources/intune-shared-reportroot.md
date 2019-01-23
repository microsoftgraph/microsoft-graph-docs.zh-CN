---
title: reportRoot 资源类型
description: 表示的设备或疑难解答的报告，具体取决于上下文实例的资源。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421331"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="1ba69-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ba69-103">reportRoot resource type</span></span>

> <span data-ttu-id="1ba69-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1ba69-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1ba69-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1ba69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ba69-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ba69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ba69-107">表示的设备或疑难解答的报告，具体取决于上下文实例的资源。</span><span class="sxs-lookup"><span data-stu-id="1ba69-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="1ba69-108">方法</span><span class="sxs-lookup"><span data-stu-id="1ba69-108">Methods</span></span>
|<span data-ttu-id="1ba69-109">方法</span><span class="sxs-lookup"><span data-stu-id="1ba69-109">Method</span></span>|<span data-ttu-id="1ba69-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ba69-110">Return Type</span></span>|<span data-ttu-id="1ba69-111">说明</span><span class="sxs-lookup"><span data-stu-id="1ba69-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ba69-112">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="1ba69-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="1ba69-113">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ba69-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="1ba69-114">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="1ba69-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="1ba69-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba69-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="1ba69-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="1ba69-116">**Device configuration**</span></span>|
|[<span data-ttu-id="1ba69-117">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="1ba69-118">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="1ba69-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="1ba69-119">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="1ba69-120">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="1ba69-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="1ba69-121">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="1ba69-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="1ba69-122">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="1ba69-123">报告</span><span class="sxs-lookup"><span data-stu-id="1ba69-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="1ba69-124">注册放弃的元数据的详细信息报表</span><span class="sxs-lookup"><span data-stu-id="1ba69-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="1ba69-125">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="1ba69-126">报告</span><span class="sxs-lookup"><span data-stu-id="1ba69-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="1ba69-127">注册放弃摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="1ba69-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="1ba69-128">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="1ba69-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1ba69-129">Not yet documented</span></span>|
|[<span data-ttu-id="1ba69-130">managedDeviceEnrollmentFailureTrends 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="1ba69-131">注册失败趋势报告的元数据</span><span class="sxs-lookup"><span data-stu-id="1ba69-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="1ba69-132">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="1ba69-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="1ba69-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1ba69-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1ba69-134">属性</span><span class="sxs-lookup"><span data-stu-id="1ba69-134">Properties</span></span>
|<span data-ttu-id="1ba69-135">属性</span><span class="sxs-lookup"><span data-stu-id="1ba69-135">Property</span></span>|<span data-ttu-id="1ba69-136">类型</span><span class="sxs-lookup"><span data-stu-id="1ba69-136">Type</span></span>|<span data-ttu-id="1ba69-137">说明</span><span class="sxs-lookup"><span data-stu-id="1ba69-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ba69-138">id</span><span class="sxs-lookup"><span data-stu-id="1ba69-138">id</span></span>|<span data-ttu-id="1ba69-139">String</span><span class="sxs-lookup"><span data-stu-id="1ba69-139">String</span></span>|<span data-ttu-id="1ba69-140">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1ba69-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ba69-141">关系</span><span class="sxs-lookup"><span data-stu-id="1ba69-141">Relationships</span></span>
<span data-ttu-id="1ba69-142">无</span><span class="sxs-lookup"><span data-stu-id="1ba69-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ba69-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ba69-143">JSON Representation</span></span>
<span data-ttu-id="1ba69-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ba69-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



