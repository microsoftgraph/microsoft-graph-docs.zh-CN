---
title: reportRoot 资源类型
description: 表示设备实例或故障排除报告的资源, 具体取决于上下文。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2e41d9b17ca7acafa98dad65db5d2ff5ce30925
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151294"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="2032c-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="2032c-103">reportRoot resource type</span></span>

> <span data-ttu-id="2032c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2032c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2032c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2032c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2032c-106">表示设备实例或故障排除报告的资源, 具体取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="2032c-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="2032c-107">方法</span><span class="sxs-lookup"><span data-stu-id="2032c-107">Methods</span></span>
|<span data-ttu-id="2032c-108">方法</span><span class="sxs-lookup"><span data-stu-id="2032c-108">Method</span></span>|<span data-ttu-id="2032c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2032c-109">Return Type</span></span>|<span data-ttu-id="2032c-110">说明</span><span class="sxs-lookup"><span data-stu-id="2032c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2032c-111">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="2032c-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="2032c-112">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2032c-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="2032c-113">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="2032c-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="2032c-114">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2032c-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="2032c-115">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="2032c-115">**Device configuration**</span></span>|
|[<span data-ttu-id="2032c-116">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="2032c-117">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="2032c-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="2032c-118">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="2032c-119">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="2032c-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="2032c-120">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="2032c-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="2032c-121">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="2032c-122">报告</span><span class="sxs-lookup"><span data-stu-id="2032c-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="2032c-123">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="2032c-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="2032c-124">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="2032c-125">报告</span><span class="sxs-lookup"><span data-stu-id="2032c-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="2032c-126">注册 abandonment 摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="2032c-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="2032c-127">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="2032c-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2032c-128">Not yet documented</span></span>|
|[<span data-ttu-id="2032c-129">managedDeviceEnrollmentFailureTrends 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="2032c-130">"注册失败趋势" 报告的元数据</span><span class="sxs-lookup"><span data-stu-id="2032c-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="2032c-131">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="2032c-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="2032c-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2032c-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2032c-133">属性</span><span class="sxs-lookup"><span data-stu-id="2032c-133">Properties</span></span>
|<span data-ttu-id="2032c-134">属性</span><span class="sxs-lookup"><span data-stu-id="2032c-134">Property</span></span>|<span data-ttu-id="2032c-135">类型</span><span class="sxs-lookup"><span data-stu-id="2032c-135">Type</span></span>|<span data-ttu-id="2032c-136">说明</span><span class="sxs-lookup"><span data-stu-id="2032c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2032c-137">id</span><span class="sxs-lookup"><span data-stu-id="2032c-137">id</span></span>|<span data-ttu-id="2032c-138">String</span><span class="sxs-lookup"><span data-stu-id="2032c-138">String</span></span>|<span data-ttu-id="2032c-139">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2032c-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2032c-140">关系</span><span class="sxs-lookup"><span data-stu-id="2032c-140">Relationships</span></span>
<span data-ttu-id="2032c-141">无</span><span class="sxs-lookup"><span data-stu-id="2032c-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2032c-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2032c-142">JSON Representation</span></span>
<span data-ttu-id="2032c-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2032c-143">Here is a JSON representation of the resource.</span></span>
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



