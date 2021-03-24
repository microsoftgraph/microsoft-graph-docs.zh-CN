---
title: 更新 deviceManagementReportSchedule
description: 更新 deviceManagementReportSchedule 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e1466e9a24ba3cd4021ed7d8aa59897af017354
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134373"
---
# <a name="update-devicemanagementreportschedule"></a><span data-ttu-id="a1380-103">更新 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="a1380-103">Update deviceManagementReportSchedule</span></span>

<span data-ttu-id="a1380-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1380-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1380-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1380-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1380-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1380-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1380-107">更新 [deviceManagementReportSchedule 对象](../resources/intune-reporting-devicemanagementreportschedule.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a1380-107">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1380-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1380-108">Prerequisites</span></span>
<span data-ttu-id="a1380-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1380-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1380-111">Permission type</span></span>|<span data-ttu-id="a1380-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1380-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1380-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1380-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1380-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1380-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1380-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1380-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1380-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1380-116">Not supported.</span></span>|
|<span data-ttu-id="a1380-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1380-117">Application</span></span>|<span data-ttu-id="a1380-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1380-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1380-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1380-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="request-headers"></a><span data-ttu-id="a1380-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1380-120">Request headers</span></span>
|<span data-ttu-id="a1380-121">标头</span><span class="sxs-lookup"><span data-stu-id="a1380-121">Header</span></span>|<span data-ttu-id="a1380-122">值</span><span class="sxs-lookup"><span data-stu-id="a1380-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1380-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1380-123">Authorization</span></span>|<span data-ttu-id="a1380-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1380-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1380-125">接受</span><span class="sxs-lookup"><span data-stu-id="a1380-125">Accept</span></span>|<span data-ttu-id="a1380-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1380-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1380-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1380-127">Request body</span></span>
<span data-ttu-id="a1380-128">在请求正文中，提供 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1380-128">In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

<span data-ttu-id="a1380-129">下表显示创建 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1380-129">The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>

|<span data-ttu-id="a1380-130">属性</span><span class="sxs-lookup"><span data-stu-id="a1380-130">Property</span></span>|<span data-ttu-id="a1380-131">类型</span><span class="sxs-lookup"><span data-stu-id="a1380-131">Type</span></span>|<span data-ttu-id="a1380-132">说明</span><span class="sxs-lookup"><span data-stu-id="a1380-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1380-133">id</span><span class="sxs-lookup"><span data-stu-id="a1380-133">id</span></span>|<span data-ttu-id="a1380-134">String</span><span class="sxs-lookup"><span data-stu-id="a1380-134">String</span></span>|<span data-ttu-id="a1380-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="a1380-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="a1380-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="a1380-136">reportScheduleName</span></span>|<span data-ttu-id="a1380-137">String</span><span class="sxs-lookup"><span data-stu-id="a1380-137">String</span></span>|<span data-ttu-id="a1380-138">计划的名称</span><span class="sxs-lookup"><span data-stu-id="a1380-138">Name of the schedule</span></span>|
|<span data-ttu-id="a1380-139">subject</span><span class="sxs-lookup"><span data-stu-id="a1380-139">subject</span></span>|<span data-ttu-id="a1380-140">String</span><span class="sxs-lookup"><span data-stu-id="a1380-140">String</span></span>|<span data-ttu-id="a1380-141">已送达的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="a1380-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="a1380-142">电子邮件</span><span class="sxs-lookup"><span data-stu-id="a1380-142">emails</span></span>|<span data-ttu-id="a1380-143">String collection</span><span class="sxs-lookup"><span data-stu-id="a1380-143">String collection</span></span>|<span data-ttu-id="a1380-144">将计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="a1380-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="a1380-145">定期</span><span class="sxs-lookup"><span data-stu-id="a1380-145">recurrence</span></span>|[<span data-ttu-id="a1380-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="a1380-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="a1380-147">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="a1380-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="a1380-148">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="a1380-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="a1380-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a1380-149">startDateTime</span></span>|<span data-ttu-id="a1380-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1380-150">DateTimeOffset</span></span>|<span data-ttu-id="a1380-151">计划报告交付开始的时间</span><span class="sxs-lookup"><span data-stu-id="a1380-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="a1380-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a1380-152">endDateTime</span></span>|<span data-ttu-id="a1380-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1380-153">DateTimeOffset</span></span>|<span data-ttu-id="a1380-154">计划报告传递结束的时间</span><span class="sxs-lookup"><span data-stu-id="a1380-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="a1380-155">userId</span><span class="sxs-lookup"><span data-stu-id="a1380-155">userId</span></span>|<span data-ttu-id="a1380-156">String</span><span class="sxs-lookup"><span data-stu-id="a1380-156">String</span></span>|<span data-ttu-id="a1380-157">创建报告的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="a1380-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="a1380-158">reportName</span><span class="sxs-lookup"><span data-stu-id="a1380-158">reportName</span></span>|<span data-ttu-id="a1380-159">String</span><span class="sxs-lookup"><span data-stu-id="a1380-159">String</span></span>|<span data-ttu-id="a1380-160">报告的名称</span><span class="sxs-lookup"><span data-stu-id="a1380-160">Name of the report</span></span>|
|<span data-ttu-id="a1380-161">filter</span><span class="sxs-lookup"><span data-stu-id="a1380-161">filter</span></span>|<span data-ttu-id="a1380-162">String</span><span class="sxs-lookup"><span data-stu-id="a1380-162">String</span></span>|<span data-ttu-id="a1380-163">应用于报表的筛选器</span><span class="sxs-lookup"><span data-stu-id="a1380-163">Filters applied on the report</span></span>|
|<span data-ttu-id="a1380-164">select</span><span class="sxs-lookup"><span data-stu-id="a1380-164">select</span></span>|<span data-ttu-id="a1380-165">String collection</span><span class="sxs-lookup"><span data-stu-id="a1380-165">String collection</span></span>|<span data-ttu-id="a1380-166">从报表选择的列</span><span class="sxs-lookup"><span data-stu-id="a1380-166">Columns selected from the report</span></span>|
|<span data-ttu-id="a1380-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="a1380-167">orderBy</span></span>|<span data-ttu-id="a1380-168">String collection</span><span class="sxs-lookup"><span data-stu-id="a1380-168">String collection</span></span>|<span data-ttu-id="a1380-169">报告中列的排序</span><span class="sxs-lookup"><span data-stu-id="a1380-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="a1380-170">format</span><span class="sxs-lookup"><span data-stu-id="a1380-170">format</span></span>|[<span data-ttu-id="a1380-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="a1380-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="a1380-172">计划报表的格式。</span><span class="sxs-lookup"><span data-stu-id="a1380-172">Format of the scheduled report.</span></span> <span data-ttu-id="a1380-173">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="a1380-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1380-174">响应</span><span class="sxs-lookup"><span data-stu-id="a1380-174">Response</span></span>
<span data-ttu-id="a1380-175">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1380-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1380-176">示例</span><span class="sxs-lookup"><span data-stu-id="a1380-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1380-177">请求</span><span class="sxs-lookup"><span data-stu-id="a1380-177">Request</span></span>
<span data-ttu-id="a1380-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1380-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
Content-type: application/json
Content-length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```

### <a name="response"></a><span data-ttu-id="a1380-179">响应</span><span class="sxs-lookup"><span data-stu-id="a1380-179">Response</span></span>
<span data-ttu-id="a1380-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1380-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "00bb9785-9785-00bb-8597-bb008597bb00",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```




