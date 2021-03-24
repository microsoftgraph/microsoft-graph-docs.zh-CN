---
title: 更新 macOSSoftwareUpdateAccountSummary
description: 更新 macOSSoftwareUpdateAccountSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2412c54b1576308e7861cd961b211ea9fdc09dd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129725"
---
# <a name="update-macossoftwareupdateaccountsummary"></a><span data-ttu-id="0d883-103">更新 macOSSoftwareUpdateAccountSummary</span><span class="sxs-lookup"><span data-stu-id="0d883-103">Update macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="0d883-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d883-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d883-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d883-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d883-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d883-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d883-107">更新 [macOSSoftwareUpdateAccountSummary 对象](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0d883-107">Update the properties of a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d883-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0d883-108">Prerequisites</span></span>
<span data-ttu-id="0d883-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d883-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d883-111">Permission type</span></span>|<span data-ttu-id="0d883-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d883-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d883-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d883-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d883-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d883-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d883-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d883-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d883-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d883-116">Not supported.</span></span>|
|<span data-ttu-id="0d883-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d883-117">Application</span></span>|<span data-ttu-id="0d883-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d883-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d883-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d883-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="0d883-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d883-120">Request headers</span></span>
|<span data-ttu-id="0d883-121">标头</span><span class="sxs-lookup"><span data-stu-id="0d883-121">Header</span></span>|<span data-ttu-id="0d883-122">值</span><span class="sxs-lookup"><span data-stu-id="0d883-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d883-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d883-123">Authorization</span></span>|<span data-ttu-id="0d883-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0d883-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d883-125">接受</span><span class="sxs-lookup"><span data-stu-id="0d883-125">Accept</span></span>|<span data-ttu-id="0d883-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d883-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d883-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d883-127">Request body</span></span>
<span data-ttu-id="0d883-128">在请求正文中，提供 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d883-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

<span data-ttu-id="0d883-129">下表显示创建 [macOSSoftwareUpdateAccountSummary 时所需的属性](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="0d883-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).</span></span>

|<span data-ttu-id="0d883-130">属性</span><span class="sxs-lookup"><span data-stu-id="0d883-130">Property</span></span>|<span data-ttu-id="0d883-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d883-131">Type</span></span>|<span data-ttu-id="0d883-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d883-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d883-133">id</span><span class="sxs-lookup"><span data-stu-id="0d883-133">id</span></span>|<span data-ttu-id="0d883-134">String</span><span class="sxs-lookup"><span data-stu-id="0d883-134">String</span></span>|<span data-ttu-id="0d883-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0d883-135">Key of the entity.</span></span>|
|<span data-ttu-id="0d883-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0d883-136">displayName</span></span>|<span data-ttu-id="0d883-137">String</span><span class="sxs-lookup"><span data-stu-id="0d883-137">String</span></span>|<span data-ttu-id="0d883-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="0d883-138">The name of the report</span></span>|
|<span data-ttu-id="0d883-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0d883-139">deviceId</span></span>|<span data-ttu-id="0d883-140">String</span><span class="sxs-lookup"><span data-stu-id="0d883-140">String</span></span>|<span data-ttu-id="0d883-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="0d883-141">The device ID.</span></span>|
|<span data-ttu-id="0d883-142">userId</span><span class="sxs-lookup"><span data-stu-id="0d883-142">userId</span></span>|<span data-ttu-id="0d883-143">String</span><span class="sxs-lookup"><span data-stu-id="0d883-143">String</span></span>|<span data-ttu-id="0d883-144">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="0d883-144">The user ID.</span></span>|
|<span data-ttu-id="0d883-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="0d883-145">deviceName</span></span>|<span data-ttu-id="0d883-146">String</span><span class="sxs-lookup"><span data-stu-id="0d883-146">String</span></span>|<span data-ttu-id="0d883-147">设备名称。</span><span class="sxs-lookup"><span data-stu-id="0d883-147">The device name.</span></span>|
|<span data-ttu-id="0d883-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0d883-148">userPrincipalName</span></span>|<span data-ttu-id="0d883-149">String</span><span class="sxs-lookup"><span data-stu-id="0d883-149">String</span></span>|<span data-ttu-id="0d883-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="0d883-150">The user principal name</span></span>|
|<span data-ttu-id="0d883-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="0d883-151">osVersion</span></span>|<span data-ttu-id="0d883-152">String</span><span class="sxs-lookup"><span data-stu-id="0d883-152">String</span></span>|<span data-ttu-id="0d883-153">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0d883-153">The OS version.</span></span>|
|<span data-ttu-id="0d883-154">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="0d883-154">successfulUpdateCount</span></span>|<span data-ttu-id="0d883-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0d883-155">Int32</span></span>|<span data-ttu-id="0d883-156">设备上成功更新的数量。</span><span class="sxs-lookup"><span data-stu-id="0d883-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="0d883-157">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="0d883-157">failedUpdateCount</span></span>|<span data-ttu-id="0d883-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0d883-158">Int32</span></span>|<span data-ttu-id="0d883-159">设备上失败的更新数。</span><span class="sxs-lookup"><span data-stu-id="0d883-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="0d883-160">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="0d883-160">totalUpdateCount</span></span>|<span data-ttu-id="0d883-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0d883-161">Int32</span></span>|<span data-ttu-id="0d883-162">设备上的总更新数。</span><span class="sxs-lookup"><span data-stu-id="0d883-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="0d883-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d883-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="0d883-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d883-164">DateTimeOffset</span></span>|<span data-ttu-id="0d883-165">上次更新此设备的报告的日期时间。</span><span class="sxs-lookup"><span data-stu-id="0d883-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="0d883-166">响应</span><span class="sxs-lookup"><span data-stu-id="0d883-166">Response</span></span>
<span data-ttu-id="0d883-167">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d883-167">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d883-168">示例</span><span class="sxs-lookup"><span data-stu-id="0d883-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d883-169">请求</span><span class="sxs-lookup"><span data-stu-id="0d883-169">Request</span></span>
<span data-ttu-id="0d883-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d883-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d883-171">响应</span><span class="sxs-lookup"><span data-stu-id="0d883-171">Response</span></span>
<span data-ttu-id="0d883-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d883-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




