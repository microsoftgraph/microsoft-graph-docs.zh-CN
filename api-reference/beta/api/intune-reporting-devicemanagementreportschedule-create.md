---
title: 创建 deviceManagementReportSchedule
description: 创建新的 deviceManagementReportSchedule 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39efbd22ab87b44e3a460775e1c69aba8cac5edf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698111"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="f661c-103">创建 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="f661c-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="f661c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f661c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f661c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f661c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f661c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f661c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f661c-107">创建新的 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f661c-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f661c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f661c-108">Prerequisites</span></span>
<span data-ttu-id="f661c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f661c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f661c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f661c-111">Permission type</span></span>|<span data-ttu-id="f661c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f661c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f661c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f661c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f661c-114">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="f661c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f661c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f661c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f661c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f661c-116">Not supported.</span></span>|
|<span data-ttu-id="f661c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f661c-117">Application</span></span>|<span data-ttu-id="f661c-118">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="f661c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f661c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f661c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="f661c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f661c-120">Request headers</span></span>
|<span data-ttu-id="f661c-121">标头</span><span class="sxs-lookup"><span data-stu-id="f661c-121">Header</span></span>|<span data-ttu-id="f661c-122">值</span><span class="sxs-lookup"><span data-stu-id="f661c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f661c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f661c-123">Authorization</span></span>|<span data-ttu-id="f661c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f661c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f661c-125">接受</span><span class="sxs-lookup"><span data-stu-id="f661c-125">Accept</span></span>|<span data-ttu-id="f661c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f661c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f661c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f661c-127">Request body</span></span>
<span data-ttu-id="f661c-128">在请求正文中，提供 deviceManagementReportSchedule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f661c-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="f661c-129">下表显示创建 deviceManagementReportSchedule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f661c-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="f661c-130">属性</span><span class="sxs-lookup"><span data-stu-id="f661c-130">Property</span></span>|<span data-ttu-id="f661c-131">类型</span><span class="sxs-lookup"><span data-stu-id="f661c-131">Type</span></span>|<span data-ttu-id="f661c-132">说明</span><span class="sxs-lookup"><span data-stu-id="f661c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f661c-133">id</span><span class="sxs-lookup"><span data-stu-id="f661c-133">id</span></span>|<span data-ttu-id="f661c-134">String</span><span class="sxs-lookup"><span data-stu-id="f661c-134">String</span></span>|<span data-ttu-id="f661c-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f661c-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="f661c-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="f661c-136">reportScheduleName</span></span>|<span data-ttu-id="f661c-137">String</span><span class="sxs-lookup"><span data-stu-id="f661c-137">String</span></span>|<span data-ttu-id="f661c-138">计划的名称</span><span class="sxs-lookup"><span data-stu-id="f661c-138">Name of the schedule</span></span>|
|<span data-ttu-id="f661c-139">subject</span><span class="sxs-lookup"><span data-stu-id="f661c-139">subject</span></span>|<span data-ttu-id="f661c-140">String</span><span class="sxs-lookup"><span data-stu-id="f661c-140">String</span></span>|<span data-ttu-id="f661c-141">已传递的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="f661c-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="f661c-142">电子邮件</span><span class="sxs-lookup"><span data-stu-id="f661c-142">emails</span></span>|<span data-ttu-id="f661c-143">String collection</span><span class="sxs-lookup"><span data-stu-id="f661c-143">String collection</span></span>|<span data-ttu-id="f661c-144">计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="f661c-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="f661c-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="f661c-145">recurrence</span></span>|[<span data-ttu-id="f661c-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="f661c-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="f661c-147">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="f661c-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="f661c-148">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="f661c-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="f661c-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f661c-149">startDateTime</span></span>|<span data-ttu-id="f661c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f661c-150">DateTimeOffset</span></span>|<span data-ttu-id="f661c-151">计划报告的开始交付时间</span><span class="sxs-lookup"><span data-stu-id="f661c-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="f661c-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f661c-152">endDateTime</span></span>|<span data-ttu-id="f661c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f661c-153">DateTimeOffset</span></span>|<span data-ttu-id="f661c-154">计划报告的结束传递时间</span><span class="sxs-lookup"><span data-stu-id="f661c-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="f661c-155">userId</span><span class="sxs-lookup"><span data-stu-id="f661c-155">userId</span></span>|<span data-ttu-id="f661c-156">String</span><span class="sxs-lookup"><span data-stu-id="f661c-156">String</span></span>|<span data-ttu-id="f661c-157">创建报表的用户的 Id</span><span class="sxs-lookup"><span data-stu-id="f661c-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="f661c-158">reportName</span><span class="sxs-lookup"><span data-stu-id="f661c-158">reportName</span></span>|<span data-ttu-id="f661c-159">String</span><span class="sxs-lookup"><span data-stu-id="f661c-159">String</span></span>|<span data-ttu-id="f661c-160">报告的名称</span><span class="sxs-lookup"><span data-stu-id="f661c-160">Name of the report</span></span>|
|<span data-ttu-id="f661c-161">filter</span><span class="sxs-lookup"><span data-stu-id="f661c-161">filter</span></span>|<span data-ttu-id="f661c-162">String</span><span class="sxs-lookup"><span data-stu-id="f661c-162">String</span></span>|<span data-ttu-id="f661c-163">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="f661c-163">Filters applied on the report</span></span>|
|<span data-ttu-id="f661c-164">select</span><span class="sxs-lookup"><span data-stu-id="f661c-164">select</span></span>|<span data-ttu-id="f661c-165">String collection</span><span class="sxs-lookup"><span data-stu-id="f661c-165">String collection</span></span>|<span data-ttu-id="f661c-166">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="f661c-166">Columns selected from the report</span></span>|
|<span data-ttu-id="f661c-167">By</span><span class="sxs-lookup"><span data-stu-id="f661c-167">orderBy</span></span>|<span data-ttu-id="f661c-168">String collection</span><span class="sxs-lookup"><span data-stu-id="f661c-168">String collection</span></span>|<span data-ttu-id="f661c-169">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="f661c-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="f661c-170">format</span><span class="sxs-lookup"><span data-stu-id="f661c-170">format</span></span>|[<span data-ttu-id="f661c-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="f661c-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="f661c-172">计划报告的格式。</span><span class="sxs-lookup"><span data-stu-id="f661c-172">Format of the scheduled report.</span></span> <span data-ttu-id="f661c-173">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="f661c-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="f661c-174">响应</span><span class="sxs-lookup"><span data-stu-id="f661c-174">Response</span></span>
<span data-ttu-id="f661c-175">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f661c-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f661c-176">示例</span><span class="sxs-lookup"><span data-stu-id="f661c-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f661c-177">请求</span><span class="sxs-lookup"><span data-stu-id="f661c-177">Request</span></span>
<span data-ttu-id="f661c-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f661c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
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

### <a name="response"></a><span data-ttu-id="f661c-179">响应</span><span class="sxs-lookup"><span data-stu-id="f661c-179">Response</span></span>
<span data-ttu-id="f661c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f661c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





