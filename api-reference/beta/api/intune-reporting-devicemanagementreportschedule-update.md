---
title: 更新 deviceManagementReportSchedule
description: 更新 deviceManagementReportSchedule 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 292094610627ee65d0a7f675aaae2eb578625dab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459075"
---
# <a name="update-devicemanagementreportschedule"></a><span data-ttu-id="4c8dc-103">更新 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="4c8dc-103">Update deviceManagementReportSchedule</span></span>

<span data-ttu-id="4c8dc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4c8dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c8dc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c8dc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c8dc-107">更新[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-107">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c8dc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c8dc-108">Prerequisites</span></span>
<span data-ttu-id="4c8dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c8dc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c8dc-111">Permission type</span></span>|<span data-ttu-id="4c8dc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c8dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c8dc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c8dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c8dc-114">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="4c8dc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4c8dc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c8dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c8dc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-116">Not supported.</span></span>|
|<span data-ttu-id="4c8dc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c8dc-117">Application</span></span>|<span data-ttu-id="4c8dc-118">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="4c8dc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c8dc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c8dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="request-headers"></a><span data-ttu-id="4c8dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c8dc-120">Request headers</span></span>
|<span data-ttu-id="4c8dc-121">标头</span><span class="sxs-lookup"><span data-stu-id="4c8dc-121">Header</span></span>|<span data-ttu-id="4c8dc-122">值</span><span class="sxs-lookup"><span data-stu-id="4c8dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c8dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c8dc-123">Authorization</span></span>|<span data-ttu-id="4c8dc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c8dc-125">接受</span><span class="sxs-lookup"><span data-stu-id="4c8dc-125">Accept</span></span>|<span data-ttu-id="4c8dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c8dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c8dc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c8dc-127">Request body</span></span>
<span data-ttu-id="4c8dc-128">在请求正文中，提供[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-128">In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

<span data-ttu-id="4c8dc-129">下表显示创建[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-129">The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>

|<span data-ttu-id="4c8dc-130">属性</span><span class="sxs-lookup"><span data-stu-id="4c8dc-130">Property</span></span>|<span data-ttu-id="4c8dc-131">类型</span><span class="sxs-lookup"><span data-stu-id="4c8dc-131">Type</span></span>|<span data-ttu-id="4c8dc-132">说明</span><span class="sxs-lookup"><span data-stu-id="4c8dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c8dc-133">id</span><span class="sxs-lookup"><span data-stu-id="4c8dc-133">id</span></span>|<span data-ttu-id="4c8dc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4c8dc-134">String</span></span>|<span data-ttu-id="4c8dc-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="4c8dc-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="4c8dc-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="4c8dc-136">reportScheduleName</span></span>|<span data-ttu-id="4c8dc-137">String</span><span class="sxs-lookup"><span data-stu-id="4c8dc-137">String</span></span>|<span data-ttu-id="4c8dc-138">计划的名称</span><span class="sxs-lookup"><span data-stu-id="4c8dc-138">Name of the schedule</span></span>|
|<span data-ttu-id="4c8dc-139">subject</span><span class="sxs-lookup"><span data-stu-id="4c8dc-139">subject</span></span>|<span data-ttu-id="4c8dc-140">String</span><span class="sxs-lookup"><span data-stu-id="4c8dc-140">String</span></span>|<span data-ttu-id="4c8dc-141">已传递的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="4c8dc-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="4c8dc-142">电子邮件</span><span class="sxs-lookup"><span data-stu-id="4c8dc-142">emails</span></span>|<span data-ttu-id="4c8dc-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="4c8dc-143">String collection</span></span>|<span data-ttu-id="4c8dc-144">计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="4c8dc-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="4c8dc-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="4c8dc-145">recurrence</span></span>|[<span data-ttu-id="4c8dc-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="4c8dc-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="4c8dc-147">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="4c8dc-148">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="4c8dc-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4c8dc-149">startDateTime</span></span>|<span data-ttu-id="4c8dc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c8dc-150">DateTimeOffset</span></span>|<span data-ttu-id="4c8dc-151">计划报告的开始交付时间</span><span class="sxs-lookup"><span data-stu-id="4c8dc-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="4c8dc-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4c8dc-152">endDateTime</span></span>|<span data-ttu-id="4c8dc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c8dc-153">DateTimeOffset</span></span>|<span data-ttu-id="4c8dc-154">计划报告的结束传递时间</span><span class="sxs-lookup"><span data-stu-id="4c8dc-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="4c8dc-155">userId</span><span class="sxs-lookup"><span data-stu-id="4c8dc-155">userId</span></span>|<span data-ttu-id="4c8dc-156">String</span><span class="sxs-lookup"><span data-stu-id="4c8dc-156">String</span></span>|<span data-ttu-id="4c8dc-157">创建报表的用户的 Id</span><span class="sxs-lookup"><span data-stu-id="4c8dc-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="4c8dc-158">reportName</span><span class="sxs-lookup"><span data-stu-id="4c8dc-158">reportName</span></span>|<span data-ttu-id="4c8dc-159">String</span><span class="sxs-lookup"><span data-stu-id="4c8dc-159">String</span></span>|<span data-ttu-id="4c8dc-160">报告的名称</span><span class="sxs-lookup"><span data-stu-id="4c8dc-160">Name of the report</span></span>|
|<span data-ttu-id="4c8dc-161">filter</span><span class="sxs-lookup"><span data-stu-id="4c8dc-161">filter</span></span>|<span data-ttu-id="4c8dc-162">String</span><span class="sxs-lookup"><span data-stu-id="4c8dc-162">String</span></span>|<span data-ttu-id="4c8dc-163">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="4c8dc-163">Filters applied on the report</span></span>|
|<span data-ttu-id="4c8dc-164">select</span><span class="sxs-lookup"><span data-stu-id="4c8dc-164">select</span></span>|<span data-ttu-id="4c8dc-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="4c8dc-165">String collection</span></span>|<span data-ttu-id="4c8dc-166">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="4c8dc-166">Columns selected from the report</span></span>|
|<span data-ttu-id="4c8dc-167">By</span><span class="sxs-lookup"><span data-stu-id="4c8dc-167">orderBy</span></span>|<span data-ttu-id="4c8dc-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="4c8dc-168">String collection</span></span>|<span data-ttu-id="4c8dc-169">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="4c8dc-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="4c8dc-170">format</span><span class="sxs-lookup"><span data-stu-id="4c8dc-170">format</span></span>|[<span data-ttu-id="4c8dc-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="4c8dc-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="4c8dc-172">计划报告的格式。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-172">Format of the scheduled report.</span></span> <span data-ttu-id="4c8dc-173">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="4c8dc-174">响应</span><span class="sxs-lookup"><span data-stu-id="4c8dc-174">Response</span></span>
<span data-ttu-id="4c8dc-175">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c8dc-176">示例</span><span class="sxs-lookup"><span data-stu-id="4c8dc-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c8dc-177">请求</span><span class="sxs-lookup"><span data-stu-id="4c8dc-177">Request</span></span>
<span data-ttu-id="4c8dc-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c8dc-179">响应</span><span class="sxs-lookup"><span data-stu-id="4c8dc-179">Response</span></span>
<span data-ttu-id="4c8dc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c8dc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





