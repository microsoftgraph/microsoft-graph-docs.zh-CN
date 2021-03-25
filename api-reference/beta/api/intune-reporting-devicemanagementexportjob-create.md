---
title: 创建 deviceManagementExportJob
description: 创建新的 deviceManagementExportJob 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a126023796b92d8158d7875913efff9be6cf9695
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158456"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="7efcf-103">创建 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="7efcf-103">Create deviceManagementExportJob</span></span>

<span data-ttu-id="7efcf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7efcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7efcf-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7efcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7efcf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7efcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7efcf-107">创建新的 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7efcf-107">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7efcf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7efcf-108">Prerequisites</span></span>
<span data-ttu-id="7efcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7efcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7efcf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7efcf-111">Permission type</span></span>|<span data-ttu-id="7efcf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7efcf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7efcf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7efcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7efcf-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7efcf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7efcf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7efcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7efcf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7efcf-116">Not supported.</span></span>|
|<span data-ttu-id="7efcf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7efcf-117">Application</span></span>|<span data-ttu-id="7efcf-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7efcf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7efcf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7efcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="7efcf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7efcf-120">Request headers</span></span>
|<span data-ttu-id="7efcf-121">标头</span><span class="sxs-lookup"><span data-stu-id="7efcf-121">Header</span></span>|<span data-ttu-id="7efcf-122">值</span><span class="sxs-lookup"><span data-stu-id="7efcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7efcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7efcf-123">Authorization</span></span>|<span data-ttu-id="7efcf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7efcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7efcf-125">接受</span><span class="sxs-lookup"><span data-stu-id="7efcf-125">Accept</span></span>|<span data-ttu-id="7efcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7efcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7efcf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7efcf-127">Request body</span></span>
<span data-ttu-id="7efcf-128">在请求正文中，提供 deviceManagementExportJob 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7efcf-128">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="7efcf-129">下表显示创建 deviceManagementExportJob 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7efcf-129">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="7efcf-130">属性</span><span class="sxs-lookup"><span data-stu-id="7efcf-130">Property</span></span>|<span data-ttu-id="7efcf-131">类型</span><span class="sxs-lookup"><span data-stu-id="7efcf-131">Type</span></span>|<span data-ttu-id="7efcf-132">说明</span><span class="sxs-lookup"><span data-stu-id="7efcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7efcf-133">id</span><span class="sxs-lookup"><span data-stu-id="7efcf-133">id</span></span>|<span data-ttu-id="7efcf-134">String</span><span class="sxs-lookup"><span data-stu-id="7efcf-134">String</span></span>|<span data-ttu-id="7efcf-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7efcf-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="7efcf-136">reportName</span><span class="sxs-lookup"><span data-stu-id="7efcf-136">reportName</span></span>|<span data-ttu-id="7efcf-137">String</span><span class="sxs-lookup"><span data-stu-id="7efcf-137">String</span></span>|<span data-ttu-id="7efcf-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="7efcf-138">Name of the report</span></span>|
|<span data-ttu-id="7efcf-139">filter</span><span class="sxs-lookup"><span data-stu-id="7efcf-139">filter</span></span>|<span data-ttu-id="7efcf-140">String</span><span class="sxs-lookup"><span data-stu-id="7efcf-140">String</span></span>|<span data-ttu-id="7efcf-141">应用于报表的筛选器</span><span class="sxs-lookup"><span data-stu-id="7efcf-141">Filters applied on the report</span></span>|
|<span data-ttu-id="7efcf-142">select</span><span class="sxs-lookup"><span data-stu-id="7efcf-142">select</span></span>|<span data-ttu-id="7efcf-143">String collection</span><span class="sxs-lookup"><span data-stu-id="7efcf-143">String collection</span></span>|<span data-ttu-id="7efcf-144">从报表选择的列</span><span class="sxs-lookup"><span data-stu-id="7efcf-144">Columns selected from the report</span></span>|
|<span data-ttu-id="7efcf-145">format</span><span class="sxs-lookup"><span data-stu-id="7efcf-145">format</span></span>|[<span data-ttu-id="7efcf-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="7efcf-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="7efcf-147">导出的报告的格式。</span><span class="sxs-lookup"><span data-stu-id="7efcf-147">Format of the exported report.</span></span> <span data-ttu-id="7efcf-148">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="7efcf-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="7efcf-149">snapshotId</span><span class="sxs-lookup"><span data-stu-id="7efcf-149">snapshotId</span></span>|<span data-ttu-id="7efcf-150">String</span><span class="sxs-lookup"><span data-stu-id="7efcf-150">String</span></span>|<span data-ttu-id="7efcf-151">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="7efcf-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="7efcf-152">可以在此处使用 sessionId 或 CachedReportConfiguration ID。</span><span class="sxs-lookup"><span data-stu-id="7efcf-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="7efcf-153">如果指定了 sessionId，则 Filter、Select 和 OrderBy 将应用于 sessionId 表示的数据。</span><span class="sxs-lookup"><span data-stu-id="7efcf-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="7efcf-154">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="7efcf-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="7efcf-155">localizationType</span><span class="sxs-lookup"><span data-stu-id="7efcf-155">localizationType</span></span>|[<span data-ttu-id="7efcf-156">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="7efcf-156">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="7efcf-157">配置所请求的导出作业的本地化方式。</span><span class="sxs-lookup"><span data-stu-id="7efcf-157">Configures how the requested export job is localized.</span></span> <span data-ttu-id="7efcf-158">可取值为：`localizedValuesAsAdditionalColumn`、`replaceLocalizableValues`。</span><span class="sxs-lookup"><span data-stu-id="7efcf-158">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="7efcf-159">状态</span><span class="sxs-lookup"><span data-stu-id="7efcf-159">status</span></span>|[<span data-ttu-id="7efcf-160">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="7efcf-160">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="7efcf-161">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="7efcf-161">Status of the export job.</span></span> <span data-ttu-id="7efcf-162">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="7efcf-162">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="7efcf-163">url</span><span class="sxs-lookup"><span data-stu-id="7efcf-163">url</span></span>|<span data-ttu-id="7efcf-164">String</span><span class="sxs-lookup"><span data-stu-id="7efcf-164">String</span></span>|<span data-ttu-id="7efcf-165">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="7efcf-165">Temporary location of the exported report</span></span>|
|<span data-ttu-id="7efcf-166">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="7efcf-166">requestDateTime</span></span>|<span data-ttu-id="7efcf-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7efcf-167">DateTimeOffset</span></span>|<span data-ttu-id="7efcf-168">请求导出报告的时间</span><span class="sxs-lookup"><span data-stu-id="7efcf-168">Time that the exported report was requested</span></span>|
|<span data-ttu-id="7efcf-169">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7efcf-169">expirationDateTime</span></span>|<span data-ttu-id="7efcf-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7efcf-170">DateTimeOffset</span></span>|<span data-ttu-id="7efcf-171">导出报告的过期时间</span><span class="sxs-lookup"><span data-stu-id="7efcf-171">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="7efcf-172">响应</span><span class="sxs-lookup"><span data-stu-id="7efcf-172">Response</span></span>
<span data-ttu-id="7efcf-173">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7efcf-173">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7efcf-174">示例</span><span class="sxs-lookup"><span data-stu-id="7efcf-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="7efcf-175">请求</span><span class="sxs-lookup"><span data-stu-id="7efcf-175">Request</span></span>
<span data-ttu-id="7efcf-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7efcf-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="7efcf-177">响应</span><span class="sxs-lookup"><span data-stu-id="7efcf-177">Response</span></span>
<span data-ttu-id="7efcf-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7efcf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




