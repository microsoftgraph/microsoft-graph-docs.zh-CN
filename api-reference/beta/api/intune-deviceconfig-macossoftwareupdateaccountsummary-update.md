---
title: 更新 macOSSoftwareUpdateAccountSummary
description: 更新 macOSSoftwareUpdateAccountSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29ca1b5e3028abf3fd48e77501b7e02389963240
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731832"
---
# <a name="update-macossoftwareupdateaccountsummary"></a><span data-ttu-id="1e52e-103">更新 macOSSoftwareUpdateAccountSummary</span><span class="sxs-lookup"><span data-stu-id="1e52e-103">Update macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="1e52e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e52e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e52e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e52e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e52e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e52e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e52e-107">更新 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e52e-107">Update the properties of a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e52e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e52e-108">Prerequisites</span></span>
<span data-ttu-id="1e52e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e52e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e52e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e52e-111">Permission type</span></span>|<span data-ttu-id="1e52e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e52e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e52e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e52e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e52e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e52e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e52e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e52e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e52e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e52e-116">Not supported.</span></span>|
|<span data-ttu-id="1e52e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e52e-117">Application</span></span>|<span data-ttu-id="1e52e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e52e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e52e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e52e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1e52e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e52e-120">Request headers</span></span>
|<span data-ttu-id="1e52e-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e52e-121">Header</span></span>|<span data-ttu-id="1e52e-122">值</span><span class="sxs-lookup"><span data-stu-id="1e52e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e52e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e52e-123">Authorization</span></span>|<span data-ttu-id="1e52e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e52e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e52e-125">接受</span><span class="sxs-lookup"><span data-stu-id="1e52e-125">Accept</span></span>|<span data-ttu-id="1e52e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e52e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e52e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e52e-127">Request body</span></span>
<span data-ttu-id="1e52e-128">在请求正文中，提供 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e52e-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

<span data-ttu-id="1e52e-129">下表显示创建 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e52e-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).</span></span>

|<span data-ttu-id="1e52e-130">属性</span><span class="sxs-lookup"><span data-stu-id="1e52e-130">Property</span></span>|<span data-ttu-id="1e52e-131">类型</span><span class="sxs-lookup"><span data-stu-id="1e52e-131">Type</span></span>|<span data-ttu-id="1e52e-132">说明</span><span class="sxs-lookup"><span data-stu-id="1e52e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e52e-133">id</span><span class="sxs-lookup"><span data-stu-id="1e52e-133">id</span></span>|<span data-ttu-id="1e52e-134">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-134">String</span></span>|<span data-ttu-id="1e52e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e52e-135">Key of the entity.</span></span>|
|<span data-ttu-id="1e52e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1e52e-136">displayName</span></span>|<span data-ttu-id="1e52e-137">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-137">String</span></span>|<span data-ttu-id="1e52e-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="1e52e-138">The name of the report</span></span>|
|<span data-ttu-id="1e52e-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="1e52e-139">deviceId</span></span>|<span data-ttu-id="1e52e-140">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-140">String</span></span>|<span data-ttu-id="1e52e-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="1e52e-141">The device ID.</span></span>|
|<span data-ttu-id="1e52e-142">userId</span><span class="sxs-lookup"><span data-stu-id="1e52e-142">userId</span></span>|<span data-ttu-id="1e52e-143">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-143">String</span></span>|<span data-ttu-id="1e52e-144">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="1e52e-144">The user ID.</span></span>|
|<span data-ttu-id="1e52e-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="1e52e-145">deviceName</span></span>|<span data-ttu-id="1e52e-146">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-146">String</span></span>|<span data-ttu-id="1e52e-147">设备名称。</span><span class="sxs-lookup"><span data-stu-id="1e52e-147">The device name.</span></span>|
|<span data-ttu-id="1e52e-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e52e-148">userPrincipalName</span></span>|<span data-ttu-id="1e52e-149">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-149">String</span></span>|<span data-ttu-id="1e52e-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1e52e-150">The user principal name</span></span>|
|<span data-ttu-id="1e52e-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="1e52e-151">osVersion</span></span>|<span data-ttu-id="1e52e-152">String</span><span class="sxs-lookup"><span data-stu-id="1e52e-152">String</span></span>|<span data-ttu-id="1e52e-153">OS 版本。</span><span class="sxs-lookup"><span data-stu-id="1e52e-153">The OS version.</span></span>|
|<span data-ttu-id="1e52e-154">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="1e52e-154">successfulUpdateCount</span></span>|<span data-ttu-id="1e52e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1e52e-155">Int32</span></span>|<span data-ttu-id="1e52e-156">设备上的成功更新数。</span><span class="sxs-lookup"><span data-stu-id="1e52e-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="1e52e-157">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="1e52e-157">failedUpdateCount</span></span>|<span data-ttu-id="1e52e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1e52e-158">Int32</span></span>|<span data-ttu-id="1e52e-159">设备上的失败更新数。</span><span class="sxs-lookup"><span data-stu-id="1e52e-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="1e52e-160">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="1e52e-160">totalUpdateCount</span></span>|<span data-ttu-id="1e52e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1e52e-161">Int32</span></span>|<span data-ttu-id="1e52e-162">设备上的总更新数。</span><span class="sxs-lookup"><span data-stu-id="1e52e-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="1e52e-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e52e-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="1e52e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e52e-164">DateTimeOffset</span></span>|<span data-ttu-id="1e52e-165">最后一次更新此设备的报告的日期。</span><span class="sxs-lookup"><span data-stu-id="1e52e-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="1e52e-166">响应</span><span class="sxs-lookup"><span data-stu-id="1e52e-166">Response</span></span>
<span data-ttu-id="1e52e-167">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e52e-167">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e52e-168">示例</span><span class="sxs-lookup"><span data-stu-id="1e52e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e52e-169">请求</span><span class="sxs-lookup"><span data-stu-id="1e52e-169">Request</span></span>
<span data-ttu-id="1e52e-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e52e-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1e52e-171">响应</span><span class="sxs-lookup"><span data-stu-id="1e52e-171">Response</span></span>
<span data-ttu-id="1e52e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e52e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "64687d05-7d05-6468-057d-6864057d6864",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```





