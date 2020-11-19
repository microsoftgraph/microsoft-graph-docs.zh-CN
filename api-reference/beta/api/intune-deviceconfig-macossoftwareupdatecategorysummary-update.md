---
title: 更新 macOSSoftwareUpdateCategorySummary
description: 更新 macOSSoftwareUpdateCategorySummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69c75261058fa1ebdc60c726d77e093f49ea0b24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236447"
---
# <a name="update-macossoftwareupdatecategorysummary"></a><span data-ttu-id="399ff-103">更新 macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="399ff-103">Update macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="399ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="399ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="399ff-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="399ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="399ff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="399ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="399ff-107">更新 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="399ff-107">Update the properties of a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="399ff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="399ff-108">Prerequisites</span></span>
<span data-ttu-id="399ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="399ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="399ff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="399ff-111">Permission type</span></span>|<span data-ttu-id="399ff-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="399ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="399ff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="399ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="399ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="399ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="399ff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="399ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="399ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="399ff-116">Not supported.</span></span>|
|<span data-ttu-id="399ff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="399ff-117">Application</span></span>|<span data-ttu-id="399ff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="399ff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="399ff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="399ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="399ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="399ff-120">Request headers</span></span>
|<span data-ttu-id="399ff-121">标头</span><span class="sxs-lookup"><span data-stu-id="399ff-121">Header</span></span>|<span data-ttu-id="399ff-122">值</span><span class="sxs-lookup"><span data-stu-id="399ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="399ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="399ff-123">Authorization</span></span>|<span data-ttu-id="399ff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="399ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="399ff-125">接受</span><span class="sxs-lookup"><span data-stu-id="399ff-125">Accept</span></span>|<span data-ttu-id="399ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="399ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="399ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="399ff-127">Request body</span></span>
<span data-ttu-id="399ff-128">在请求正文中，提供 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="399ff-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

<span data-ttu-id="399ff-129">下表显示创建 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="399ff-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).</span></span>

|<span data-ttu-id="399ff-130">属性</span><span class="sxs-lookup"><span data-stu-id="399ff-130">Property</span></span>|<span data-ttu-id="399ff-131">类型</span><span class="sxs-lookup"><span data-stu-id="399ff-131">Type</span></span>|<span data-ttu-id="399ff-132">说明</span><span class="sxs-lookup"><span data-stu-id="399ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="399ff-133">id</span><span class="sxs-lookup"><span data-stu-id="399ff-133">id</span></span>|<span data-ttu-id="399ff-134">String</span><span class="sxs-lookup"><span data-stu-id="399ff-134">String</span></span>|<span data-ttu-id="399ff-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="399ff-135">Key of the entity.</span></span>|
|<span data-ttu-id="399ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="399ff-136">displayName</span></span>|<span data-ttu-id="399ff-137">String</span><span class="sxs-lookup"><span data-stu-id="399ff-137">String</span></span>|<span data-ttu-id="399ff-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="399ff-138">The name of the report</span></span>|
|<span data-ttu-id="399ff-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="399ff-139">deviceId</span></span>|<span data-ttu-id="399ff-140">String</span><span class="sxs-lookup"><span data-stu-id="399ff-140">String</span></span>|<span data-ttu-id="399ff-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="399ff-141">The device ID.</span></span>|
|<span data-ttu-id="399ff-142">userId</span><span class="sxs-lookup"><span data-stu-id="399ff-142">userId</span></span>|<span data-ttu-id="399ff-143">String</span><span class="sxs-lookup"><span data-stu-id="399ff-143">String</span></span>|<span data-ttu-id="399ff-144">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="399ff-144">The user ID.</span></span>|
|<span data-ttu-id="399ff-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="399ff-145">updateCategory</span></span>|[<span data-ttu-id="399ff-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="399ff-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="399ff-147">软件更新类型。</span><span class="sxs-lookup"><span data-stu-id="399ff-147">Software update type.</span></span> <span data-ttu-id="399ff-148">可取值为：`critical`、`configurationDataFile`、`firmware`、`other`。</span><span class="sxs-lookup"><span data-stu-id="399ff-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="399ff-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="399ff-149">successfulUpdateCount</span></span>|<span data-ttu-id="399ff-150">Int32</span><span class="sxs-lookup"><span data-stu-id="399ff-150">Int32</span></span>|<span data-ttu-id="399ff-151">设备上的成功更新数</span><span class="sxs-lookup"><span data-stu-id="399ff-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="399ff-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="399ff-152">failedUpdateCount</span></span>|<span data-ttu-id="399ff-153">Int32</span><span class="sxs-lookup"><span data-stu-id="399ff-153">Int32</span></span>|<span data-ttu-id="399ff-154">设备上的失败更新数</span><span class="sxs-lookup"><span data-stu-id="399ff-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="399ff-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="399ff-155">totalUpdateCount</span></span>|<span data-ttu-id="399ff-156">Int32</span><span class="sxs-lookup"><span data-stu-id="399ff-156">Int32</span></span>|<span data-ttu-id="399ff-157">设备上的总更新数</span><span class="sxs-lookup"><span data-stu-id="399ff-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="399ff-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="399ff-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="399ff-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="399ff-159">DateTimeOffset</span></span>|<span data-ttu-id="399ff-160">最后一次更新此设备的报告的日期。</span><span class="sxs-lookup"><span data-stu-id="399ff-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="399ff-161">响应</span><span class="sxs-lookup"><span data-stu-id="399ff-161">Response</span></span>
<span data-ttu-id="399ff-162">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="399ff-162">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="399ff-163">示例</span><span class="sxs-lookup"><span data-stu-id="399ff-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="399ff-164">请求</span><span class="sxs-lookup"><span data-stu-id="399ff-164">Request</span></span>
<span data-ttu-id="399ff-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="399ff-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
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

### <a name="response"></a><span data-ttu-id="399ff-166">响应</span><span class="sxs-lookup"><span data-stu-id="399ff-166">Response</span></span>
<span data-ttu-id="399ff-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="399ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




