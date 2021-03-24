---
title: 创建 macOSSoftwareUpdateAccountSummary
description: 创建新的 macOSSoftwareUpdateAccountSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a34b35952ee240784a4b4f28705fe49354024cb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129753"
---
# <a name="create-macossoftwareupdateaccountsummary"></a><span data-ttu-id="56216-103">创建 macOSSoftwareUpdateAccountSummary</span><span class="sxs-lookup"><span data-stu-id="56216-103">Create macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="56216-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56216-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56216-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56216-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56216-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56216-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56216-107">创建新的 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56216-107">Create a new [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56216-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="56216-108">Prerequisites</span></span>
<span data-ttu-id="56216-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56216-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="56216-111">Permission type</span></span>|<span data-ttu-id="56216-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56216-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56216-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56216-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56216-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56216-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56216-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56216-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56216-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56216-116">Not supported.</span></span>|
|<span data-ttu-id="56216-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="56216-117">Application</span></span>|<span data-ttu-id="56216-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56216-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56216-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56216-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries
```

## <a name="request-headers"></a><span data-ttu-id="56216-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="56216-120">Request headers</span></span>
|<span data-ttu-id="56216-121">标头</span><span class="sxs-lookup"><span data-stu-id="56216-121">Header</span></span>|<span data-ttu-id="56216-122">值</span><span class="sxs-lookup"><span data-stu-id="56216-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56216-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56216-123">Authorization</span></span>|<span data-ttu-id="56216-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56216-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56216-125">接受</span><span class="sxs-lookup"><span data-stu-id="56216-125">Accept</span></span>|<span data-ttu-id="56216-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56216-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56216-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="56216-127">Request body</span></span>
<span data-ttu-id="56216-128">在请求正文中，提供 macOSSoftwareUpdateAccountSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56216-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateAccountSummary object.</span></span>

<span data-ttu-id="56216-129">下表显示创建 macOSSoftwareUpdateAccountSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="56216-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateAccountSummary.</span></span>

|<span data-ttu-id="56216-130">属性</span><span class="sxs-lookup"><span data-stu-id="56216-130">Property</span></span>|<span data-ttu-id="56216-131">类型</span><span class="sxs-lookup"><span data-stu-id="56216-131">Type</span></span>|<span data-ttu-id="56216-132">说明</span><span class="sxs-lookup"><span data-stu-id="56216-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56216-133">id</span><span class="sxs-lookup"><span data-stu-id="56216-133">id</span></span>|<span data-ttu-id="56216-134">String</span><span class="sxs-lookup"><span data-stu-id="56216-134">String</span></span>|<span data-ttu-id="56216-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56216-135">Key of the entity.</span></span>|
|<span data-ttu-id="56216-136">displayName</span><span class="sxs-lookup"><span data-stu-id="56216-136">displayName</span></span>|<span data-ttu-id="56216-137">String</span><span class="sxs-lookup"><span data-stu-id="56216-137">String</span></span>|<span data-ttu-id="56216-138">报告的名称</span><span class="sxs-lookup"><span data-stu-id="56216-138">The name of the report</span></span>|
|<span data-ttu-id="56216-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="56216-139">deviceId</span></span>|<span data-ttu-id="56216-140">String</span><span class="sxs-lookup"><span data-stu-id="56216-140">String</span></span>|<span data-ttu-id="56216-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="56216-141">The device ID.</span></span>|
|<span data-ttu-id="56216-142">userId</span><span class="sxs-lookup"><span data-stu-id="56216-142">userId</span></span>|<span data-ttu-id="56216-143">String</span><span class="sxs-lookup"><span data-stu-id="56216-143">String</span></span>|<span data-ttu-id="56216-144">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="56216-144">The user ID.</span></span>|
|<span data-ttu-id="56216-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="56216-145">deviceName</span></span>|<span data-ttu-id="56216-146">String</span><span class="sxs-lookup"><span data-stu-id="56216-146">String</span></span>|<span data-ttu-id="56216-147">设备名称。</span><span class="sxs-lookup"><span data-stu-id="56216-147">The device name.</span></span>|
|<span data-ttu-id="56216-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="56216-148">userPrincipalName</span></span>|<span data-ttu-id="56216-149">String</span><span class="sxs-lookup"><span data-stu-id="56216-149">String</span></span>|<span data-ttu-id="56216-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="56216-150">The user principal name</span></span>|
|<span data-ttu-id="56216-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="56216-151">osVersion</span></span>|<span data-ttu-id="56216-152">String</span><span class="sxs-lookup"><span data-stu-id="56216-152">String</span></span>|<span data-ttu-id="56216-153">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="56216-153">The OS version.</span></span>|
|<span data-ttu-id="56216-154">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="56216-154">successfulUpdateCount</span></span>|<span data-ttu-id="56216-155">Int32</span><span class="sxs-lookup"><span data-stu-id="56216-155">Int32</span></span>|<span data-ttu-id="56216-156">设备上成功更新的数量。</span><span class="sxs-lookup"><span data-stu-id="56216-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="56216-157">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="56216-157">failedUpdateCount</span></span>|<span data-ttu-id="56216-158">Int32</span><span class="sxs-lookup"><span data-stu-id="56216-158">Int32</span></span>|<span data-ttu-id="56216-159">设备上失败的更新数。</span><span class="sxs-lookup"><span data-stu-id="56216-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="56216-160">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="56216-160">totalUpdateCount</span></span>|<span data-ttu-id="56216-161">Int32</span><span class="sxs-lookup"><span data-stu-id="56216-161">Int32</span></span>|<span data-ttu-id="56216-162">设备上的总更新数。</span><span class="sxs-lookup"><span data-stu-id="56216-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="56216-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="56216-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="56216-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56216-164">DateTimeOffset</span></span>|<span data-ttu-id="56216-165">上次更新此设备的报告的日期时间。</span><span class="sxs-lookup"><span data-stu-id="56216-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="56216-166">响应</span><span class="sxs-lookup"><span data-stu-id="56216-166">Response</span></span>
<span data-ttu-id="56216-167">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56216-167">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56216-168">示例</span><span class="sxs-lookup"><span data-stu-id="56216-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="56216-169">请求</span><span class="sxs-lookup"><span data-stu-id="56216-169">Request</span></span>
<span data-ttu-id="56216-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56216-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries
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

### <a name="response"></a><span data-ttu-id="56216-171">响应</span><span class="sxs-lookup"><span data-stu-id="56216-171">Response</span></span>
<span data-ttu-id="56216-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56216-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




