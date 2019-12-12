---
title: 创建 deviceManagementCachedReportConfiguration
description: 创建新的 deviceManagementCachedReportConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 240ca89d363f60eff21cc1d299b5b96c5523cbbc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955075"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="8ee25-103">创建 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ee25-103">Create deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="8ee25-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ee25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ee25-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ee25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ee25-106">创建新的[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8ee25-106">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ee25-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ee25-107">Prerequisites</span></span>
<span data-ttu-id="8ee25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ee25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee25-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ee25-110">Permission type</span></span>|<span data-ttu-id="8ee25-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8ee25-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ee25-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ee25-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ee25-113">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="8ee25-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ee25-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ee25-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ee25-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ee25-115">Not supported.</span></span>|
|<span data-ttu-id="8ee25-116">Application</span><span class="sxs-lookup"><span data-stu-id="8ee25-116">Application</span></span>|<span data-ttu-id="8ee25-117">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="8ee25-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ee25-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ee25-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ee25-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ee25-119">Request headers</span></span>
|<span data-ttu-id="8ee25-120">标头</span><span class="sxs-lookup"><span data-stu-id="8ee25-120">Header</span></span>|<span data-ttu-id="8ee25-121">值</span><span class="sxs-lookup"><span data-stu-id="8ee25-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ee25-122">授权</span><span class="sxs-lookup"><span data-stu-id="8ee25-122">Authorization</span></span>|<span data-ttu-id="8ee25-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ee25-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ee25-124">接受</span><span class="sxs-lookup"><span data-stu-id="8ee25-124">Accept</span></span>|<span data-ttu-id="8ee25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ee25-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee25-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ee25-126">Request body</span></span>
<span data-ttu-id="8ee25-127">在请求正文中，提供 deviceManagementCachedReportConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ee25-127">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="8ee25-128">下表显示创建 deviceManagementCachedReportConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ee25-128">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="8ee25-129">属性</span><span class="sxs-lookup"><span data-stu-id="8ee25-129">Property</span></span>|<span data-ttu-id="8ee25-130">类型</span><span class="sxs-lookup"><span data-stu-id="8ee25-130">Type</span></span>|<span data-ttu-id="8ee25-131">说明</span><span class="sxs-lookup"><span data-stu-id="8ee25-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ee25-132">id</span><span class="sxs-lookup"><span data-stu-id="8ee25-132">id</span></span>|<span data-ttu-id="8ee25-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8ee25-133">String</span></span>|<span data-ttu-id="8ee25-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8ee25-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="8ee25-135">reportName</span><span class="sxs-lookup"><span data-stu-id="8ee25-135">reportName</span></span>|<span data-ttu-id="8ee25-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8ee25-136">String</span></span>|<span data-ttu-id="8ee25-137">报告的名称</span><span class="sxs-lookup"><span data-stu-id="8ee25-137">Name of the report</span></span>|
|<span data-ttu-id="8ee25-138">filter</span><span class="sxs-lookup"><span data-stu-id="8ee25-138">filter</span></span>|<span data-ttu-id="8ee25-139">字符串</span><span class="sxs-lookup"><span data-stu-id="8ee25-139">String</span></span>|<span data-ttu-id="8ee25-140">在创建报表时应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="8ee25-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="8ee25-141">select</span><span class="sxs-lookup"><span data-stu-id="8ee25-141">select</span></span>|<span data-ttu-id="8ee25-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8ee25-142">String collection</span></span>|<span data-ttu-id="8ee25-143">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="8ee25-143">Columns selected from the report</span></span>|
|<span data-ttu-id="8ee25-144">By</span><span class="sxs-lookup"><span data-stu-id="8ee25-144">orderBy</span></span>|<span data-ttu-id="8ee25-145">String collection</span><span class="sxs-lookup"><span data-stu-id="8ee25-145">String collection</span></span>|<span data-ttu-id="8ee25-146">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="8ee25-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="8ee25-147">状态</span><span class="sxs-lookup"><span data-stu-id="8ee25-147">status</span></span>|[<span data-ttu-id="8ee25-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="8ee25-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="8ee25-149">缓存报告的状态。</span><span class="sxs-lookup"><span data-stu-id="8ee25-149">Status of the cached report.</span></span> <span data-ttu-id="8ee25-150">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="8ee25-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="8ee25-151">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee25-151">lastRefreshDateTime</span></span>|<span data-ttu-id="8ee25-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee25-152">DateTimeOffset</span></span>|<span data-ttu-id="8ee25-153">上次刷新缓存的报告的时间</span><span class="sxs-lookup"><span data-stu-id="8ee25-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="8ee25-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee25-154">expirationDateTime</span></span>|<span data-ttu-id="8ee25-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee25-155">DateTimeOffset</span></span>|<span data-ttu-id="8ee25-156">缓存的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="8ee25-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="8ee25-157">响应</span><span class="sxs-lookup"><span data-stu-id="8ee25-157">Response</span></span>
<span data-ttu-id="8ee25-158">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8ee25-158">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee25-159">示例</span><span class="sxs-lookup"><span data-stu-id="8ee25-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ee25-160">请求</span><span class="sxs-lookup"><span data-stu-id="8ee25-160">Request</span></span>
<span data-ttu-id="8ee25-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ee25-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8ee25-162">响应</span><span class="sxs-lookup"><span data-stu-id="8ee25-162">Response</span></span>
<span data-ttu-id="8ee25-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ee25-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "46947722-7722-4694-2277-944622779446",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```





