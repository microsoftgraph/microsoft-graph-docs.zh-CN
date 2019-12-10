---
title: 创建 deviceManagementExportJob
description: 创建新的 deviceManagementExportJob 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1552a722a5dd33c987ea137ed1be42675074a49
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940346"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="08fc3-103">创建 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="08fc3-103">Create deviceManagementExportJob</span></span>

> <span data-ttu-id="08fc3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08fc3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08fc3-106">创建新的[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08fc3-106">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08fc3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08fc3-107">Prerequisites</span></span>
<span data-ttu-id="08fc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08fc3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08fc3-110">Permission type</span></span>|<span data-ttu-id="08fc3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08fc3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08fc3-113">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="08fc3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08fc3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08fc3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08fc3-115">Not supported.</span></span>|
|<span data-ttu-id="08fc3-116">Application</span><span class="sxs-lookup"><span data-stu-id="08fc3-116">Application</span></span>|<span data-ttu-id="08fc3-117">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="08fc3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08fc3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="08fc3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="08fc3-119">Request headers</span></span>
|<span data-ttu-id="08fc3-120">标头</span><span class="sxs-lookup"><span data-stu-id="08fc3-120">Header</span></span>|<span data-ttu-id="08fc3-121">值</span><span class="sxs-lookup"><span data-stu-id="08fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08fc3-122">授权</span><span class="sxs-lookup"><span data-stu-id="08fc3-122">Authorization</span></span>|<span data-ttu-id="08fc3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08fc3-124">接受</span><span class="sxs-lookup"><span data-stu-id="08fc3-124">Accept</span></span>|<span data-ttu-id="08fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08fc3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08fc3-126">Request body</span></span>
<span data-ttu-id="08fc3-127">在请求正文中，提供 deviceManagementExportJob 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08fc3-127">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="08fc3-128">下表显示创建 deviceManagementExportJob 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08fc3-128">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="08fc3-129">属性</span><span class="sxs-lookup"><span data-stu-id="08fc3-129">Property</span></span>|<span data-ttu-id="08fc3-130">类型</span><span class="sxs-lookup"><span data-stu-id="08fc3-130">Type</span></span>|<span data-ttu-id="08fc3-131">说明</span><span class="sxs-lookup"><span data-stu-id="08fc3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08fc3-132">id</span><span class="sxs-lookup"><span data-stu-id="08fc3-132">id</span></span>|<span data-ttu-id="08fc3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="08fc3-133">String</span></span>|<span data-ttu-id="08fc3-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="08fc3-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="08fc3-135">reportName</span><span class="sxs-lookup"><span data-stu-id="08fc3-135">reportName</span></span>|<span data-ttu-id="08fc3-136">字符串</span><span class="sxs-lookup"><span data-stu-id="08fc3-136">String</span></span>|<span data-ttu-id="08fc3-137">报告的名称</span><span class="sxs-lookup"><span data-stu-id="08fc3-137">Name of the report</span></span>|
|<span data-ttu-id="08fc3-138">filter</span><span class="sxs-lookup"><span data-stu-id="08fc3-138">filter</span></span>|<span data-ttu-id="08fc3-139">字符串</span><span class="sxs-lookup"><span data-stu-id="08fc3-139">String</span></span>|<span data-ttu-id="08fc3-140">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="08fc3-140">Filters applied on the report</span></span>|
|<span data-ttu-id="08fc3-141">select</span><span class="sxs-lookup"><span data-stu-id="08fc3-141">select</span></span>|<span data-ttu-id="08fc3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="08fc3-142">String collection</span></span>|<span data-ttu-id="08fc3-143">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="08fc3-143">Columns selected from the report</span></span>|
|<span data-ttu-id="08fc3-144">format</span><span class="sxs-lookup"><span data-stu-id="08fc3-144">format</span></span>|[<span data-ttu-id="08fc3-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="08fc3-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="08fc3-146">导出的报表的格式。</span><span class="sxs-lookup"><span data-stu-id="08fc3-146">Format of the exported report.</span></span> <span data-ttu-id="08fc3-147">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="08fc3-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="08fc3-148">snapshotId</span><span class="sxs-lookup"><span data-stu-id="08fc3-148">snapshotId</span></span>|<span data-ttu-id="08fc3-149">字符串</span><span class="sxs-lookup"><span data-stu-id="08fc3-149">String</span></span>|<span data-ttu-id="08fc3-150">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="08fc3-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="08fc3-151">可以在此处使用 sessionId 或 CachedReportConfiguration id。</span><span class="sxs-lookup"><span data-stu-id="08fc3-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="08fc3-152">如果指定了 sessionId，则筛选器、Select 和 OrderBy 将应用于 sessionId 所代表的数据。</span><span class="sxs-lookup"><span data-stu-id="08fc3-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="08fc3-153">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="08fc3-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="08fc3-154">状态</span><span class="sxs-lookup"><span data-stu-id="08fc3-154">status</span></span>|[<span data-ttu-id="08fc3-155">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="08fc3-155">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="08fc3-156">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="08fc3-156">Status of the export job.</span></span> <span data-ttu-id="08fc3-157">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="08fc3-157">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="08fc3-158">url</span><span class="sxs-lookup"><span data-stu-id="08fc3-158">url</span></span>|<span data-ttu-id="08fc3-159">String</span><span class="sxs-lookup"><span data-stu-id="08fc3-159">String</span></span>|<span data-ttu-id="08fc3-160">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="08fc3-160">Temporary location of the exported report</span></span>|
|<span data-ttu-id="08fc3-161">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="08fc3-161">requestDateTime</span></span>|<span data-ttu-id="08fc3-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fc3-162">DateTimeOffset</span></span>|<span data-ttu-id="08fc3-163">请求导出的报告的时间</span><span class="sxs-lookup"><span data-stu-id="08fc3-163">Time that the exported report was requested</span></span>|
|<span data-ttu-id="08fc3-164">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="08fc3-164">expirationDateTime</span></span>|<span data-ttu-id="08fc3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fc3-165">DateTimeOffset</span></span>|<span data-ttu-id="08fc3-166">导出的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="08fc3-166">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="08fc3-167">响应</span><span class="sxs-lookup"><span data-stu-id="08fc3-167">Response</span></span>
<span data-ttu-id="08fc3-168">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08fc3-168">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08fc3-169">示例</span><span class="sxs-lookup"><span data-stu-id="08fc3-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="08fc3-170">请求</span><span class="sxs-lookup"><span data-stu-id="08fc3-170">Request</span></span>
<span data-ttu-id="08fc3-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08fc3-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="08fc3-172">响应</span><span class="sxs-lookup"><span data-stu-id="08fc3-172">Response</span></span>
<span data-ttu-id="08fc3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08fc3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





