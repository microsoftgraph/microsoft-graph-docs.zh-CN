---
title: 更新 deviceManagementScriptUserState
description: 更新 deviceManagementScriptUserState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f2d37dec81fb45179fa28268c2a2c49bde219b1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944881"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="2d713-103">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="2d713-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="2d713-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d713-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d713-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d713-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d713-106">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2d713-106">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d713-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d713-107">Prerequisites</span></span>
<span data-ttu-id="2d713-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d713-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d713-110">Permission type</span></span>|<span data-ttu-id="2d713-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d713-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d713-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d713-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d713-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d713-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2d713-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d713-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d713-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d713-115">Not supported.</span></span>|
|<span data-ttu-id="2d713-116">Application</span><span class="sxs-lookup"><span data-stu-id="2d713-116">Application</span></span>|<span data-ttu-id="2d713-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d713-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d713-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d713-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2d713-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d713-119">Request headers</span></span>
|<span data-ttu-id="2d713-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d713-120">Header</span></span>|<span data-ttu-id="2d713-121">值</span><span class="sxs-lookup"><span data-stu-id="2d713-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d713-122">授权</span><span class="sxs-lookup"><span data-stu-id="2d713-122">Authorization</span></span>|<span data-ttu-id="2d713-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d713-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d713-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d713-124">Accept</span></span>|<span data-ttu-id="2d713-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d713-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d713-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d713-126">Request body</span></span>
<span data-ttu-id="2d713-127">在请求正文中，提供[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d713-127">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="2d713-128">下表显示创建[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d713-128">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="2d713-129">属性</span><span class="sxs-lookup"><span data-stu-id="2d713-129">Property</span></span>|<span data-ttu-id="2d713-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d713-130">Type</span></span>|<span data-ttu-id="2d713-131">说明</span><span class="sxs-lookup"><span data-stu-id="2d713-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d713-132">id</span><span class="sxs-lookup"><span data-stu-id="2d713-132">id</span></span>|<span data-ttu-id="2d713-133">String</span><span class="sxs-lookup"><span data-stu-id="2d713-133">String</span></span>|<span data-ttu-id="2d713-134">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="2d713-134">Key of the device management script user state entity.</span></span> <span data-ttu-id="2d713-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2d713-135">This property is read-only.</span></span>|
|<span data-ttu-id="2d713-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d713-136">successDeviceCount</span></span>|<span data-ttu-id="2d713-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2d713-137">Int32</span></span>|<span data-ttu-id="2d713-138">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="2d713-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="2d713-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d713-139">errorDeviceCount</span></span>|<span data-ttu-id="2d713-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2d713-140">Int32</span></span>|<span data-ttu-id="2d713-141">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="2d713-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="2d713-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d713-142">userPrincipalName</span></span>|<span data-ttu-id="2d713-143">字符串</span><span class="sxs-lookup"><span data-stu-id="2d713-143">String</span></span>|<span data-ttu-id="2d713-144">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="2d713-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="2d713-145">响应</span><span class="sxs-lookup"><span data-stu-id="2d713-145">Response</span></span>
<span data-ttu-id="2d713-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d713-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d713-147">示例</span><span class="sxs-lookup"><span data-stu-id="2d713-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d713-148">请求</span><span class="sxs-lookup"><span data-stu-id="2d713-148">Request</span></span>
<span data-ttu-id="2d713-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d713-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d713-150">响应</span><span class="sxs-lookup"><span data-stu-id="2d713-150">Response</span></span>
<span data-ttu-id="2d713-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d713-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





