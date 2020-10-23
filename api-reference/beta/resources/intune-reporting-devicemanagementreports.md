---
title: deviceManagementReports 资源类型
description: 充当所有报表功能的容器的单一实例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 988d7e11039ab3074cce46dccbd5a671a8dc0d7b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709808"
---
# <a name="devicemanagementreports-resource-type"></a><span data-ttu-id="e94b5-103">deviceManagementReports 资源类型</span><span class="sxs-lookup"><span data-stu-id="e94b5-103">deviceManagementReports resource type</span></span>

<span data-ttu-id="e94b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e94b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e94b5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e94b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e94b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e94b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e94b5-107">充当所有报表功能的容器的单一实例实体。</span><span class="sxs-lookup"><span data-stu-id="e94b5-107">Singleton entity that acts as a container for all reports functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="e94b5-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e94b5-108">Methods</span></span>
|<span data-ttu-id="e94b5-109">方法</span><span class="sxs-lookup"><span data-stu-id="e94b5-109">Method</span></span>|<span data-ttu-id="e94b5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e94b5-110">Return Type</span></span>|<span data-ttu-id="e94b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e94b5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e94b5-112">获取 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="e94b5-112">Get deviceManagementReports</span></span>](../api/intune-reporting-devicemanagementreports-get.md)|[<span data-ttu-id="e94b5-113">deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="e94b5-113">deviceManagementReports</span></span>](../resources/intune-reporting-devicemanagementreports.md)|<span data-ttu-id="e94b5-114">读取 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e94b5-114">Read properties and relationships of the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>|
|[<span data-ttu-id="e94b5-115">更新 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="e94b5-115">Update deviceManagementReports</span></span>](../api/intune-reporting-devicemanagementreports-update.md)|[<span data-ttu-id="e94b5-116">deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="e94b5-116">deviceManagementReports</span></span>](../resources/intune-reporting-devicemanagementreports.md)|<span data-ttu-id="e94b5-117">更新 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e94b5-117">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>|
|[<span data-ttu-id="e94b5-118">getDeviceNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-118">getDeviceNonComplianceReport action</span></span>](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|<span data-ttu-id="e94b5-119">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-119">Stream</span></span>|<span data-ttu-id="e94b5-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-120">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-121">getPolicyNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-121">getPolicyNonComplianceReport action</span></span>](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|<span data-ttu-id="e94b5-122">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-122">Stream</span></span>|<span data-ttu-id="e94b5-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-123">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-124">getPolicyNonComplianceMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-124">getPolicyNonComplianceMetadata action</span></span>](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|<span data-ttu-id="e94b5-125">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-125">Stream</span></span>|<span data-ttu-id="e94b5-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-126">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-127">getPolicyNonComplianceSummaryReport 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-127">getPolicyNonComplianceSummaryReport action</span></span>](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|<span data-ttu-id="e94b5-128">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-128">Stream</span></span>|<span data-ttu-id="e94b5-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-129">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-130">getSettingNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-130">getSettingNonComplianceReport action</span></span>](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|<span data-ttu-id="e94b5-131">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-131">Stream</span></span>|<span data-ttu-id="e94b5-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-132">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-133">getReportFilters 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-133">getReportFilters action</span></span>](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|<span data-ttu-id="e94b5-134">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-134">Stream</span></span>|<span data-ttu-id="e94b5-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-135">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-136">getHistoricalReport 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-136">getHistoricalReport action</span></span>](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|<span data-ttu-id="e94b5-137">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-137">Stream</span></span>|<span data-ttu-id="e94b5-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-138">Not yet documented</span></span>|
|[<span data-ttu-id="e94b5-139">getCachedReport 操作</span><span class="sxs-lookup"><span data-stu-id="e94b5-139">getCachedReport action</span></span>](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|<span data-ttu-id="e94b5-140">Stream</span><span class="sxs-lookup"><span data-stu-id="e94b5-140">Stream</span></span>|<span data-ttu-id="e94b5-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e94b5-141">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e94b5-142">属性</span><span class="sxs-lookup"><span data-stu-id="e94b5-142">Properties</span></span>
|<span data-ttu-id="e94b5-143">属性</span><span class="sxs-lookup"><span data-stu-id="e94b5-143">Property</span></span>|<span data-ttu-id="e94b5-144">类型</span><span class="sxs-lookup"><span data-stu-id="e94b5-144">Type</span></span>|<span data-ttu-id="e94b5-145">说明</span><span class="sxs-lookup"><span data-stu-id="e94b5-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e94b5-146">id</span><span class="sxs-lookup"><span data-stu-id="e94b5-146">id</span></span>|<span data-ttu-id="e94b5-147">String</span><span class="sxs-lookup"><span data-stu-id="e94b5-147">String</span></span>|<span data-ttu-id="e94b5-148">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e94b5-148">Unique identifier for this entity</span></span>|

## <a name="relationships"></a><span data-ttu-id="e94b5-149">关系</span><span class="sxs-lookup"><span data-stu-id="e94b5-149">Relationships</span></span>
|<span data-ttu-id="e94b5-150">关系</span><span class="sxs-lookup"><span data-stu-id="e94b5-150">Relationship</span></span>|<span data-ttu-id="e94b5-151">类型</span><span class="sxs-lookup"><span data-stu-id="e94b5-151">Type</span></span>|<span data-ttu-id="e94b5-152">说明</span><span class="sxs-lookup"><span data-stu-id="e94b5-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e94b5-153">cachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="e94b5-153">cachedReportConfigurations</span></span>|<span data-ttu-id="e94b5-154">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e94b5-154">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) collection</span></span>|<span data-ttu-id="e94b5-155">表示缓存报告配置的实体</span><span class="sxs-lookup"><span data-stu-id="e94b5-155">Entity representing the configuration of a cached report</span></span>|
|<span data-ttu-id="e94b5-156">exportJobs</span><span class="sxs-lookup"><span data-stu-id="e94b5-156">exportJobs</span></span>|<span data-ttu-id="e94b5-157">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e94b5-157">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) collection</span></span>|<span data-ttu-id="e94b5-158">表示导出报告的作业的实体</span><span class="sxs-lookup"><span data-stu-id="e94b5-158">Entity representing a job to export a report</span></span>|
|<span data-ttu-id="e94b5-159">reportSchedules</span><span class="sxs-lookup"><span data-stu-id="e94b5-159">reportSchedules</span></span>|<span data-ttu-id="e94b5-160">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e94b5-160">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) collection</span></span>|<span data-ttu-id="e94b5-161">表示为其传递报告的计划的实体</span><span class="sxs-lookup"><span data-stu-id="e94b5-161">Entity representing a schedule for which reports are delivered</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e94b5-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e94b5-162">JSON Representation</span></span>
<span data-ttu-id="e94b5-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e94b5-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```





