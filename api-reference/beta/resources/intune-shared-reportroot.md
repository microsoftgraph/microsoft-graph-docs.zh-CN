---
title: reportRoot 资源类型
description: 表示设备实例或故障排除报告的资源，具体取决于上下文。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 739cdc4bd9b10f9d472cebd77c88ae796593a1f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523574"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="f3a7d-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3a7d-103">reportRoot resource type</span></span>

<span data-ttu-id="f3a7d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f3a7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3a7d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a7d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a7d-107">表示设备实例或故障排除报告的资源，具体取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="f3a7d-108">方法</span><span class="sxs-lookup"><span data-stu-id="f3a7d-108">Methods</span></span>
|<span data-ttu-id="f3a7d-109">方法</span><span class="sxs-lookup"><span data-stu-id="f3a7d-109">Method</span></span>|<span data-ttu-id="f3a7d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f3a7d-110">Return Type</span></span>|<span data-ttu-id="f3a7d-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3a7d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3a7d-112">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="f3a7d-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="f3a7d-113">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="f3a7d-114">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="f3a7d-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="f3a7d-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="f3a7d-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="f3a7d-116">**Device configuration**</span></span>|
|[<span data-ttu-id="f3a7d-117">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="f3a7d-118">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f3a7d-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="f3a7d-119">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="f3a7d-120">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f3a7d-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="f3a7d-121">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="f3a7d-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="f3a7d-122">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="f3a7d-123">报告</span><span class="sxs-lookup"><span data-stu-id="f3a7d-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f3a7d-124">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f3a7d-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="f3a7d-125">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="f3a7d-126">报告</span><span class="sxs-lookup"><span data-stu-id="f3a7d-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f3a7d-127">注册 abandonment 摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f3a7d-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="f3a7d-128">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="f3a7d-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3a7d-129">Not yet documented</span></span>|
|[<span data-ttu-id="f3a7d-130">managedDeviceEnrollmentFailureTrends 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="f3a7d-131">"注册失败趋势" 报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f3a7d-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="f3a7d-132">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="f3a7d-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="f3a7d-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3a7d-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f3a7d-134">属性</span><span class="sxs-lookup"><span data-stu-id="f3a7d-134">Properties</span></span>
|<span data-ttu-id="f3a7d-135">属性</span><span class="sxs-lookup"><span data-stu-id="f3a7d-135">Property</span></span>|<span data-ttu-id="f3a7d-136">类型</span><span class="sxs-lookup"><span data-stu-id="f3a7d-136">Type</span></span>|<span data-ttu-id="f3a7d-137">说明</span><span class="sxs-lookup"><span data-stu-id="f3a7d-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a7d-138">id</span><span class="sxs-lookup"><span data-stu-id="f3a7d-138">id</span></span>|<span data-ttu-id="f3a7d-139">String</span><span class="sxs-lookup"><span data-stu-id="f3a7d-139">String</span></span>|<span data-ttu-id="f3a7d-140">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3a7d-141">关系</span><span class="sxs-lookup"><span data-stu-id="f3a7d-141">Relationships</span></span>
<span data-ttu-id="f3a7d-142">无</span><span class="sxs-lookup"><span data-stu-id="f3a7d-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3a7d-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3a7d-143">JSON Representation</span></span>
<span data-ttu-id="f3a7d-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3a7d-144">Here is a JSON representation of the resource.</span></span>
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



