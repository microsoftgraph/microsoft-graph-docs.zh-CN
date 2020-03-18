---
title: 更新 deviceManagementExportJob
description: 更新 deviceManagementExportJob 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34c4b952b14b012d6eea73cf792ae8efba415d8f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801409"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="0e5d0-103">更新 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="0e5d0-103">Update deviceManagementExportJob</span></span>

> <span data-ttu-id="0e5d0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e5d0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e5d0-106">更新[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-106">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e5d0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e5d0-107">Prerequisites</span></span>
<span data-ttu-id="0e5d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e5d0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e5d0-110">Permission type</span></span>|<span data-ttu-id="0e5d0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e5d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e5d0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e5d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e5d0-113">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="0e5d0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0e5d0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e5d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e5d0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-115">Not supported.</span></span>|
|<span data-ttu-id="0e5d0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e5d0-116">Application</span></span>|<span data-ttu-id="0e5d0-117">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="0e5d0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e5d0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e5d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="0e5d0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e5d0-119">Request headers</span></span>
|<span data-ttu-id="0e5d0-120">标头</span><span class="sxs-lookup"><span data-stu-id="0e5d0-120">Header</span></span>|<span data-ttu-id="0e5d0-121">值</span><span class="sxs-lookup"><span data-stu-id="0e5d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e5d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e5d0-122">Authorization</span></span>|<span data-ttu-id="0e5d0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e5d0-124">接受</span><span class="sxs-lookup"><span data-stu-id="0e5d0-124">Accept</span></span>|<span data-ttu-id="0e5d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e5d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e5d0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e5d0-126">Request body</span></span>
<span data-ttu-id="0e5d0-127">在请求正文中，提供[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-127">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="0e5d0-128">下表显示创建[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-128">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="0e5d0-129">属性</span><span class="sxs-lookup"><span data-stu-id="0e5d0-129">Property</span></span>|<span data-ttu-id="0e5d0-130">类型</span><span class="sxs-lookup"><span data-stu-id="0e5d0-130">Type</span></span>|<span data-ttu-id="0e5d0-131">说明</span><span class="sxs-lookup"><span data-stu-id="0e5d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e5d0-132">id</span><span class="sxs-lookup"><span data-stu-id="0e5d0-132">id</span></span>|<span data-ttu-id="0e5d0-133">String</span><span class="sxs-lookup"><span data-stu-id="0e5d0-133">String</span></span>|<span data-ttu-id="0e5d0-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0e5d0-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="0e5d0-135">reportName</span><span class="sxs-lookup"><span data-stu-id="0e5d0-135">reportName</span></span>|<span data-ttu-id="0e5d0-136">String</span><span class="sxs-lookup"><span data-stu-id="0e5d0-136">String</span></span>|<span data-ttu-id="0e5d0-137">报告的名称</span><span class="sxs-lookup"><span data-stu-id="0e5d0-137">Name of the report</span></span>|
|<span data-ttu-id="0e5d0-138">filter</span><span class="sxs-lookup"><span data-stu-id="0e5d0-138">filter</span></span>|<span data-ttu-id="0e5d0-139">String</span><span class="sxs-lookup"><span data-stu-id="0e5d0-139">String</span></span>|<span data-ttu-id="0e5d0-140">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="0e5d0-140">Filters applied on the report</span></span>|
|<span data-ttu-id="0e5d0-141">select</span><span class="sxs-lookup"><span data-stu-id="0e5d0-141">select</span></span>|<span data-ttu-id="0e5d0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0e5d0-142">String collection</span></span>|<span data-ttu-id="0e5d0-143">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="0e5d0-143">Columns selected from the report</span></span>|
|<span data-ttu-id="0e5d0-144">format</span><span class="sxs-lookup"><span data-stu-id="0e5d0-144">format</span></span>|[<span data-ttu-id="0e5d0-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="0e5d0-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="0e5d0-146">导出的报表的格式。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-146">Format of the exported report.</span></span> <span data-ttu-id="0e5d0-147">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="0e5d0-148">snapshotId</span><span class="sxs-lookup"><span data-stu-id="0e5d0-148">snapshotId</span></span>|<span data-ttu-id="0e5d0-149">String</span><span class="sxs-lookup"><span data-stu-id="0e5d0-149">String</span></span>|<span data-ttu-id="0e5d0-150">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="0e5d0-151">可以在此处使用 sessionId 或 CachedReportConfiguration id。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="0e5d0-152">如果指定了 sessionId，则筛选器、Select 和 OrderBy 将应用于 sessionId 所代表的数据。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="0e5d0-153">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="0e5d0-154">状态</span><span class="sxs-lookup"><span data-stu-id="0e5d0-154">status</span></span>|[<span data-ttu-id="0e5d0-155">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="0e5d0-155">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="0e5d0-156">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-156">Status of the export job.</span></span> <span data-ttu-id="0e5d0-157">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-157">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="0e5d0-158">url</span><span class="sxs-lookup"><span data-stu-id="0e5d0-158">url</span></span>|<span data-ttu-id="0e5d0-159">String</span><span class="sxs-lookup"><span data-stu-id="0e5d0-159">String</span></span>|<span data-ttu-id="0e5d0-160">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="0e5d0-160">Temporary location of the exported report</span></span>|
|<span data-ttu-id="0e5d0-161">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="0e5d0-161">requestDateTime</span></span>|<span data-ttu-id="0e5d0-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e5d0-162">DateTimeOffset</span></span>|<span data-ttu-id="0e5d0-163">请求导出的报告的时间</span><span class="sxs-lookup"><span data-stu-id="0e5d0-163">Time that the exported report was requested</span></span>|
|<span data-ttu-id="0e5d0-164">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e5d0-164">expirationDateTime</span></span>|<span data-ttu-id="0e5d0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e5d0-165">DateTimeOffset</span></span>|<span data-ttu-id="0e5d0-166">导出的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="0e5d0-166">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="0e5d0-167">响应</span><span class="sxs-lookup"><span data-stu-id="0e5d0-167">Response</span></span>
<span data-ttu-id="0e5d0-168">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e5d0-169">示例</span><span class="sxs-lookup"><span data-stu-id="0e5d0-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e5d0-170">请求</span><span class="sxs-lookup"><span data-stu-id="0e5d0-170">Request</span></span>
<span data-ttu-id="0e5d0-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="0e5d0-172">响应</span><span class="sxs-lookup"><span data-stu-id="0e5d0-172">Response</span></span>
<span data-ttu-id="0e5d0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e5d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




