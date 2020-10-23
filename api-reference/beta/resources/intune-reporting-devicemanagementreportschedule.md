---
title: deviceManagementReportSchedule 资源类型
description: 表示为其传递报告的计划的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5f55b056f3c20d164446c27d7c1a6d549d99ecf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735146"
---
# <a name="devicemanagementreportschedule-resource-type"></a><span data-ttu-id="3c49d-103">deviceManagementReportSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c49d-103">deviceManagementReportSchedule resource type</span></span>

<span data-ttu-id="3c49d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c49d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c49d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c49d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c49d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c49d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c49d-107">表示为其传递报告的计划的实体</span><span class="sxs-lookup"><span data-stu-id="3c49d-107">Entity representing a schedule for which reports are delivered</span></span>

## <a name="methods"></a><span data-ttu-id="3c49d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="3c49d-108">Methods</span></span>
|<span data-ttu-id="3c49d-109">方法</span><span class="sxs-lookup"><span data-stu-id="3c49d-109">Method</span></span>|<span data-ttu-id="3c49d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c49d-110">Return Type</span></span>|<span data-ttu-id="3c49d-111">说明</span><span class="sxs-lookup"><span data-stu-id="3c49d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c49d-112">列出 deviceManagementReportSchedules</span><span class="sxs-lookup"><span data-stu-id="3c49d-112">List deviceManagementReportSchedules</span></span>](../api/intune-reporting-devicemanagementreportschedule-list.md)|<span data-ttu-id="3c49d-113">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c49d-113">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) collection</span></span>|<span data-ttu-id="3c49d-114">列出 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c49d-114">List properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects.</span></span>|
|[<span data-ttu-id="3c49d-115">获取 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-115">Get deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-get.md)|[<span data-ttu-id="3c49d-116">deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-116">deviceManagementReportSchedule</span></span>](../resources/intune-reporting-devicemanagementreportschedule.md)|<span data-ttu-id="3c49d-117">读取 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c49d-117">Read properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>|
|[<span data-ttu-id="3c49d-118">创建 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-118">Create deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-create.md)|[<span data-ttu-id="3c49d-119">deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-119">deviceManagementReportSchedule</span></span>](../resources/intune-reporting-devicemanagementreportschedule.md)|<span data-ttu-id="3c49d-120">创建新的 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c49d-120">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>|
|[<span data-ttu-id="3c49d-121">删除 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-121">Delete deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-delete.md)|<span data-ttu-id="3c49d-122">无</span><span class="sxs-lookup"><span data-stu-id="3c49d-122">None</span></span>|<span data-ttu-id="3c49d-123">删除 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)。</span><span class="sxs-lookup"><span data-stu-id="3c49d-123">Deletes a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>|
|[<span data-ttu-id="3c49d-124">更新 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-124">Update deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-update.md)|[<span data-ttu-id="3c49d-125">deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="3c49d-125">deviceManagementReportSchedule</span></span>](../resources/intune-reporting-devicemanagementreportschedule.md)|<span data-ttu-id="3c49d-126">更新 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c49d-126">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c49d-127">属性</span><span class="sxs-lookup"><span data-stu-id="3c49d-127">Properties</span></span>
|<span data-ttu-id="3c49d-128">属性</span><span class="sxs-lookup"><span data-stu-id="3c49d-128">Property</span></span>|<span data-ttu-id="3c49d-129">类型</span><span class="sxs-lookup"><span data-stu-id="3c49d-129">Type</span></span>|<span data-ttu-id="3c49d-130">说明</span><span class="sxs-lookup"><span data-stu-id="3c49d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c49d-131">id</span><span class="sxs-lookup"><span data-stu-id="3c49d-131">id</span></span>|<span data-ttu-id="3c49d-132">String</span><span class="sxs-lookup"><span data-stu-id="3c49d-132">String</span></span>|<span data-ttu-id="3c49d-133">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3c49d-133">Unique identifier for this entity</span></span>|
|<span data-ttu-id="3c49d-134">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="3c49d-134">reportScheduleName</span></span>|<span data-ttu-id="3c49d-135">String</span><span class="sxs-lookup"><span data-stu-id="3c49d-135">String</span></span>|<span data-ttu-id="3c49d-136">计划的名称</span><span class="sxs-lookup"><span data-stu-id="3c49d-136">Name of the schedule</span></span>|
|<span data-ttu-id="3c49d-137">subject</span><span class="sxs-lookup"><span data-stu-id="3c49d-137">subject</span></span>|<span data-ttu-id="3c49d-138">String</span><span class="sxs-lookup"><span data-stu-id="3c49d-138">String</span></span>|<span data-ttu-id="3c49d-139">已传递的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="3c49d-139">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="3c49d-140">电子邮件</span><span class="sxs-lookup"><span data-stu-id="3c49d-140">emails</span></span>|<span data-ttu-id="3c49d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3c49d-141">String collection</span></span>|<span data-ttu-id="3c49d-142">计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="3c49d-142">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="3c49d-143">recurrence</span><span class="sxs-lookup"><span data-stu-id="3c49d-143">recurrence</span></span>|[<span data-ttu-id="3c49d-144">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="3c49d-144">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="3c49d-145">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="3c49d-145">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="3c49d-146">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="3c49d-146">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="3c49d-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3c49d-147">startDateTime</span></span>|<span data-ttu-id="3c49d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c49d-148">DateTimeOffset</span></span>|<span data-ttu-id="3c49d-149">计划报告的开始交付时间</span><span class="sxs-lookup"><span data-stu-id="3c49d-149">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="3c49d-150">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3c49d-150">endDateTime</span></span>|<span data-ttu-id="3c49d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c49d-151">DateTimeOffset</span></span>|<span data-ttu-id="3c49d-152">计划报告的结束传递时间</span><span class="sxs-lookup"><span data-stu-id="3c49d-152">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="3c49d-153">userId</span><span class="sxs-lookup"><span data-stu-id="3c49d-153">userId</span></span>|<span data-ttu-id="3c49d-154">String</span><span class="sxs-lookup"><span data-stu-id="3c49d-154">String</span></span>|<span data-ttu-id="3c49d-155">创建报表的用户的 Id</span><span class="sxs-lookup"><span data-stu-id="3c49d-155">The Id of the User who created the report</span></span>|
|<span data-ttu-id="3c49d-156">reportName</span><span class="sxs-lookup"><span data-stu-id="3c49d-156">reportName</span></span>|<span data-ttu-id="3c49d-157">String</span><span class="sxs-lookup"><span data-stu-id="3c49d-157">String</span></span>|<span data-ttu-id="3c49d-158">报告的名称</span><span class="sxs-lookup"><span data-stu-id="3c49d-158">Name of the report</span></span>|
|<span data-ttu-id="3c49d-159">filter</span><span class="sxs-lookup"><span data-stu-id="3c49d-159">filter</span></span>|<span data-ttu-id="3c49d-160">String</span><span class="sxs-lookup"><span data-stu-id="3c49d-160">String</span></span>|<span data-ttu-id="3c49d-161">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="3c49d-161">Filters applied on the report</span></span>|
|<span data-ttu-id="3c49d-162">select</span><span class="sxs-lookup"><span data-stu-id="3c49d-162">select</span></span>|<span data-ttu-id="3c49d-163">String collection</span><span class="sxs-lookup"><span data-stu-id="3c49d-163">String collection</span></span>|<span data-ttu-id="3c49d-164">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="3c49d-164">Columns selected from the report</span></span>|
|<span data-ttu-id="3c49d-165">By</span><span class="sxs-lookup"><span data-stu-id="3c49d-165">orderBy</span></span>|<span data-ttu-id="3c49d-166">String collection</span><span class="sxs-lookup"><span data-stu-id="3c49d-166">String collection</span></span>|<span data-ttu-id="3c49d-167">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="3c49d-167">Ordering of columns in the report</span></span>|
|<span data-ttu-id="3c49d-168">format</span><span class="sxs-lookup"><span data-stu-id="3c49d-168">format</span></span>|[<span data-ttu-id="3c49d-169">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="3c49d-169">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="3c49d-170">计划报告的格式。</span><span class="sxs-lookup"><span data-stu-id="3c49d-170">Format of the scheduled report.</span></span> <span data-ttu-id="3c49d-171">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="3c49d-171">Possible values are: `csv`, `pdf`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c49d-172">关系</span><span class="sxs-lookup"><span data-stu-id="3c49d-172">Relationships</span></span>
<span data-ttu-id="3c49d-173">无</span><span class="sxs-lookup"><span data-stu-id="3c49d-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c49d-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c49d-174">JSON Representation</span></span>
<span data-ttu-id="3c49d-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c49d-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "String (identifier)",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```





