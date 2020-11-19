---
title: 创建 deviceManagementReportSchedule
description: 创建新的 deviceManagementReportSchedule 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f91038e518550b9ebfc50d59c3a0168d8e489cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257623"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="8be9a-103">创建 deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="8be9a-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="8be9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8be9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8be9a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8be9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8be9a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8be9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8be9a-107">创建新的 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8be9a-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8be9a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8be9a-108">Prerequisites</span></span>
<span data-ttu-id="8be9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8be9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8be9a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8be9a-111">Permission type</span></span>|<span data-ttu-id="8be9a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8be9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8be9a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8be9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8be9a-114">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="8be9a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8be9a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8be9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8be9a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8be9a-116">Not supported.</span></span>|
|<span data-ttu-id="8be9a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8be9a-117">Application</span></span>|<span data-ttu-id="8be9a-118">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="8be9a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8be9a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8be9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="8be9a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8be9a-120">Request headers</span></span>
|<span data-ttu-id="8be9a-121">标头</span><span class="sxs-lookup"><span data-stu-id="8be9a-121">Header</span></span>|<span data-ttu-id="8be9a-122">值</span><span class="sxs-lookup"><span data-stu-id="8be9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8be9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8be9a-123">Authorization</span></span>|<span data-ttu-id="8be9a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8be9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8be9a-125">接受</span><span class="sxs-lookup"><span data-stu-id="8be9a-125">Accept</span></span>|<span data-ttu-id="8be9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8be9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8be9a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8be9a-127">Request body</span></span>
<span data-ttu-id="8be9a-128">在请求正文中，提供 deviceManagementReportSchedule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8be9a-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="8be9a-129">下表显示创建 deviceManagementReportSchedule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8be9a-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="8be9a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8be9a-130">Property</span></span>|<span data-ttu-id="8be9a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8be9a-131">Type</span></span>|<span data-ttu-id="8be9a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8be9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8be9a-133">id</span><span class="sxs-lookup"><span data-stu-id="8be9a-133">id</span></span>|<span data-ttu-id="8be9a-134">String</span><span class="sxs-lookup"><span data-stu-id="8be9a-134">String</span></span>|<span data-ttu-id="8be9a-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8be9a-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="8be9a-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="8be9a-136">reportScheduleName</span></span>|<span data-ttu-id="8be9a-137">String</span><span class="sxs-lookup"><span data-stu-id="8be9a-137">String</span></span>|<span data-ttu-id="8be9a-138">计划的名称</span><span class="sxs-lookup"><span data-stu-id="8be9a-138">Name of the schedule</span></span>|
|<span data-ttu-id="8be9a-139">subject</span><span class="sxs-lookup"><span data-stu-id="8be9a-139">subject</span></span>|<span data-ttu-id="8be9a-140">String</span><span class="sxs-lookup"><span data-stu-id="8be9a-140">String</span></span>|<span data-ttu-id="8be9a-141">已传递的计划报告的主题</span><span class="sxs-lookup"><span data-stu-id="8be9a-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="8be9a-142">电子邮件</span><span class="sxs-lookup"><span data-stu-id="8be9a-142">emails</span></span>|<span data-ttu-id="8be9a-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="8be9a-143">String collection</span></span>|<span data-ttu-id="8be9a-144">计划报告传递到的电子邮件</span><span class="sxs-lookup"><span data-stu-id="8be9a-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="8be9a-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="8be9a-145">recurrence</span></span>|[<span data-ttu-id="8be9a-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="8be9a-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="8be9a-147">计划报告传递的频率。</span><span class="sxs-lookup"><span data-stu-id="8be9a-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="8be9a-148">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="8be9a-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="8be9a-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8be9a-149">startDateTime</span></span>|<span data-ttu-id="8be9a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8be9a-150">DateTimeOffset</span></span>|<span data-ttu-id="8be9a-151">计划报告的开始交付时间</span><span class="sxs-lookup"><span data-stu-id="8be9a-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="8be9a-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8be9a-152">endDateTime</span></span>|<span data-ttu-id="8be9a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8be9a-153">DateTimeOffset</span></span>|<span data-ttu-id="8be9a-154">计划报告的结束传递时间</span><span class="sxs-lookup"><span data-stu-id="8be9a-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="8be9a-155">userId</span><span class="sxs-lookup"><span data-stu-id="8be9a-155">userId</span></span>|<span data-ttu-id="8be9a-156">String</span><span class="sxs-lookup"><span data-stu-id="8be9a-156">String</span></span>|<span data-ttu-id="8be9a-157">创建报表的用户的 Id</span><span class="sxs-lookup"><span data-stu-id="8be9a-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="8be9a-158">reportName</span><span class="sxs-lookup"><span data-stu-id="8be9a-158">reportName</span></span>|<span data-ttu-id="8be9a-159">String</span><span class="sxs-lookup"><span data-stu-id="8be9a-159">String</span></span>|<span data-ttu-id="8be9a-160">报告的名称</span><span class="sxs-lookup"><span data-stu-id="8be9a-160">Name of the report</span></span>|
|<span data-ttu-id="8be9a-161">filter</span><span class="sxs-lookup"><span data-stu-id="8be9a-161">filter</span></span>|<span data-ttu-id="8be9a-162">String</span><span class="sxs-lookup"><span data-stu-id="8be9a-162">String</span></span>|<span data-ttu-id="8be9a-163">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="8be9a-163">Filters applied on the report</span></span>|
|<span data-ttu-id="8be9a-164">select</span><span class="sxs-lookup"><span data-stu-id="8be9a-164">select</span></span>|<span data-ttu-id="8be9a-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="8be9a-165">String collection</span></span>|<span data-ttu-id="8be9a-166">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="8be9a-166">Columns selected from the report</span></span>|
|<span data-ttu-id="8be9a-167">By</span><span class="sxs-lookup"><span data-stu-id="8be9a-167">orderBy</span></span>|<span data-ttu-id="8be9a-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="8be9a-168">String collection</span></span>|<span data-ttu-id="8be9a-169">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="8be9a-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="8be9a-170">format</span><span class="sxs-lookup"><span data-stu-id="8be9a-170">format</span></span>|[<span data-ttu-id="8be9a-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="8be9a-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="8be9a-172">计划报告的格式。</span><span class="sxs-lookup"><span data-stu-id="8be9a-172">Format of the scheduled report.</span></span> <span data-ttu-id="8be9a-173">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="8be9a-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="8be9a-174">响应</span><span class="sxs-lookup"><span data-stu-id="8be9a-174">Response</span></span>
<span data-ttu-id="8be9a-175">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8be9a-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8be9a-176">示例</span><span class="sxs-lookup"><span data-stu-id="8be9a-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="8be9a-177">请求</span><span class="sxs-lookup"><span data-stu-id="8be9a-177">Request</span></span>
<span data-ttu-id="8be9a-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8be9a-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8be9a-179">响应</span><span class="sxs-lookup"><span data-stu-id="8be9a-179">Response</span></span>
<span data-ttu-id="8be9a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8be9a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




