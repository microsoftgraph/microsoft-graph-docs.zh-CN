---
title: 更新 deviceManagementExportJob
description: 更新 deviceManagementExportJob 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4951d458500a0d6863eebed807aa5e2120496376
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537259"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="bf552-103">更新 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="bf552-103">Update deviceManagementExportJob</span></span>

> <span data-ttu-id="bf552-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf552-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf552-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf552-106">更新[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf552-106">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf552-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf552-107">Prerequisites</span></span>
<span data-ttu-id="bf552-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf552-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf552-110">Permission type</span></span>|<span data-ttu-id="bf552-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf552-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf552-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf552-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf552-113">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="bf552-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bf552-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf552-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf552-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf552-115">Not supported.</span></span>|
|<span data-ttu-id="bf552-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf552-116">Application</span></span>|<span data-ttu-id="bf552-117">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="bf552-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf552-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf552-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="bf552-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf552-119">Request headers</span></span>
|<span data-ttu-id="bf552-120">标头</span><span class="sxs-lookup"><span data-stu-id="bf552-120">Header</span></span>|<span data-ttu-id="bf552-121">值</span><span class="sxs-lookup"><span data-stu-id="bf552-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf552-122">授权</span><span class="sxs-lookup"><span data-stu-id="bf552-122">Authorization</span></span>|<span data-ttu-id="bf552-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf552-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf552-124">接受</span><span class="sxs-lookup"><span data-stu-id="bf552-124">Accept</span></span>|<span data-ttu-id="bf552-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf552-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf552-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf552-126">Request body</span></span>
<span data-ttu-id="bf552-127">在请求正文中，提供[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf552-127">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="bf552-128">下表显示创建[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bf552-128">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="bf552-129">属性</span><span class="sxs-lookup"><span data-stu-id="bf552-129">Property</span></span>|<span data-ttu-id="bf552-130">类型</span><span class="sxs-lookup"><span data-stu-id="bf552-130">Type</span></span>|<span data-ttu-id="bf552-131">说明</span><span class="sxs-lookup"><span data-stu-id="bf552-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf552-132">id</span><span class="sxs-lookup"><span data-stu-id="bf552-132">id</span></span>|<span data-ttu-id="bf552-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bf552-133">String</span></span>|<span data-ttu-id="bf552-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bf552-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="bf552-135">reportName</span><span class="sxs-lookup"><span data-stu-id="bf552-135">reportName</span></span>|<span data-ttu-id="bf552-136">字符串</span><span class="sxs-lookup"><span data-stu-id="bf552-136">String</span></span>|<span data-ttu-id="bf552-137">报告的名称</span><span class="sxs-lookup"><span data-stu-id="bf552-137">Name of the report</span></span>|
|<span data-ttu-id="bf552-138">filter</span><span class="sxs-lookup"><span data-stu-id="bf552-138">filter</span></span>|<span data-ttu-id="bf552-139">字符串</span><span class="sxs-lookup"><span data-stu-id="bf552-139">String</span></span>|<span data-ttu-id="bf552-140">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="bf552-140">Filters applied on the report</span></span>|
|<span data-ttu-id="bf552-141">select</span><span class="sxs-lookup"><span data-stu-id="bf552-141">select</span></span>|<span data-ttu-id="bf552-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="bf552-142">String collection</span></span>|<span data-ttu-id="bf552-143">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="bf552-143">Columns selected from the report</span></span>|
|<span data-ttu-id="bf552-144">By</span><span class="sxs-lookup"><span data-stu-id="bf552-144">orderBy</span></span>|<span data-ttu-id="bf552-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="bf552-145">String collection</span></span>|<span data-ttu-id="bf552-146">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="bf552-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="bf552-147">format</span><span class="sxs-lookup"><span data-stu-id="bf552-147">format</span></span>|[<span data-ttu-id="bf552-148">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="bf552-148">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="bf552-149">导出的报表的格式。</span><span class="sxs-lookup"><span data-stu-id="bf552-149">Format of the exported report.</span></span> <span data-ttu-id="bf552-150">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="bf552-150">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="bf552-151">snapshotId</span><span class="sxs-lookup"><span data-stu-id="bf552-151">snapshotId</span></span>|<span data-ttu-id="bf552-152">字符串</span><span class="sxs-lookup"><span data-stu-id="bf552-152">String</span></span>|<span data-ttu-id="bf552-153">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="bf552-153">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="bf552-154">可以在此处使用 sessionId 或 CachedReportConfiguration id。</span><span class="sxs-lookup"><span data-stu-id="bf552-154">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="bf552-155">如果指定了 sessionId，则筛选器、Select 和 OrderBy 将应用于 sessionId 所代表的数据。</span><span class="sxs-lookup"><span data-stu-id="bf552-155">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="bf552-156">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="bf552-156">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="bf552-157">status</span><span class="sxs-lookup"><span data-stu-id="bf552-157">status</span></span>|[<span data-ttu-id="bf552-158">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="bf552-158">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="bf552-159">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="bf552-159">Status of the export job.</span></span> <span data-ttu-id="bf552-160">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="bf552-160">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="bf552-161">url</span><span class="sxs-lookup"><span data-stu-id="bf552-161">url</span></span>|<span data-ttu-id="bf552-162">String</span><span class="sxs-lookup"><span data-stu-id="bf552-162">String</span></span>|<span data-ttu-id="bf552-163">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="bf552-163">Temporary location of the exported report</span></span>|
|<span data-ttu-id="bf552-164">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="bf552-164">requestDateTime</span></span>|<span data-ttu-id="bf552-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf552-165">DateTimeOffset</span></span>|<span data-ttu-id="bf552-166">请求导出的报告的时间</span><span class="sxs-lookup"><span data-stu-id="bf552-166">Time that the exported report was requested</span></span>|
|<span data-ttu-id="bf552-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bf552-167">expirationDateTime</span></span>|<span data-ttu-id="bf552-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf552-168">DateTimeOffset</span></span>|<span data-ttu-id="bf552-169">导出的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="bf552-169">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="bf552-170">响应</span><span class="sxs-lookup"><span data-stu-id="bf552-170">Response</span></span>
<span data-ttu-id="bf552-171">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf552-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf552-172">示例</span><span class="sxs-lookup"><span data-stu-id="bf552-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf552-173">请求</span><span class="sxs-lookup"><span data-stu-id="bf552-173">Request</span></span>
<span data-ttu-id="bf552-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf552-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 448

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bf552-175">响应</span><span class="sxs-lookup"><span data-stu-id="bf552-175">Response</span></span>
<span data-ttu-id="bf552-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf552-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```






