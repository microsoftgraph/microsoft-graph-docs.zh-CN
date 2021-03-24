---
title: 创建 deviceManagementCachedReportConfiguration
description: 创建新的 deviceManagementCachedReportConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9df14360ac503b20eaf881fb37a79c111c8c2c2a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51124601"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="5a772-103">创建 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a772-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="5a772-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a772-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a772-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a772-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a772-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a772-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a772-107">创建新的 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a772-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a772-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a772-108">Prerequisites</span></span>
<span data-ttu-id="5a772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a772-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a772-111">Permission type</span></span>|<span data-ttu-id="5a772-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a772-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a772-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a772-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a772-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a772-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5a772-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a772-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a772-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a772-116">Not supported.</span></span>|
|<span data-ttu-id="5a772-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a772-117">Application</span></span>|<span data-ttu-id="5a772-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a772-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a772-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a772-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a772-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a772-120">Request headers</span></span>
|<span data-ttu-id="5a772-121">标头</span><span class="sxs-lookup"><span data-stu-id="5a772-121">Header</span></span>|<span data-ttu-id="5a772-122">值</span><span class="sxs-lookup"><span data-stu-id="5a772-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a772-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a772-123">Authorization</span></span>|<span data-ttu-id="5a772-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a772-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a772-125">接受</span><span class="sxs-lookup"><span data-stu-id="5a772-125">Accept</span></span>|<span data-ttu-id="5a772-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a772-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a772-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a772-127">Request body</span></span>
<span data-ttu-id="5a772-128">在请求正文中，提供 deviceManagementCachedReportConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a772-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="5a772-129">下表显示创建 deviceManagementCachedReportConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a772-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="5a772-130">属性</span><span class="sxs-lookup"><span data-stu-id="5a772-130">Property</span></span>|<span data-ttu-id="5a772-131">类型</span><span class="sxs-lookup"><span data-stu-id="5a772-131">Type</span></span>|<span data-ttu-id="5a772-132">说明</span><span class="sxs-lookup"><span data-stu-id="5a772-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a772-133">id</span><span class="sxs-lookup"><span data-stu-id="5a772-133">id</span></span>|<span data-ttu-id="5a772-134">String</span><span class="sxs-lookup"><span data-stu-id="5a772-134">String</span></span>|<span data-ttu-id="5a772-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5a772-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="5a772-136">reportName</span><span class="sxs-lookup"><span data-stu-id="5a772-136">reportName</span></span>|<span data-ttu-id="5a772-137">String</span><span class="sxs-lookup"><span data-stu-id="5a772-137">String</span></span>|<span data-ttu-id="5a772-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="5a772-138">Name of the report</span></span>|
|<span data-ttu-id="5a772-139">filter</span><span class="sxs-lookup"><span data-stu-id="5a772-139">filter</span></span>|<span data-ttu-id="5a772-140">String</span><span class="sxs-lookup"><span data-stu-id="5a772-140">String</span></span>|<span data-ttu-id="5a772-141">创建报表时应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="5a772-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="5a772-142">select</span><span class="sxs-lookup"><span data-stu-id="5a772-142">select</span></span>|<span data-ttu-id="5a772-143">String collection</span><span class="sxs-lookup"><span data-stu-id="5a772-143">String collection</span></span>|<span data-ttu-id="5a772-144">从报表选择的列</span><span class="sxs-lookup"><span data-stu-id="5a772-144">Columns selected from the report</span></span>|
|<span data-ttu-id="5a772-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="5a772-145">orderBy</span></span>|<span data-ttu-id="5a772-146">String collection</span><span class="sxs-lookup"><span data-stu-id="5a772-146">String collection</span></span>|<span data-ttu-id="5a772-147">报告中列的排序</span><span class="sxs-lookup"><span data-stu-id="5a772-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="5a772-148">metadata</span><span class="sxs-lookup"><span data-stu-id="5a772-148">metadata</span></span>|<span data-ttu-id="5a772-149">String</span><span class="sxs-lookup"><span data-stu-id="5a772-149">String</span></span>|<span data-ttu-id="5a772-150">与报告关联的呼叫者管理的元数据</span><span class="sxs-lookup"><span data-stu-id="5a772-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="5a772-151">状态</span><span class="sxs-lookup"><span data-stu-id="5a772-151">status</span></span>|[<span data-ttu-id="5a772-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="5a772-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="5a772-153">缓存报表的状态。</span><span class="sxs-lookup"><span data-stu-id="5a772-153">Status of the cached report.</span></span> <span data-ttu-id="5a772-154">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="5a772-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="5a772-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="5a772-155">lastRefreshDateTime</span></span>|<span data-ttu-id="5a772-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a772-156">DateTimeOffset</span></span>|<span data-ttu-id="5a772-157">上次刷新缓存报告的时间</span><span class="sxs-lookup"><span data-stu-id="5a772-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="5a772-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5a772-158">expirationDateTime</span></span>|<span data-ttu-id="5a772-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a772-159">DateTimeOffset</span></span>|<span data-ttu-id="5a772-160">缓存报告的过期时间</span><span class="sxs-lookup"><span data-stu-id="5a772-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="5a772-161">响应</span><span class="sxs-lookup"><span data-stu-id="5a772-161">Response</span></span>
<span data-ttu-id="5a772-162">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a772-162">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a772-163">示例</span><span class="sxs-lookup"><span data-stu-id="5a772-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a772-164">请求</span><span class="sxs-lookup"><span data-stu-id="5a772-164">Request</span></span>
<span data-ttu-id="5a772-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a772-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
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

### <a name="response"></a><span data-ttu-id="5a772-166">响应</span><span class="sxs-lookup"><span data-stu-id="5a772-166">Response</span></span>
<span data-ttu-id="5a772-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a772-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




