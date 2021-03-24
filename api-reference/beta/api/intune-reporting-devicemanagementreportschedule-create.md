---
title: 创建 deviceManagementReportSchedule
description: 创建新的 deviceManagementReportSchedule 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9e29979c0999d05592adaad8e2f19a332a57a8a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134387"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="70739-103">创建 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="70739-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="70739-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70739-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70739-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70739-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70739-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70739-107">创建新的 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70739-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70739-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="70739-108">Prerequisites</span></span>
<span data-ttu-id="70739-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70739-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="70739-111">Permission type</span></span>|<span data-ttu-id="70739-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70739-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70739-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70739-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70739-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70739-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="70739-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70739-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70739-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70739-116">Not supported.</span></span>|
|<span data-ttu-id="70739-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70739-117">Application</span></span>|<span data-ttu-id="70739-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70739-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70739-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70739-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="70739-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70739-120">Request headers</span></span>
|<span data-ttu-id="70739-121">标头</span><span class="sxs-lookup"><span data-stu-id="70739-121">Header</span></span>|<span data-ttu-id="70739-122">值</span><span class="sxs-lookup"><span data-stu-id="70739-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70739-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70739-123">Authorization</span></span>|<span data-ttu-id="70739-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70739-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70739-125">接受</span><span class="sxs-lookup"><span data-stu-id="70739-125">Accept</span></span>|<span data-ttu-id="70739-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70739-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70739-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70739-127">Request body</span></span>
<span data-ttu-id="70739-128">在请求正文中，提供 deviceManagementReportSchedule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70739-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="70739-129">下表显示创建 deviceManagementReportSchedule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="70739-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="70739-130">属性</span><span class="sxs-lookup"><span data-stu-id="70739-130">Property</span></span>|<span data-ttu-id="70739-131">类型</span><span class="sxs-lookup"><span data-stu-id="70739-131">Type</span></span>|<span data-ttu-id="70739-132">说明</span><span class="sxs-lookup"><span data-stu-id="70739-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70739-133">id</span><span class="sxs-lookup"><span data-stu-id="70739-133">id</span></span>|<span data-ttu-id="70739-134">String</span><span class="sxs-lookup"><span data-stu-id="70739-134">String</span></span>|<span data-ttu-id="70739-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="70739-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="70739-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="70739-136">reportScheduleName</span></span>|<span data-ttu-id="70739-137">String</span><span class="sxs-lookup"><span data-stu-id="70739-137">String</span></span>|<span data-ttu-id="70739-138">计划的名称</span><span class="sxs-lookup"><span data-stu-id="70739-138">Name of the schedule</span></span>|
|<span data-ttu-id="70739-139">subject</span><span class="sxs-lookup"><span data-stu-id="70739-139">subject</span></span>|<span data-ttu-id="70739-140">String</span><span class="sxs-lookup"><span data-stu-id="70739-140">String</span></span>|<span data-ttu-id="70739-141">已送达的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="70739-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="70739-142">电子邮件</span><span class="sxs-lookup"><span data-stu-id="70739-142">emails</span></span>|<span data-ttu-id="70739-143">String collection</span><span class="sxs-lookup"><span data-stu-id="70739-143">String collection</span></span>|<span data-ttu-id="70739-144">将计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="70739-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="70739-145">定期</span><span class="sxs-lookup"><span data-stu-id="70739-145">recurrence</span></span>|[<span data-ttu-id="70739-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="70739-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="70739-147">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="70739-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="70739-148">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="70739-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="70739-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="70739-149">startDateTime</span></span>|<span data-ttu-id="70739-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70739-150">DateTimeOffset</span></span>|<span data-ttu-id="70739-151">计划报告交付开始的时间</span><span class="sxs-lookup"><span data-stu-id="70739-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="70739-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="70739-152">endDateTime</span></span>|<span data-ttu-id="70739-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70739-153">DateTimeOffset</span></span>|<span data-ttu-id="70739-154">计划报告传递结束的时间</span><span class="sxs-lookup"><span data-stu-id="70739-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="70739-155">userId</span><span class="sxs-lookup"><span data-stu-id="70739-155">userId</span></span>|<span data-ttu-id="70739-156">String</span><span class="sxs-lookup"><span data-stu-id="70739-156">String</span></span>|<span data-ttu-id="70739-157">创建报告的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="70739-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="70739-158">reportName</span><span class="sxs-lookup"><span data-stu-id="70739-158">reportName</span></span>|<span data-ttu-id="70739-159">String</span><span class="sxs-lookup"><span data-stu-id="70739-159">String</span></span>|<span data-ttu-id="70739-160">报告的名称</span><span class="sxs-lookup"><span data-stu-id="70739-160">Name of the report</span></span>|
|<span data-ttu-id="70739-161">filter</span><span class="sxs-lookup"><span data-stu-id="70739-161">filter</span></span>|<span data-ttu-id="70739-162">String</span><span class="sxs-lookup"><span data-stu-id="70739-162">String</span></span>|<span data-ttu-id="70739-163">应用于报表的筛选器</span><span class="sxs-lookup"><span data-stu-id="70739-163">Filters applied on the report</span></span>|
|<span data-ttu-id="70739-164">select</span><span class="sxs-lookup"><span data-stu-id="70739-164">select</span></span>|<span data-ttu-id="70739-165">String collection</span><span class="sxs-lookup"><span data-stu-id="70739-165">String collection</span></span>|<span data-ttu-id="70739-166">从报表选择的列</span><span class="sxs-lookup"><span data-stu-id="70739-166">Columns selected from the report</span></span>|
|<span data-ttu-id="70739-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="70739-167">orderBy</span></span>|<span data-ttu-id="70739-168">String collection</span><span class="sxs-lookup"><span data-stu-id="70739-168">String collection</span></span>|<span data-ttu-id="70739-169">报告中列的排序</span><span class="sxs-lookup"><span data-stu-id="70739-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="70739-170">format</span><span class="sxs-lookup"><span data-stu-id="70739-170">format</span></span>|[<span data-ttu-id="70739-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="70739-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="70739-172">计划报表的格式。</span><span class="sxs-lookup"><span data-stu-id="70739-172">Format of the scheduled report.</span></span> <span data-ttu-id="70739-173">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="70739-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="70739-174">响应</span><span class="sxs-lookup"><span data-stu-id="70739-174">Response</span></span>
<span data-ttu-id="70739-175">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70739-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70739-176">示例</span><span class="sxs-lookup"><span data-stu-id="70739-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="70739-177">请求</span><span class="sxs-lookup"><span data-stu-id="70739-177">Request</span></span>
<span data-ttu-id="70739-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70739-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70739-179">响应</span><span class="sxs-lookup"><span data-stu-id="70739-179">Response</span></span>
<span data-ttu-id="70739-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70739-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




