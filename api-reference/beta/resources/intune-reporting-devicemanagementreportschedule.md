---
title: deviceManagementReportSchedule 资源类型
description: 表示为其传递报告的计划的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 231f1f84acd294c340984c0c375bb87ceba94f95
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538845"
---
# <a name="devicemanagementreportschedule-resource-type"></a><span data-ttu-id="26270-103">deviceManagementReportSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="26270-103">deviceManagementReportSchedule resource type</span></span>

> <span data-ttu-id="26270-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26270-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26270-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26270-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26270-106">表示为其传递报告的计划的实体</span><span class="sxs-lookup"><span data-stu-id="26270-106">Entity representing a schedule for which reports are delivered</span></span>

## <a name="methods"></a><span data-ttu-id="26270-107">方法</span><span class="sxs-lookup"><span data-stu-id="26270-107">Methods</span></span>
|<span data-ttu-id="26270-108">方法</span><span class="sxs-lookup"><span data-stu-id="26270-108">Method</span></span>|<span data-ttu-id="26270-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26270-109">Return Type</span></span>|<span data-ttu-id="26270-110">说明</span><span class="sxs-lookup"><span data-stu-id="26270-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26270-111">列出 deviceManagementReportSchedules</span><span class="sxs-lookup"><span data-stu-id="26270-111">List deviceManagementReportSchedules</span></span>](../api/intune-reporting-devicemanagementreportschedule-list.md)|<span data-ttu-id="26270-112">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)集合</span><span class="sxs-lookup"><span data-stu-id="26270-112">[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) collection</span></span>|<span data-ttu-id="26270-113">列出[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26270-113">List properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects.</span></span>|
|[<span data-ttu-id="26270-114">获取 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-114">Get deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-get.md)|[<span data-ttu-id="26270-115">deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-115">deviceManagementReportSchedule</span></span>](../resources/intune-reporting-devicemanagementreportschedule.md)|<span data-ttu-id="26270-116">读取[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26270-116">Read properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>|
|[<span data-ttu-id="26270-117">创建 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-117">Create deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-create.md)|[<span data-ttu-id="26270-118">deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-118">deviceManagementReportSchedule</span></span>](../resources/intune-reporting-devicemanagementreportschedule.md)|<span data-ttu-id="26270-119">创建新的[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26270-119">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>|
|[<span data-ttu-id="26270-120">删除 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-120">Delete deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-delete.md)|<span data-ttu-id="26270-121">无</span><span class="sxs-lookup"><span data-stu-id="26270-121">None</span></span>|<span data-ttu-id="26270-122">删除[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)。</span><span class="sxs-lookup"><span data-stu-id="26270-122">Deletes a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>|
|[<span data-ttu-id="26270-123">更新 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-123">Update deviceManagementReportSchedule</span></span>](../api/intune-reporting-devicemanagementreportschedule-update.md)|[<span data-ttu-id="26270-124">deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="26270-124">deviceManagementReportSchedule</span></span>](../resources/intune-reporting-devicemanagementreportschedule.md)|<span data-ttu-id="26270-125">更新[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26270-125">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="26270-126">属性</span><span class="sxs-lookup"><span data-stu-id="26270-126">Properties</span></span>
|<span data-ttu-id="26270-127">属性</span><span class="sxs-lookup"><span data-stu-id="26270-127">Property</span></span>|<span data-ttu-id="26270-128">类型</span><span class="sxs-lookup"><span data-stu-id="26270-128">Type</span></span>|<span data-ttu-id="26270-129">说明</span><span class="sxs-lookup"><span data-stu-id="26270-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26270-130">id</span><span class="sxs-lookup"><span data-stu-id="26270-130">id</span></span>|<span data-ttu-id="26270-131">字符串</span><span class="sxs-lookup"><span data-stu-id="26270-131">String</span></span>|<span data-ttu-id="26270-132">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="26270-132">Unique identifier for this entity</span></span>|
|<span data-ttu-id="26270-133">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="26270-133">reportScheduleName</span></span>|<span data-ttu-id="26270-134">字符串</span><span class="sxs-lookup"><span data-stu-id="26270-134">String</span></span>|<span data-ttu-id="26270-135">计划的名称</span><span class="sxs-lookup"><span data-stu-id="26270-135">Name of the schedule</span></span>|
|<span data-ttu-id="26270-136">subject</span><span class="sxs-lookup"><span data-stu-id="26270-136">subject</span></span>|<span data-ttu-id="26270-137">String</span><span class="sxs-lookup"><span data-stu-id="26270-137">String</span></span>|<span data-ttu-id="26270-138">已传递的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="26270-138">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="26270-139">电子邮件</span><span class="sxs-lookup"><span data-stu-id="26270-139">emails</span></span>|<span data-ttu-id="26270-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="26270-140">String collection</span></span>|<span data-ttu-id="26270-141">计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="26270-141">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="26270-142">recurrence</span><span class="sxs-lookup"><span data-stu-id="26270-142">recurrence</span></span>|[<span data-ttu-id="26270-143">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="26270-143">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="26270-144">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="26270-144">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="26270-145">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="26270-145">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="26270-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="26270-146">startDateTime</span></span>|<span data-ttu-id="26270-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26270-147">DateTimeOffset</span></span>|<span data-ttu-id="26270-148">计划报告的开始交付时间</span><span class="sxs-lookup"><span data-stu-id="26270-148">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="26270-149">endDateTime</span><span class="sxs-lookup"><span data-stu-id="26270-149">endDateTime</span></span>|<span data-ttu-id="26270-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26270-150">DateTimeOffset</span></span>|<span data-ttu-id="26270-151">计划报告的结束传递时间</span><span class="sxs-lookup"><span data-stu-id="26270-151">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="26270-152">userId</span><span class="sxs-lookup"><span data-stu-id="26270-152">userId</span></span>|<span data-ttu-id="26270-153">String</span><span class="sxs-lookup"><span data-stu-id="26270-153">String</span></span>|<span data-ttu-id="26270-154">创建报表的用户的 Id</span><span class="sxs-lookup"><span data-stu-id="26270-154">The Id of the User who created the report</span></span>|
|<span data-ttu-id="26270-155">reportName</span><span class="sxs-lookup"><span data-stu-id="26270-155">reportName</span></span>|<span data-ttu-id="26270-156">字符串</span><span class="sxs-lookup"><span data-stu-id="26270-156">String</span></span>|<span data-ttu-id="26270-157">报告的名称</span><span class="sxs-lookup"><span data-stu-id="26270-157">Name of the report</span></span>|
|<span data-ttu-id="26270-158">filter</span><span class="sxs-lookup"><span data-stu-id="26270-158">filter</span></span>|<span data-ttu-id="26270-159">字符串</span><span class="sxs-lookup"><span data-stu-id="26270-159">String</span></span>|<span data-ttu-id="26270-160">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="26270-160">Filters applied on the report</span></span>|
|<span data-ttu-id="26270-161">select</span><span class="sxs-lookup"><span data-stu-id="26270-161">select</span></span>|<span data-ttu-id="26270-162">String 集合</span><span class="sxs-lookup"><span data-stu-id="26270-162">String collection</span></span>|<span data-ttu-id="26270-163">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="26270-163">Columns selected from the report</span></span>|
|<span data-ttu-id="26270-164">By</span><span class="sxs-lookup"><span data-stu-id="26270-164">orderBy</span></span>|<span data-ttu-id="26270-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="26270-165">String collection</span></span>|<span data-ttu-id="26270-166">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="26270-166">Ordering of columns in the report</span></span>|
|<span data-ttu-id="26270-167">format</span><span class="sxs-lookup"><span data-stu-id="26270-167">format</span></span>|[<span data-ttu-id="26270-168">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="26270-168">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="26270-169">计划报告的格式。</span><span class="sxs-lookup"><span data-stu-id="26270-169">Format of the scheduled report.</span></span> <span data-ttu-id="26270-170">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="26270-170">Possible values are: `csv`, `pdf`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26270-171">关系</span><span class="sxs-lookup"><span data-stu-id="26270-171">Relationships</span></span>
<span data-ttu-id="26270-172">无</span><span class="sxs-lookup"><span data-stu-id="26270-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26270-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26270-173">JSON Representation</span></span>
<span data-ttu-id="26270-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26270-174">Here is a JSON representation of the resource.</span></span>
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



