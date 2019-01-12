---
title: 创建 deviceInstallState
description: 创建新的 deviceInstallState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7e37857cfa7d7c8820844f506b59d50933c5866
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962539"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="f1ba1-103">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f1ba1-103">Create deviceInstallState</span></span>

> <span data-ttu-id="f1ba1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1ba1-105">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1ba1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1ba1-106">Prerequisites</span></span>
<span data-ttu-id="f1ba1-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f1ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ba1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1ba1-109">Permission type</span></span>|<span data-ttu-id="f1ba1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1ba1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1ba1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1ba1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1ba1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ba1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1ba1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1ba1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1ba1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-114">Not supported.</span></span>|
|<span data-ttu-id="f1ba1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1ba1-115">Application</span></span>|<span data-ttu-id="f1ba1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1ba1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1ba1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="f1ba1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1ba1-118">Request headers</span></span>
|<span data-ttu-id="f1ba1-119">标头</span><span class="sxs-lookup"><span data-stu-id="f1ba1-119">Header</span></span>|<span data-ttu-id="f1ba1-120">值</span><span class="sxs-lookup"><span data-stu-id="f1ba1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1ba1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1ba1-121">Authorization</span></span>|<span data-ttu-id="f1ba1-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1ba1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f1ba1-123">Accept</span></span>|<span data-ttu-id="f1ba1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ba1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ba1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1ba1-125">Request body</span></span>
<span data-ttu-id="f1ba1-126">在请求正文中，提供 deviceInstallState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="f1ba1-127">下表显示创建 deviceInstallState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="f1ba1-128">属性</span><span class="sxs-lookup"><span data-stu-id="f1ba1-128">Property</span></span>|<span data-ttu-id="f1ba1-129">类型</span><span class="sxs-lookup"><span data-stu-id="f1ba1-129">Type</span></span>|<span data-ttu-id="f1ba1-130">说明</span><span class="sxs-lookup"><span data-stu-id="f1ba1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ba1-131">id</span><span class="sxs-lookup"><span data-stu-id="f1ba1-131">id</span></span>|<span data-ttu-id="f1ba1-132">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-132">String</span></span>|<span data-ttu-id="f1ba1-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-133">Key of the entity.</span></span>|
|<span data-ttu-id="f1ba1-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="f1ba1-134">deviceName</span></span>|<span data-ttu-id="f1ba1-135">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-135">String</span></span>|<span data-ttu-id="f1ba1-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-136">Device name.</span></span>|
|<span data-ttu-id="f1ba1-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="f1ba1-137">deviceId</span></span>|<span data-ttu-id="f1ba1-138">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-138">String</span></span>|<span data-ttu-id="f1ba1-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-139">Device Id.</span></span>|
|<span data-ttu-id="f1ba1-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f1ba1-140">lastSyncDateTime</span></span>|<span data-ttu-id="f1ba1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1ba1-141">DateTimeOffset</span></span>|<span data-ttu-id="f1ba1-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-142">Last sync date and time.</span></span>|
|<span data-ttu-id="f1ba1-143">installState</span><span class="sxs-lookup"><span data-stu-id="f1ba1-143">installState</span></span>|[<span data-ttu-id="f1ba1-144">installState</span><span class="sxs-lookup"><span data-stu-id="f1ba1-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="f1ba1-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-145">The install state of the eBook.</span></span> <span data-ttu-id="f1ba1-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="f1ba1-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="f1ba1-147">errorCode</span></span>|<span data-ttu-id="f1ba1-148">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-148">String</span></span>|<span data-ttu-id="f1ba1-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-149">The error code for install failures.</span></span>|
|<span data-ttu-id="f1ba1-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="f1ba1-150">osVersion</span></span>|<span data-ttu-id="f1ba1-151">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-151">String</span></span>|<span data-ttu-id="f1ba1-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-152">OS Version.</span></span>|
|<span data-ttu-id="f1ba1-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="f1ba1-153">osDescription</span></span>|<span data-ttu-id="f1ba1-154">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-154">String</span></span>|<span data-ttu-id="f1ba1-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-155">OS Description.</span></span>|
|<span data-ttu-id="f1ba1-156">userName</span><span class="sxs-lookup"><span data-stu-id="f1ba1-156">userName</span></span>|<span data-ttu-id="f1ba1-157">String</span><span class="sxs-lookup"><span data-stu-id="f1ba1-157">String</span></span>|<span data-ttu-id="f1ba1-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f1ba1-159">响应</span><span class="sxs-lookup"><span data-stu-id="f1ba1-159">Response</span></span>
<span data-ttu-id="f1ba1-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ba1-161">示例</span><span class="sxs-lookup"><span data-stu-id="f1ba1-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1ba1-162">请求</span><span class="sxs-lookup"><span data-stu-id="f1ba1-162">Request</span></span>
<span data-ttu-id="f1ba1-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="f1ba1-164">响应</span><span class="sxs-lookup"><span data-stu-id="f1ba1-164">Response</span></span>
<span data-ttu-id="f1ba1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1ba1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```



