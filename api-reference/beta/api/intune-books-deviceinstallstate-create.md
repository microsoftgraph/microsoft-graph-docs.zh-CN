---
title: 创建 deviceInstallState
description: 创建新的 deviceInstallState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfc1adae0175dcdf2c19d90d54bf597316919994
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990899"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="8056e-103">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="8056e-103">Create deviceInstallState</span></span>

> <span data-ttu-id="8056e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8056e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8056e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8056e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8056e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8056e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8056e-107">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8056e-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8056e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8056e-108">Prerequisites</span></span>
<span data-ttu-id="8056e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8056e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8056e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8056e-111">Permission type</span></span>|<span data-ttu-id="8056e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8056e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8056e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8056e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8056e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8056e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8056e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8056e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8056e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8056e-116">Not supported.</span></span>|
|<span data-ttu-id="8056e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8056e-117">Application</span></span>|<span data-ttu-id="8056e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8056e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8056e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8056e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="8056e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8056e-120">Request headers</span></span>
|<span data-ttu-id="8056e-121">标头</span><span class="sxs-lookup"><span data-stu-id="8056e-121">Header</span></span>|<span data-ttu-id="8056e-122">值</span><span class="sxs-lookup"><span data-stu-id="8056e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8056e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8056e-123">Authorization</span></span>|<span data-ttu-id="8056e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8056e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8056e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8056e-125">Accept</span></span>|<span data-ttu-id="8056e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8056e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8056e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8056e-127">Request body</span></span>
<span data-ttu-id="8056e-128">在请求正文中，提供 deviceInstallState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8056e-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="8056e-129">下表显示创建 deviceInstallState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8056e-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="8056e-130">属性</span><span class="sxs-lookup"><span data-stu-id="8056e-130">Property</span></span>|<span data-ttu-id="8056e-131">类型</span><span class="sxs-lookup"><span data-stu-id="8056e-131">Type</span></span>|<span data-ttu-id="8056e-132">说明</span><span class="sxs-lookup"><span data-stu-id="8056e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8056e-133">id</span><span class="sxs-lookup"><span data-stu-id="8056e-133">id</span></span>|<span data-ttu-id="8056e-134">String</span><span class="sxs-lookup"><span data-stu-id="8056e-134">String</span></span>|<span data-ttu-id="8056e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8056e-135">Key of the entity.</span></span>|
|<span data-ttu-id="8056e-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="8056e-136">deviceName</span></span>|<span data-ttu-id="8056e-137">String</span><span class="sxs-lookup"><span data-stu-id="8056e-137">String</span></span>|<span data-ttu-id="8056e-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="8056e-138">Device name.</span></span>|
|<span data-ttu-id="8056e-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="8056e-139">deviceId</span></span>|<span data-ttu-id="8056e-140">String</span><span class="sxs-lookup"><span data-stu-id="8056e-140">String</span></span>|<span data-ttu-id="8056e-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="8056e-141">Device Id.</span></span>|
|<span data-ttu-id="8056e-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8056e-142">lastSyncDateTime</span></span>|<span data-ttu-id="8056e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8056e-143">DateTimeOffset</span></span>|<span data-ttu-id="8056e-144">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8056e-144">Last sync date and time.</span></span>|
|<span data-ttu-id="8056e-145">installState</span><span class="sxs-lookup"><span data-stu-id="8056e-145">installState</span></span>|[<span data-ttu-id="8056e-146">installState</span><span class="sxs-lookup"><span data-stu-id="8056e-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="8056e-147">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="8056e-147">The install state of the eBook.</span></span> <span data-ttu-id="8056e-148">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="8056e-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="8056e-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="8056e-149">errorCode</span></span>|<span data-ttu-id="8056e-150">String</span><span class="sxs-lookup"><span data-stu-id="8056e-150">String</span></span>|<span data-ttu-id="8056e-151">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="8056e-151">The error code for install failures.</span></span>|
|<span data-ttu-id="8056e-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="8056e-152">osVersion</span></span>|<span data-ttu-id="8056e-153">String</span><span class="sxs-lookup"><span data-stu-id="8056e-153">String</span></span>|<span data-ttu-id="8056e-154">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8056e-154">OS Version.</span></span>|
|<span data-ttu-id="8056e-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="8056e-155">osDescription</span></span>|<span data-ttu-id="8056e-156">String</span><span class="sxs-lookup"><span data-stu-id="8056e-156">String</span></span>|<span data-ttu-id="8056e-157">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="8056e-157">OS Description.</span></span>|
|<span data-ttu-id="8056e-158">userName</span><span class="sxs-lookup"><span data-stu-id="8056e-158">userName</span></span>|<span data-ttu-id="8056e-159">String</span><span class="sxs-lookup"><span data-stu-id="8056e-159">String</span></span>|<span data-ttu-id="8056e-160">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="8056e-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="8056e-161">响应</span><span class="sxs-lookup"><span data-stu-id="8056e-161">Response</span></span>
<span data-ttu-id="8056e-162">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8056e-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8056e-163">示例</span><span class="sxs-lookup"><span data-stu-id="8056e-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="8056e-164">请求</span><span class="sxs-lookup"><span data-stu-id="8056e-164">Request</span></span>
<span data-ttu-id="8056e-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8056e-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="8056e-166">响应</span><span class="sxs-lookup"><span data-stu-id="8056e-166">Response</span></span>
<span data-ttu-id="8056e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8056e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





