---
title: deviceManagementReports 资源类型
description: 充当所有报表功能的容器的单一实例实体。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4f5712acc1dc4b50861a387d594cd2be55bc139
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772410"
---
# <a name="devicemanagementreports-resource-type"></a><span data-ttu-id="7f91c-103">deviceManagementReports 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f91c-103">deviceManagementReports resource type</span></span>

> <span data-ttu-id="7f91c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f91c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f91c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f91c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f91c-106">充当所有报表功能的容器的单一实例实体。</span><span class="sxs-lookup"><span data-stu-id="7f91c-106">Singleton entity that acts as a container for all reports functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="7f91c-107">方法</span><span class="sxs-lookup"><span data-stu-id="7f91c-107">Methods</span></span>
|<span data-ttu-id="7f91c-108">方法</span><span class="sxs-lookup"><span data-stu-id="7f91c-108">Method</span></span>|<span data-ttu-id="7f91c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7f91c-109">Return Type</span></span>|<span data-ttu-id="7f91c-110">说明</span><span class="sxs-lookup"><span data-stu-id="7f91c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f91c-111">获取 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="7f91c-111">Get deviceManagementReports</span></span>](../api/intune-reporting-devicemanagementreports-get.md)|[<span data-ttu-id="7f91c-112">deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="7f91c-112">deviceManagementReports</span></span>](../resources/intune-reporting-devicemanagementreports.md)|<span data-ttu-id="7f91c-113">读取[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f91c-113">Read properties and relationships of the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>|
|[<span data-ttu-id="7f91c-114">更新 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="7f91c-114">Update deviceManagementReports</span></span>](../api/intune-reporting-devicemanagementreports-update.md)|[<span data-ttu-id="7f91c-115">deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="7f91c-115">deviceManagementReports</span></span>](../resources/intune-reporting-devicemanagementreports.md)|<span data-ttu-id="7f91c-116">更新[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7f91c-116">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>|
|[<span data-ttu-id="7f91c-117">getDeviceNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="7f91c-117">getDeviceNonComplianceReport action</span></span>](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|<span data-ttu-id="7f91c-118">Stream</span><span class="sxs-lookup"><span data-stu-id="7f91c-118">Stream</span></span>|<span data-ttu-id="7f91c-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f91c-119">Not yet documented</span></span>|
|[<span data-ttu-id="7f91c-120">getPolicyNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="7f91c-120">getPolicyNonComplianceReport action</span></span>](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|<span data-ttu-id="7f91c-121">Stream</span><span class="sxs-lookup"><span data-stu-id="7f91c-121">Stream</span></span>|<span data-ttu-id="7f91c-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f91c-122">Not yet documented</span></span>|
|[<span data-ttu-id="7f91c-123">getPolicyNonComplianceMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="7f91c-123">getPolicyNonComplianceMetadata action</span></span>](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|<span data-ttu-id="7f91c-124">Stream</span><span class="sxs-lookup"><span data-stu-id="7f91c-124">Stream</span></span>|<span data-ttu-id="7f91c-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f91c-125">Not yet documented</span></span>|
|[<span data-ttu-id="7f91c-126">getSettingNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="7f91c-126">getSettingNonComplianceReport action</span></span>](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|<span data-ttu-id="7f91c-127">Stream</span><span class="sxs-lookup"><span data-stu-id="7f91c-127">Stream</span></span>|<span data-ttu-id="7f91c-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f91c-128">Not yet documented</span></span>|
|[<span data-ttu-id="7f91c-129">getHistoricalReport 操作</span><span class="sxs-lookup"><span data-stu-id="7f91c-129">getHistoricalReport action</span></span>](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|<span data-ttu-id="7f91c-130">Stream</span><span class="sxs-lookup"><span data-stu-id="7f91c-130">Stream</span></span>|<span data-ttu-id="7f91c-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f91c-131">Not yet documented</span></span>|
|[<span data-ttu-id="7f91c-132">getCachedReport 操作</span><span class="sxs-lookup"><span data-stu-id="7f91c-132">getCachedReport action</span></span>](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|<span data-ttu-id="7f91c-133">Stream</span><span class="sxs-lookup"><span data-stu-id="7f91c-133">Stream</span></span>|<span data-ttu-id="7f91c-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f91c-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7f91c-135">属性</span><span class="sxs-lookup"><span data-stu-id="7f91c-135">Properties</span></span>
|<span data-ttu-id="7f91c-136">属性</span><span class="sxs-lookup"><span data-stu-id="7f91c-136">Property</span></span>|<span data-ttu-id="7f91c-137">类型</span><span class="sxs-lookup"><span data-stu-id="7f91c-137">Type</span></span>|<span data-ttu-id="7f91c-138">说明</span><span class="sxs-lookup"><span data-stu-id="7f91c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f91c-139">id</span><span class="sxs-lookup"><span data-stu-id="7f91c-139">id</span></span>|<span data-ttu-id="7f91c-140">String</span><span class="sxs-lookup"><span data-stu-id="7f91c-140">String</span></span>|<span data-ttu-id="7f91c-141">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7f91c-141">Unique identifier for this entity</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f91c-142">关系</span><span class="sxs-lookup"><span data-stu-id="7f91c-142">Relationships</span></span>
|<span data-ttu-id="7f91c-143">关系</span><span class="sxs-lookup"><span data-stu-id="7f91c-143">Relationship</span></span>|<span data-ttu-id="7f91c-144">类型</span><span class="sxs-lookup"><span data-stu-id="7f91c-144">Type</span></span>|<span data-ttu-id="7f91c-145">说明</span><span class="sxs-lookup"><span data-stu-id="7f91c-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f91c-146">cachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="7f91c-146">cachedReportConfigurations</span></span>|<span data-ttu-id="7f91c-147">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f91c-147">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) collection</span></span>|<span data-ttu-id="7f91c-148">表示缓存报告配置的实体</span><span class="sxs-lookup"><span data-stu-id="7f91c-148">Entity representing the configuration of a cached report</span></span>|
|<span data-ttu-id="7f91c-149">exportJobs</span><span class="sxs-lookup"><span data-stu-id="7f91c-149">exportJobs</span></span>|<span data-ttu-id="7f91c-150">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f91c-150">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) collection</span></span>|<span data-ttu-id="7f91c-151">表示导出报告的作业的实体</span><span class="sxs-lookup"><span data-stu-id="7f91c-151">Entity representing a job to export a report</span></span>|
|<span data-ttu-id="7f91c-152">reportSchedules</span><span class="sxs-lookup"><span data-stu-id="7f91c-152">reportSchedules</span></span>|<span data-ttu-id="7f91c-153">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f91c-153">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) collection</span></span>|<span data-ttu-id="7f91c-154">表示为其传递报告的计划的实体</span><span class="sxs-lookup"><span data-stu-id="7f91c-154">Entity representing a schedule for which reports are delivered</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f91c-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f91c-155">JSON Representation</span></span>
<span data-ttu-id="7f91c-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f91c-156">Here is a JSON representation of the resource.</span></span>
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



