---
title: reportRoot 资源类型
description: 表示设备实例或故障排除报告的资源, 具体取决于上下文。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c975abfa3cb580d107967c7adaf66627bad2ad2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938728"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="6ac11-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ac11-103">reportRoot resource type</span></span>

> <span data-ttu-id="6ac11-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ac11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ac11-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ac11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ac11-106">表示设备实例或故障排除报告的资源, 具体取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="6ac11-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="6ac11-107">方法</span><span class="sxs-lookup"><span data-stu-id="6ac11-107">Methods</span></span>
|<span data-ttu-id="6ac11-108">方法</span><span class="sxs-lookup"><span data-stu-id="6ac11-108">Method</span></span>|<span data-ttu-id="6ac11-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6ac11-109">Return Type</span></span>|<span data-ttu-id="6ac11-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ac11-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ac11-111">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="6ac11-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="6ac11-112">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ac11-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="6ac11-113">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="6ac11-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="6ac11-114">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6ac11-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="6ac11-115">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="6ac11-115">**Device configuration**</span></span>|
|[<span data-ttu-id="6ac11-116">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="6ac11-117">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6ac11-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="6ac11-118">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="6ac11-119">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6ac11-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="6ac11-120">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="6ac11-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="6ac11-121">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="6ac11-122">报告</span><span class="sxs-lookup"><span data-stu-id="6ac11-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6ac11-123">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6ac11-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="6ac11-124">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="6ac11-125">报告</span><span class="sxs-lookup"><span data-stu-id="6ac11-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6ac11-126">注册 abandonment 摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6ac11-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="6ac11-127">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="6ac11-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6ac11-128">Not yet documented</span></span>|
|[<span data-ttu-id="6ac11-129">managedDeviceEnrollmentFailureTrends 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="6ac11-130">"注册失败趋势" 报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6ac11-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="6ac11-131">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="6ac11-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="6ac11-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6ac11-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6ac11-133">属性</span><span class="sxs-lookup"><span data-stu-id="6ac11-133">Properties</span></span>
|<span data-ttu-id="6ac11-134">属性</span><span class="sxs-lookup"><span data-stu-id="6ac11-134">Property</span></span>|<span data-ttu-id="6ac11-135">类型</span><span class="sxs-lookup"><span data-stu-id="6ac11-135">Type</span></span>|<span data-ttu-id="6ac11-136">说明</span><span class="sxs-lookup"><span data-stu-id="6ac11-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ac11-137">id</span><span class="sxs-lookup"><span data-stu-id="6ac11-137">id</span></span>|<span data-ttu-id="6ac11-138">String</span><span class="sxs-lookup"><span data-stu-id="6ac11-138">String</span></span>|<span data-ttu-id="6ac11-139">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6ac11-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ac11-140">关系</span><span class="sxs-lookup"><span data-stu-id="6ac11-140">Relationships</span></span>
<span data-ttu-id="6ac11-141">无</span><span class="sxs-lookup"><span data-stu-id="6ac11-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ac11-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ac11-142">JSON Representation</span></span>
<span data-ttu-id="6ac11-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ac11-143">Here is a JSON representation of the resource.</span></span>
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



