---
title: 创建 macOSSoftwareUpdateCategorySummary
description: 创建新的 macOSSoftwareUpdateCategorySummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc47fac234f046d69235af431db9d75dc1093e40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129711"
---
# <a name="create-macossoftwareupdatecategorysummary"></a><span data-ttu-id="c272d-103">创建 macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="c272d-103">Create macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="c272d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c272d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c272d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c272d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c272d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c272d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c272d-107">创建新的 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c272d-107">Create a new [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c272d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c272d-108">Prerequisites</span></span>
<span data-ttu-id="c272d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c272d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c272d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c272d-111">Permission type</span></span>|<span data-ttu-id="c272d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c272d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c272d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c272d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c272d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c272d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c272d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c272d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c272d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c272d-116">Not supported.</span></span>|
|<span data-ttu-id="c272d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c272d-117">Application</span></span>|<span data-ttu-id="c272d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c272d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c272d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c272d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a><span data-ttu-id="c272d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c272d-120">Request headers</span></span>
|<span data-ttu-id="c272d-121">标头</span><span class="sxs-lookup"><span data-stu-id="c272d-121">Header</span></span>|<span data-ttu-id="c272d-122">值</span><span class="sxs-lookup"><span data-stu-id="c272d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c272d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c272d-123">Authorization</span></span>|<span data-ttu-id="c272d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c272d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c272d-125">接受</span><span class="sxs-lookup"><span data-stu-id="c272d-125">Accept</span></span>|<span data-ttu-id="c272d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c272d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c272d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c272d-127">Request body</span></span>
<span data-ttu-id="c272d-128">在请求正文中，提供 macOSSoftwareUpdateCategorySummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c272d-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateCategorySummary object.</span></span>

<span data-ttu-id="c272d-129">下表显示创建 macOSSoftwareUpdateCategorySummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c272d-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateCategorySummary.</span></span>

|<span data-ttu-id="c272d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c272d-130">Property</span></span>|<span data-ttu-id="c272d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c272d-131">Type</span></span>|<span data-ttu-id="c272d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c272d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c272d-133">id</span><span class="sxs-lookup"><span data-stu-id="c272d-133">id</span></span>|<span data-ttu-id="c272d-134">String</span><span class="sxs-lookup"><span data-stu-id="c272d-134">String</span></span>|<span data-ttu-id="c272d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c272d-135">Key of the entity.</span></span>|
|<span data-ttu-id="c272d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c272d-136">displayName</span></span>|<span data-ttu-id="c272d-137">String</span><span class="sxs-lookup"><span data-stu-id="c272d-137">String</span></span>|<span data-ttu-id="c272d-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="c272d-138">The name of the report</span></span>|
|<span data-ttu-id="c272d-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="c272d-139">deviceId</span></span>|<span data-ttu-id="c272d-140">String</span><span class="sxs-lookup"><span data-stu-id="c272d-140">String</span></span>|<span data-ttu-id="c272d-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="c272d-141">The device ID.</span></span>|
|<span data-ttu-id="c272d-142">userId</span><span class="sxs-lookup"><span data-stu-id="c272d-142">userId</span></span>|<span data-ttu-id="c272d-143">String</span><span class="sxs-lookup"><span data-stu-id="c272d-143">String</span></span>|<span data-ttu-id="c272d-144">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="c272d-144">The user ID.</span></span>|
|<span data-ttu-id="c272d-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="c272d-145">updateCategory</span></span>|[<span data-ttu-id="c272d-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="c272d-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="c272d-147">软件更新类型。</span><span class="sxs-lookup"><span data-stu-id="c272d-147">Software update type.</span></span> <span data-ttu-id="c272d-148">可取值为：`critical`、`configurationDataFile`、`firmware`、`other`。</span><span class="sxs-lookup"><span data-stu-id="c272d-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="c272d-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="c272d-149">successfulUpdateCount</span></span>|<span data-ttu-id="c272d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c272d-150">Int32</span></span>|<span data-ttu-id="c272d-151">设备上成功更新的数量</span><span class="sxs-lookup"><span data-stu-id="c272d-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="c272d-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="c272d-152">failedUpdateCount</span></span>|<span data-ttu-id="c272d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c272d-153">Int32</span></span>|<span data-ttu-id="c272d-154">设备上失败的更新数</span><span class="sxs-lookup"><span data-stu-id="c272d-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="c272d-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="c272d-155">totalUpdateCount</span></span>|<span data-ttu-id="c272d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c272d-156">Int32</span></span>|<span data-ttu-id="c272d-157">设备上的总更新数</span><span class="sxs-lookup"><span data-stu-id="c272d-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="c272d-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c272d-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="c272d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c272d-159">DateTimeOffset</span></span>|<span data-ttu-id="c272d-160">上次更新此设备的报告的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c272d-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="c272d-161">响应</span><span class="sxs-lookup"><span data-stu-id="c272d-161">Response</span></span>
<span data-ttu-id="c272d-162">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c272d-162">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c272d-163">示例</span><span class="sxs-lookup"><span data-stu-id="c272d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="c272d-164">请求</span><span class="sxs-lookup"><span data-stu-id="c272d-164">Request</span></span>
<span data-ttu-id="c272d-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c272d-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c272d-166">响应</span><span class="sxs-lookup"><span data-stu-id="c272d-166">Response</span></span>
<span data-ttu-id="c272d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c272d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 422

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




