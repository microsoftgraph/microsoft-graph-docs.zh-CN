---
title: 更新 deviceManagementCachedReportConfiguration
description: 更新 deviceManagementCachedReportConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f4ea7ad8e14331cd7d9b322cf977f59ff452efc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801444"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="84781-103">更新 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84781-103">Update deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="84781-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84781-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84781-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84781-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84781-106">更新[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84781-106">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84781-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="84781-107">Prerequisites</span></span>
<span data-ttu-id="84781-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84781-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84781-110">Permission type</span></span>|<span data-ttu-id="84781-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84781-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84781-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84781-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84781-113">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="84781-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84781-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84781-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84781-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84781-115">Not supported.</span></span>|
|<span data-ttu-id="84781-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84781-116">Application</span></span>|<span data-ttu-id="84781-117">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="84781-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84781-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84781-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="84781-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84781-119">Request headers</span></span>
|<span data-ttu-id="84781-120">标头</span><span class="sxs-lookup"><span data-stu-id="84781-120">Header</span></span>|<span data-ttu-id="84781-121">值</span><span class="sxs-lookup"><span data-stu-id="84781-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84781-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84781-122">Authorization</span></span>|<span data-ttu-id="84781-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84781-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84781-124">接受</span><span class="sxs-lookup"><span data-stu-id="84781-124">Accept</span></span>|<span data-ttu-id="84781-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84781-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84781-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="84781-126">Request body</span></span>
<span data-ttu-id="84781-127">在请求正文中，提供[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84781-127">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="84781-128">下表显示创建[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84781-128">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="84781-129">属性</span><span class="sxs-lookup"><span data-stu-id="84781-129">Property</span></span>|<span data-ttu-id="84781-130">类型</span><span class="sxs-lookup"><span data-stu-id="84781-130">Type</span></span>|<span data-ttu-id="84781-131">说明</span><span class="sxs-lookup"><span data-stu-id="84781-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84781-132">id</span><span class="sxs-lookup"><span data-stu-id="84781-132">id</span></span>|<span data-ttu-id="84781-133">String</span><span class="sxs-lookup"><span data-stu-id="84781-133">String</span></span>|<span data-ttu-id="84781-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="84781-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="84781-135">reportName</span><span class="sxs-lookup"><span data-stu-id="84781-135">reportName</span></span>|<span data-ttu-id="84781-136">String</span><span class="sxs-lookup"><span data-stu-id="84781-136">String</span></span>|<span data-ttu-id="84781-137">报告的名称</span><span class="sxs-lookup"><span data-stu-id="84781-137">Name of the report</span></span>|
|<span data-ttu-id="84781-138">filter</span><span class="sxs-lookup"><span data-stu-id="84781-138">filter</span></span>|<span data-ttu-id="84781-139">String</span><span class="sxs-lookup"><span data-stu-id="84781-139">String</span></span>|<span data-ttu-id="84781-140">在创建报表时应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="84781-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="84781-141">select</span><span class="sxs-lookup"><span data-stu-id="84781-141">select</span></span>|<span data-ttu-id="84781-142">String collection</span><span class="sxs-lookup"><span data-stu-id="84781-142">String collection</span></span>|<span data-ttu-id="84781-143">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="84781-143">Columns selected from the report</span></span>|
|<span data-ttu-id="84781-144">By</span><span class="sxs-lookup"><span data-stu-id="84781-144">orderBy</span></span>|<span data-ttu-id="84781-145">String collection</span><span class="sxs-lookup"><span data-stu-id="84781-145">String collection</span></span>|<span data-ttu-id="84781-146">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="84781-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="84781-147">状态</span><span class="sxs-lookup"><span data-stu-id="84781-147">status</span></span>|[<span data-ttu-id="84781-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="84781-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="84781-149">缓存报告的状态。</span><span class="sxs-lookup"><span data-stu-id="84781-149">Status of the cached report.</span></span> <span data-ttu-id="84781-150">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="84781-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="84781-151">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="84781-151">lastRefreshDateTime</span></span>|<span data-ttu-id="84781-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84781-152">DateTimeOffset</span></span>|<span data-ttu-id="84781-153">上次刷新缓存的报告的时间</span><span class="sxs-lookup"><span data-stu-id="84781-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="84781-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84781-154">expirationDateTime</span></span>|<span data-ttu-id="84781-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84781-155">DateTimeOffset</span></span>|<span data-ttu-id="84781-156">缓存的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="84781-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="84781-157">响应</span><span class="sxs-lookup"><span data-stu-id="84781-157">Response</span></span>
<span data-ttu-id="84781-158">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84781-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84781-159">示例</span><span class="sxs-lookup"><span data-stu-id="84781-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="84781-160">请求</span><span class="sxs-lookup"><span data-stu-id="84781-160">Request</span></span>
<span data-ttu-id="84781-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84781-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
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

### <a name="response"></a><span data-ttu-id="84781-162">响应</span><span class="sxs-lookup"><span data-stu-id="84781-162">Response</span></span>
<span data-ttu-id="84781-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84781-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




