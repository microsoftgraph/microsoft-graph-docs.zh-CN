---
title: 更新 deviceManagementScriptUserState
description: 更新 deviceManagementScriptUserState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5b36ac8f035cf9d4b204a40dfe749f57a004643
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150316"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="09d2b-103">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="09d2b-103">Update deviceManagementScriptUserState</span></span>

<span data-ttu-id="09d2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09d2b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09d2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09d2b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09d2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09d2b-107">更新 [deviceManagementScriptUserState 对象](../resources/intune-devices-devicemanagementscriptuserstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="09d2b-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09d2b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="09d2b-108">Prerequisites</span></span>
<span data-ttu-id="09d2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09d2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09d2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="09d2b-111">Permission type</span></span>|<span data-ttu-id="09d2b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09d2b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09d2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09d2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09d2b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d2b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="09d2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09d2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09d2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09d2b-116">Not supported.</span></span>|
|<span data-ttu-id="09d2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="09d2b-117">Application</span></span>|<span data-ttu-id="09d2b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d2b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09d2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09d2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="09d2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="09d2b-120">Request headers</span></span>
|<span data-ttu-id="09d2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="09d2b-121">Header</span></span>|<span data-ttu-id="09d2b-122">值</span><span class="sxs-lookup"><span data-stu-id="09d2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09d2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09d2b-123">Authorization</span></span>|<span data-ttu-id="09d2b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="09d2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09d2b-125">接受</span><span class="sxs-lookup"><span data-stu-id="09d2b-125">Accept</span></span>|<span data-ttu-id="09d2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09d2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09d2b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="09d2b-127">Request body</span></span>
<span data-ttu-id="09d2b-128">在请求正文中，提供 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09d2b-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="09d2b-129">下表显示创建 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="09d2b-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="09d2b-130">属性</span><span class="sxs-lookup"><span data-stu-id="09d2b-130">Property</span></span>|<span data-ttu-id="09d2b-131">类型</span><span class="sxs-lookup"><span data-stu-id="09d2b-131">Type</span></span>|<span data-ttu-id="09d2b-132">说明</span><span class="sxs-lookup"><span data-stu-id="09d2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09d2b-133">id</span><span class="sxs-lookup"><span data-stu-id="09d2b-133">id</span></span>|<span data-ttu-id="09d2b-134">String</span><span class="sxs-lookup"><span data-stu-id="09d2b-134">String</span></span>|<span data-ttu-id="09d2b-135">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="09d2b-135">Key of the device management script user state entity.</span></span> <span data-ttu-id="09d2b-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="09d2b-136">This property is read-only.</span></span>|
|<span data-ttu-id="09d2b-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09d2b-137">successDeviceCount</span></span>|<span data-ttu-id="09d2b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="09d2b-138">Int32</span></span>|<span data-ttu-id="09d2b-139">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="09d2b-139">Success device count for specific user.</span></span>|
|<span data-ttu-id="09d2b-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09d2b-140">errorDeviceCount</span></span>|<span data-ttu-id="09d2b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="09d2b-141">Int32</span></span>|<span data-ttu-id="09d2b-142">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="09d2b-142">Error device count for specific user.</span></span>|
|<span data-ttu-id="09d2b-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09d2b-143">userPrincipalName</span></span>|<span data-ttu-id="09d2b-144">String</span><span class="sxs-lookup"><span data-stu-id="09d2b-144">String</span></span>|<span data-ttu-id="09d2b-145">特定用户的用户原则名称。</span><span class="sxs-lookup"><span data-stu-id="09d2b-145">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="09d2b-146">响应</span><span class="sxs-lookup"><span data-stu-id="09d2b-146">Response</span></span>
<span data-ttu-id="09d2b-147">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09d2b-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09d2b-148">示例</span><span class="sxs-lookup"><span data-stu-id="09d2b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="09d2b-149">请求</span><span class="sxs-lookup"><span data-stu-id="09d2b-149">Request</span></span>
<span data-ttu-id="09d2b-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09d2b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09d2b-151">响应</span><span class="sxs-lookup"><span data-stu-id="09d2b-151">Response</span></span>
<span data-ttu-id="09d2b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09d2b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




