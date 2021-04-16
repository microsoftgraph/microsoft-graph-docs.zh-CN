---
title: reportRoot 资源类型
description: 表示设备或疑难解答报告的实例的资源，具体取决于上下文。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30b84ec908eea116442284d6c20e2b56be68ea3c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863644"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="ab44f-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab44f-103">reportRoot resource type</span></span>

<span data-ttu-id="ab44f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab44f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab44f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab44f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab44f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab44f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab44f-107">表示设备或疑难解答报告的实例的资源，具体取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="ab44f-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="ab44f-108">方法</span><span class="sxs-lookup"><span data-stu-id="ab44f-108">Methods</span></span>
|<span data-ttu-id="ab44f-109">方法</span><span class="sxs-lookup"><span data-stu-id="ab44f-109">Method</span></span>|<span data-ttu-id="ab44f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab44f-110">Return Type</span></span>|<span data-ttu-id="ab44f-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab44f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab44f-112">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="ab44f-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="ab44f-113">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab44f-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="ab44f-114">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="ab44f-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="ab44f-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ab44f-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="ab44f-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="ab44f-116">**Device configuration**</span></span>|
|[<span data-ttu-id="ab44f-117">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="ab44f-118">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="ab44f-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="ab44f-119">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="ab44f-120">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="ab44f-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="ab44f-121">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="ab44f-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="ab44f-122">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="ab44f-123">报告</span><span class="sxs-lookup"><span data-stu-id="ab44f-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ab44f-124">注册的元数据详细信息报告</span><span class="sxs-lookup"><span data-stu-id="ab44f-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="ab44f-125">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="ab44f-126">报告</span><span class="sxs-lookup"><span data-stu-id="ab44f-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ab44f-127">注册元数据摘要报告</span><span class="sxs-lookup"><span data-stu-id="ab44f-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="ab44f-128">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="ab44f-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ab44f-129">Not yet documented</span></span>|
|[<span data-ttu-id="ab44f-130">managedDeviceEnrollmentFailureTrends 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="ab44f-131">注册失败趋势报告的元数据</span><span class="sxs-lookup"><span data-stu-id="ab44f-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="ab44f-132">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="ab44f-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="ab44f-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ab44f-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ab44f-134">属性</span><span class="sxs-lookup"><span data-stu-id="ab44f-134">Properties</span></span>
|<span data-ttu-id="ab44f-135">属性</span><span class="sxs-lookup"><span data-stu-id="ab44f-135">Property</span></span>|<span data-ttu-id="ab44f-136">类型</span><span class="sxs-lookup"><span data-stu-id="ab44f-136">Type</span></span>|<span data-ttu-id="ab44f-137">说明</span><span class="sxs-lookup"><span data-stu-id="ab44f-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab44f-138">id</span><span class="sxs-lookup"><span data-stu-id="ab44f-138">id</span></span>|<span data-ttu-id="ab44f-139">String</span><span class="sxs-lookup"><span data-stu-id="ab44f-139">String</span></span>|<span data-ttu-id="ab44f-140">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ab44f-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab44f-141">关系</span><span class="sxs-lookup"><span data-stu-id="ab44f-141">Relationships</span></span>
<span data-ttu-id="ab44f-142">无</span><span class="sxs-lookup"><span data-stu-id="ab44f-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab44f-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab44f-143">JSON Representation</span></span>
<span data-ttu-id="ab44f-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab44f-144">Here is a JSON representation of the resource.</span></span>
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




