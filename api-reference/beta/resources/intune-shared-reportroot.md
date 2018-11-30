---
title: reportRoot 资源类型
description: 表示的设备或疑难解答的报告，具体取决于上下文实例的资源。
ms.openlocfilehash: 581f13bd7383be31ccdce7e536626eb6375ba777
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041789"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="0fb70-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fb70-103">reportRoot resource type</span></span>

> <span data-ttu-id="0fb70-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0fb70-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fb70-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0fb70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fb70-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0fb70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fb70-107">表示的设备或疑难解答的报告，具体取决于上下文实例的资源。</span><span class="sxs-lookup"><span data-stu-id="0fb70-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="0fb70-108">方法</span><span class="sxs-lookup"><span data-stu-id="0fb70-108">Methods</span></span>
|<span data-ttu-id="0fb70-109">方法</span><span class="sxs-lookup"><span data-stu-id="0fb70-109">Method</span></span>|<span data-ttu-id="0fb70-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fb70-110">Return Type</span></span>|<span data-ttu-id="0fb70-111">说明</span><span class="sxs-lookup"><span data-stu-id="0fb70-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fb70-112">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="0fb70-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="0fb70-113">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fb70-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="0fb70-114">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="0fb70-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="0fb70-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fb70-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="0fb70-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="0fb70-116">**Device configuration**</span></span>|
|[<span data-ttu-id="0fb70-117">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="0fb70-118">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="0fb70-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="0fb70-119">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="0fb70-120">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="0fb70-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="0fb70-121">**故障排除**</span><span class="sxs-lookup"><span data-stu-id="0fb70-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="0fb70-122">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="0fb70-123">报告</span><span class="sxs-lookup"><span data-stu-id="0fb70-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0fb70-124">注册放弃的元数据的详细信息报表</span><span class="sxs-lookup"><span data-stu-id="0fb70-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="0fb70-125">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="0fb70-126">报告</span><span class="sxs-lookup"><span data-stu-id="0fb70-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0fb70-127">注册放弃摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="0fb70-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="0fb70-128">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="0fb70-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fb70-129">Not yet documented</span></span>|
|[<span data-ttu-id="0fb70-130">managedDeviceEnrollmentFailureTrends 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="0fb70-131">注册失败趋势报告的元数据</span><span class="sxs-lookup"><span data-stu-id="0fb70-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="0fb70-132">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="0fb70-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="0fb70-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fb70-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0fb70-134">属性</span><span class="sxs-lookup"><span data-stu-id="0fb70-134">Properties</span></span>
|<span data-ttu-id="0fb70-135">属性</span><span class="sxs-lookup"><span data-stu-id="0fb70-135">Property</span></span>|<span data-ttu-id="0fb70-136">类型</span><span class="sxs-lookup"><span data-stu-id="0fb70-136">Type</span></span>|<span data-ttu-id="0fb70-137">说明</span><span class="sxs-lookup"><span data-stu-id="0fb70-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb70-138">id</span><span class="sxs-lookup"><span data-stu-id="0fb70-138">id</span></span>|<span data-ttu-id="0fb70-139">String</span><span class="sxs-lookup"><span data-stu-id="0fb70-139">String</span></span>|<span data-ttu-id="0fb70-140">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0fb70-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fb70-141">关系</span><span class="sxs-lookup"><span data-stu-id="0fb70-141">Relationships</span></span>
<span data-ttu-id="0fb70-142">无</span><span class="sxs-lookup"><span data-stu-id="0fb70-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fb70-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fb70-143">JSON Representation</span></span>
<span data-ttu-id="0fb70-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fb70-144">Here is a JSON representation of the resource.</span></span>
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



