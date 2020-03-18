---
title: 更新 deviceManagementScriptUserState
description: 更新 deviceManagementScriptUserState 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 31685959c0ab1ec3dc04ae51fadaefbb55d74ca0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814349"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="69f8f-103">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="69f8f-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="69f8f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69f8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f8f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69f8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f8f-106">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69f8f-106">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f8f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69f8f-107">Prerequisites</span></span>
<span data-ttu-id="69f8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f8f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69f8f-110">Permission type</span></span>|<span data-ttu-id="69f8f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69f8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f8f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69f8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69f8f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f8f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69f8f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69f8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f8f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f8f-115">Not supported.</span></span>|
|<span data-ttu-id="69f8f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69f8f-116">Application</span></span>|<span data-ttu-id="69f8f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f8f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f8f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69f8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="69f8f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="69f8f-119">Request headers</span></span>
|<span data-ttu-id="69f8f-120">标头</span><span class="sxs-lookup"><span data-stu-id="69f8f-120">Header</span></span>|<span data-ttu-id="69f8f-121">值</span><span class="sxs-lookup"><span data-stu-id="69f8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f8f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f8f-122">Authorization</span></span>|<span data-ttu-id="69f8f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69f8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f8f-124">接受</span><span class="sxs-lookup"><span data-stu-id="69f8f-124">Accept</span></span>|<span data-ttu-id="69f8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69f8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f8f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69f8f-126">Request body</span></span>
<span data-ttu-id="69f8f-127">在请求正文中，提供[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69f8f-127">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="69f8f-128">下表显示创建[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69f8f-128">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="69f8f-129">属性</span><span class="sxs-lookup"><span data-stu-id="69f8f-129">Property</span></span>|<span data-ttu-id="69f8f-130">类型</span><span class="sxs-lookup"><span data-stu-id="69f8f-130">Type</span></span>|<span data-ttu-id="69f8f-131">说明</span><span class="sxs-lookup"><span data-stu-id="69f8f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f8f-132">id</span><span class="sxs-lookup"><span data-stu-id="69f8f-132">id</span></span>|<span data-ttu-id="69f8f-133">String</span><span class="sxs-lookup"><span data-stu-id="69f8f-133">String</span></span>|<span data-ttu-id="69f8f-134">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="69f8f-134">Key of the device management script user state entity.</span></span> <span data-ttu-id="69f8f-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="69f8f-135">This property is read-only.</span></span>|
|<span data-ttu-id="69f8f-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69f8f-136">successDeviceCount</span></span>|<span data-ttu-id="69f8f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="69f8f-137">Int32</span></span>|<span data-ttu-id="69f8f-138">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="69f8f-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="69f8f-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69f8f-139">errorDeviceCount</span></span>|<span data-ttu-id="69f8f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="69f8f-140">Int32</span></span>|<span data-ttu-id="69f8f-141">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="69f8f-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="69f8f-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69f8f-142">userPrincipalName</span></span>|<span data-ttu-id="69f8f-143">String</span><span class="sxs-lookup"><span data-stu-id="69f8f-143">String</span></span>|<span data-ttu-id="69f8f-144">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="69f8f-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="69f8f-145">响应</span><span class="sxs-lookup"><span data-stu-id="69f8f-145">Response</span></span>
<span data-ttu-id="69f8f-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69f8f-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f8f-147">示例</span><span class="sxs-lookup"><span data-stu-id="69f8f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f8f-148">请求</span><span class="sxs-lookup"><span data-stu-id="69f8f-148">Request</span></span>
<span data-ttu-id="69f8f-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69f8f-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="69f8f-150">响应</span><span class="sxs-lookup"><span data-stu-id="69f8f-150">Response</span></span>
<span data-ttu-id="69f8f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69f8f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```




