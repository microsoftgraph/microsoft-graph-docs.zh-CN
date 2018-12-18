---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: tfitzmac
ms.openlocfilehash: 1f674b1c732b5804fd83c89620612354e8daccfa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325632"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="0a695-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="0a695-103">Update deviceInstallState</span></span>

> <span data-ttu-id="0a695-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a695-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a695-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a695-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a695-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0a695-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a695-107">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0a695-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a695-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0a695-108">Prerequisites</span></span>
<span data-ttu-id="0a695-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0a695-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a695-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a695-111">Permission type</span></span>|<span data-ttu-id="0a695-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0a695-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a695-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a695-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a695-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a695-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a695-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a695-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a695-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a695-116">Not supported.</span></span>|
|<span data-ttu-id="0a695-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a695-117">Application</span></span>|<span data-ttu-id="0a695-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a695-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a695-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a695-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="0a695-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a695-120">Request headers</span></span>
|<span data-ttu-id="0a695-121">标头</span><span class="sxs-lookup"><span data-stu-id="0a695-121">Header</span></span>|<span data-ttu-id="0a695-122">值</span><span class="sxs-lookup"><span data-stu-id="0a695-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a695-123">授权</span><span class="sxs-lookup"><span data-stu-id="0a695-123">Authorization</span></span>|<span data-ttu-id="0a695-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0a695-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a695-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a695-125">Accept</span></span>|<span data-ttu-id="0a695-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a695-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a695-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a695-127">Request body</span></span>
<span data-ttu-id="0a695-128">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a695-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="0a695-129">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0a695-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="0a695-130">属性</span><span class="sxs-lookup"><span data-stu-id="0a695-130">Property</span></span>|<span data-ttu-id="0a695-131">类型</span><span class="sxs-lookup"><span data-stu-id="0a695-131">Type</span></span>|<span data-ttu-id="0a695-132">说明</span><span class="sxs-lookup"><span data-stu-id="0a695-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a695-133">id</span><span class="sxs-lookup"><span data-stu-id="0a695-133">id</span></span>|<span data-ttu-id="0a695-134">String</span><span class="sxs-lookup"><span data-stu-id="0a695-134">String</span></span>|<span data-ttu-id="0a695-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0a695-135">Key of the entity.</span></span>|
|<span data-ttu-id="0a695-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="0a695-136">deviceName</span></span>|<span data-ttu-id="0a695-137">String</span><span class="sxs-lookup"><span data-stu-id="0a695-137">String</span></span>|<span data-ttu-id="0a695-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="0a695-138">Device name.</span></span>|
|<span data-ttu-id="0a695-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0a695-139">deviceId</span></span>|<span data-ttu-id="0a695-140">String</span><span class="sxs-lookup"><span data-stu-id="0a695-140">String</span></span>|<span data-ttu-id="0a695-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="0a695-141">Device Id.</span></span>|
|<span data-ttu-id="0a695-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0a695-142">lastSyncDateTime</span></span>|<span data-ttu-id="0a695-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a695-143">DateTimeOffset</span></span>|<span data-ttu-id="0a695-144">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0a695-144">Last sync date and time.</span></span>|
|<span data-ttu-id="0a695-145">installState</span><span class="sxs-lookup"><span data-stu-id="0a695-145">installState</span></span>|[<span data-ttu-id="0a695-146">installState</span><span class="sxs-lookup"><span data-stu-id="0a695-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="0a695-147">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="0a695-147">The install state of the eBook.</span></span> <span data-ttu-id="0a695-148">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="0a695-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="0a695-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="0a695-149">errorCode</span></span>|<span data-ttu-id="0a695-150">String</span><span class="sxs-lookup"><span data-stu-id="0a695-150">String</span></span>|<span data-ttu-id="0a695-151">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="0a695-151">The error code for install failures.</span></span>|
|<span data-ttu-id="0a695-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="0a695-152">osVersion</span></span>|<span data-ttu-id="0a695-153">String</span><span class="sxs-lookup"><span data-stu-id="0a695-153">String</span></span>|<span data-ttu-id="0a695-154">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0a695-154">OS Version.</span></span>|
|<span data-ttu-id="0a695-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="0a695-155">osDescription</span></span>|<span data-ttu-id="0a695-156">String</span><span class="sxs-lookup"><span data-stu-id="0a695-156">String</span></span>|<span data-ttu-id="0a695-157">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="0a695-157">OS Description.</span></span>|
|<span data-ttu-id="0a695-158">userName</span><span class="sxs-lookup"><span data-stu-id="0a695-158">userName</span></span>|<span data-ttu-id="0a695-159">String</span><span class="sxs-lookup"><span data-stu-id="0a695-159">String</span></span>|<span data-ttu-id="0a695-160">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="0a695-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0a695-161">响应</span><span class="sxs-lookup"><span data-stu-id="0a695-161">Response</span></span>
<span data-ttu-id="0a695-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a695-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a695-163">示例</span><span class="sxs-lookup"><span data-stu-id="0a695-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a695-164">请求</span><span class="sxs-lookup"><span data-stu-id="0a695-164">Request</span></span>
<span data-ttu-id="0a695-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a695-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 317

{
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

### <a name="response"></a><span data-ttu-id="0a695-166">响应</span><span class="sxs-lookup"><span data-stu-id="0a695-166">Response</span></span>
<span data-ttu-id="0a695-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a695-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





