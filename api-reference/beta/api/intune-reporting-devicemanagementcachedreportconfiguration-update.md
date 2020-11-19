---
title: 更新 deviceManagementCachedReportConfiguration
description: 更新 deviceManagementCachedReportConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdfa2512972323cb62672c6f639a95a77cc25e0e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307995"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="7967a-103">更新 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="7967a-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="7967a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7967a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7967a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7967a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7967a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7967a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7967a-107">更新 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7967a-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7967a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7967a-108">Prerequisites</span></span>
<span data-ttu-id="7967a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7967a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7967a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7967a-111">Permission type</span></span>|<span data-ttu-id="7967a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7967a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7967a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7967a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7967a-114">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="7967a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7967a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7967a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7967a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7967a-116">Not supported.</span></span>|
|<span data-ttu-id="7967a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7967a-117">Application</span></span>|<span data-ttu-id="7967a-118">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="7967a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7967a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7967a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7967a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7967a-120">Request headers</span></span>
|<span data-ttu-id="7967a-121">标头</span><span class="sxs-lookup"><span data-stu-id="7967a-121">Header</span></span>|<span data-ttu-id="7967a-122">值</span><span class="sxs-lookup"><span data-stu-id="7967a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7967a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7967a-123">Authorization</span></span>|<span data-ttu-id="7967a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7967a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7967a-125">接受</span><span class="sxs-lookup"><span data-stu-id="7967a-125">Accept</span></span>|<span data-ttu-id="7967a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7967a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7967a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7967a-127">Request body</span></span>
<span data-ttu-id="7967a-128">在请求正文中，提供 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7967a-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="7967a-129">下表显示创建 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7967a-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="7967a-130">属性</span><span class="sxs-lookup"><span data-stu-id="7967a-130">Property</span></span>|<span data-ttu-id="7967a-131">类型</span><span class="sxs-lookup"><span data-stu-id="7967a-131">Type</span></span>|<span data-ttu-id="7967a-132">说明</span><span class="sxs-lookup"><span data-stu-id="7967a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7967a-133">id</span><span class="sxs-lookup"><span data-stu-id="7967a-133">id</span></span>|<span data-ttu-id="7967a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7967a-134">String</span></span>|<span data-ttu-id="7967a-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7967a-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="7967a-136">reportName</span><span class="sxs-lookup"><span data-stu-id="7967a-136">reportName</span></span>|<span data-ttu-id="7967a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7967a-137">String</span></span>|<span data-ttu-id="7967a-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="7967a-138">Name of the report</span></span>|
|<span data-ttu-id="7967a-139">filter</span><span class="sxs-lookup"><span data-stu-id="7967a-139">filter</span></span>|<span data-ttu-id="7967a-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7967a-140">String</span></span>|<span data-ttu-id="7967a-141">在创建报表时应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="7967a-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="7967a-142">select</span><span class="sxs-lookup"><span data-stu-id="7967a-142">select</span></span>|<span data-ttu-id="7967a-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="7967a-143">String collection</span></span>|<span data-ttu-id="7967a-144">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="7967a-144">Columns selected from the report</span></span>|
|<span data-ttu-id="7967a-145">By</span><span class="sxs-lookup"><span data-stu-id="7967a-145">orderBy</span></span>|<span data-ttu-id="7967a-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="7967a-146">String collection</span></span>|<span data-ttu-id="7967a-147">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="7967a-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="7967a-148">metadata</span><span class="sxs-lookup"><span data-stu-id="7967a-148">metadata</span></span>|<span data-ttu-id="7967a-149">字符串</span><span class="sxs-lookup"><span data-stu-id="7967a-149">String</span></span>|<span data-ttu-id="7967a-150">与报告关联的调用方托管元数据</span><span class="sxs-lookup"><span data-stu-id="7967a-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="7967a-151">status</span><span class="sxs-lookup"><span data-stu-id="7967a-151">status</span></span>|[<span data-ttu-id="7967a-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="7967a-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="7967a-153">缓存报告的状态。</span><span class="sxs-lookup"><span data-stu-id="7967a-153">Status of the cached report.</span></span> <span data-ttu-id="7967a-154">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="7967a-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="7967a-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="7967a-155">lastRefreshDateTime</span></span>|<span data-ttu-id="7967a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7967a-156">DateTimeOffset</span></span>|<span data-ttu-id="7967a-157">上次刷新缓存的报告的时间</span><span class="sxs-lookup"><span data-stu-id="7967a-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="7967a-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7967a-158">expirationDateTime</span></span>|<span data-ttu-id="7967a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7967a-159">DateTimeOffset</span></span>|<span data-ttu-id="7967a-160">缓存的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="7967a-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="7967a-161">响应</span><span class="sxs-lookup"><span data-stu-id="7967a-161">Response</span></span>
<span data-ttu-id="7967a-162">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7967a-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7967a-163">示例</span><span class="sxs-lookup"><span data-stu-id="7967a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="7967a-164">请求</span><span class="sxs-lookup"><span data-stu-id="7967a-164">Request</span></span>
<span data-ttu-id="7967a-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7967a-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
Content-type: application/json
Content-length: 418

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
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="7967a-166">响应</span><span class="sxs-lookup"><span data-stu-id="7967a-166">Response</span></span>
<span data-ttu-id="7967a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7967a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

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
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




