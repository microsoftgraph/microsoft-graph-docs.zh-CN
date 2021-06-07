---
title: 更新 deviceManagementExportJob
description: 更新 deviceManagementExportJob 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aac5f773d14a22d1aea76319138e500028454ead
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748917"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="b8d40-103">更新 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="b8d40-103">Update deviceManagementExportJob</span></span>

<span data-ttu-id="b8d40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8d40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8d40-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8d40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8d40-106">更新 [deviceManagementExportJob 对象](../resources/intune-reporting-devicemanagementexportjob.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b8d40-106">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8d40-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8d40-107">Prerequisites</span></span>
<span data-ttu-id="b8d40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8d40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d40-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8d40-110">Permission type</span></span>|<span data-ttu-id="b8d40-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8d40-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8d40-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8d40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8d40-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8d40-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8d40-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8d40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8d40-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8d40-115">Not supported.</span></span>|
|<span data-ttu-id="b8d40-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8d40-116">Application</span></span>|<span data-ttu-id="b8d40-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8d40-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8d40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8d40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="b8d40-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8d40-119">Request headers</span></span>
|<span data-ttu-id="b8d40-120">标头</span><span class="sxs-lookup"><span data-stu-id="b8d40-120">Header</span></span>|<span data-ttu-id="b8d40-121">值</span><span class="sxs-lookup"><span data-stu-id="b8d40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8d40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d40-122">Authorization</span></span>|<span data-ttu-id="b8d40-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8d40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8d40-124">接受</span><span class="sxs-lookup"><span data-stu-id="b8d40-124">Accept</span></span>|<span data-ttu-id="b8d40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8d40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8d40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8d40-126">Request body</span></span>
<span data-ttu-id="b8d40-127">在请求正文中，提供 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8d40-127">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="b8d40-128">下表显示创建 [deviceManagementExportJob 时所需的属性](../resources/intune-reporting-devicemanagementexportjob.md)。</span><span class="sxs-lookup"><span data-stu-id="b8d40-128">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="b8d40-129">属性</span><span class="sxs-lookup"><span data-stu-id="b8d40-129">Property</span></span>|<span data-ttu-id="b8d40-130">类型</span><span class="sxs-lookup"><span data-stu-id="b8d40-130">Type</span></span>|<span data-ttu-id="b8d40-131">说明</span><span class="sxs-lookup"><span data-stu-id="b8d40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8d40-132">id</span><span class="sxs-lookup"><span data-stu-id="b8d40-132">id</span></span>|<span data-ttu-id="b8d40-133">String</span><span class="sxs-lookup"><span data-stu-id="b8d40-133">String</span></span>|<span data-ttu-id="b8d40-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b8d40-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="b8d40-135">reportName</span><span class="sxs-lookup"><span data-stu-id="b8d40-135">reportName</span></span>|<span data-ttu-id="b8d40-136">String</span><span class="sxs-lookup"><span data-stu-id="b8d40-136">String</span></span>|<span data-ttu-id="b8d40-137">报告的名称</span><span class="sxs-lookup"><span data-stu-id="b8d40-137">Name of the report</span></span>|
|<span data-ttu-id="b8d40-138">filter</span><span class="sxs-lookup"><span data-stu-id="b8d40-138">filter</span></span>|<span data-ttu-id="b8d40-139">String</span><span class="sxs-lookup"><span data-stu-id="b8d40-139">String</span></span>|<span data-ttu-id="b8d40-140">应用于报表的筛选器</span><span class="sxs-lookup"><span data-stu-id="b8d40-140">Filters applied on the report</span></span>|
|<span data-ttu-id="b8d40-141">select</span><span class="sxs-lookup"><span data-stu-id="b8d40-141">select</span></span>|<span data-ttu-id="b8d40-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b8d40-142">String collection</span></span>|<span data-ttu-id="b8d40-143">从报表选择的列</span><span class="sxs-lookup"><span data-stu-id="b8d40-143">Columns selected from the report</span></span>|
|<span data-ttu-id="b8d40-144">format</span><span class="sxs-lookup"><span data-stu-id="b8d40-144">format</span></span>|[<span data-ttu-id="b8d40-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="b8d40-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="b8d40-146">导出的报告的格式。</span><span class="sxs-lookup"><span data-stu-id="b8d40-146">Format of the exported report.</span></span> <span data-ttu-id="b8d40-147">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="b8d40-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="b8d40-148">snapshotId</span><span class="sxs-lookup"><span data-stu-id="b8d40-148">snapshotId</span></span>|<span data-ttu-id="b8d40-149">String</span><span class="sxs-lookup"><span data-stu-id="b8d40-149">String</span></span>|<span data-ttu-id="b8d40-150">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="b8d40-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="b8d40-151">可以在此处使用 sessionId 或 CachedReportConfiguration ID。</span><span class="sxs-lookup"><span data-stu-id="b8d40-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="b8d40-152">如果指定了 sessionId，则 Filter、Select 和 OrderBy 将应用于 sessionId 表示的数据。</span><span class="sxs-lookup"><span data-stu-id="b8d40-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="b8d40-153">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="b8d40-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="b8d40-154">localizationType</span><span class="sxs-lookup"><span data-stu-id="b8d40-154">localizationType</span></span>|[<span data-ttu-id="b8d40-155">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="b8d40-155">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="b8d40-156">配置所请求的导出作业的本地化方式。</span><span class="sxs-lookup"><span data-stu-id="b8d40-156">Configures how the requested export job is localized.</span></span> <span data-ttu-id="b8d40-157">可取值为：`localizedValuesAsAdditionalColumn`、`replaceLocalizableValues`。</span><span class="sxs-lookup"><span data-stu-id="b8d40-157">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="b8d40-158">状态</span><span class="sxs-lookup"><span data-stu-id="b8d40-158">status</span></span>|[<span data-ttu-id="b8d40-159">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="b8d40-159">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="b8d40-160">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="b8d40-160">Status of the export job.</span></span> <span data-ttu-id="b8d40-161">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b8d40-161">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="b8d40-162">url</span><span class="sxs-lookup"><span data-stu-id="b8d40-162">url</span></span>|<span data-ttu-id="b8d40-163">String</span><span class="sxs-lookup"><span data-stu-id="b8d40-163">String</span></span>|<span data-ttu-id="b8d40-164">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="b8d40-164">Temporary location of the exported report</span></span>|
|<span data-ttu-id="b8d40-165">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="b8d40-165">requestDateTime</span></span>|<span data-ttu-id="b8d40-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8d40-166">DateTimeOffset</span></span>|<span data-ttu-id="b8d40-167">请求导出报告的时间</span><span class="sxs-lookup"><span data-stu-id="b8d40-167">Time that the exported report was requested</span></span>|
|<span data-ttu-id="b8d40-168">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b8d40-168">expirationDateTime</span></span>|<span data-ttu-id="b8d40-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8d40-169">DateTimeOffset</span></span>|<span data-ttu-id="b8d40-170">导出报告的过期时间</span><span class="sxs-lookup"><span data-stu-id="b8d40-170">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="b8d40-171">响应</span><span class="sxs-lookup"><span data-stu-id="b8d40-171">Response</span></span>
<span data-ttu-id="b8d40-172">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8d40-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d40-173">示例</span><span class="sxs-lookup"><span data-stu-id="b8d40-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8d40-174">请求</span><span class="sxs-lookup"><span data-stu-id="b8d40-174">Request</span></span>
<span data-ttu-id="b8d40-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8d40-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b8d40-176">响应</span><span class="sxs-lookup"><span data-stu-id="b8d40-176">Response</span></span>
<span data-ttu-id="b8d40-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8d40-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

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
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




