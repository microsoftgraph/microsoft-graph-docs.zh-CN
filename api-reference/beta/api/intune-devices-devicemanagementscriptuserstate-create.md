---
title: 创建 deviceManagementScriptUserState
description: 创建新的 deviceManagementScriptUserState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 465ee52f3ac8e0341419e778ec95ec1daa040aa5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807432"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="af116-103">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="af116-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="af116-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af116-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af116-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af116-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af116-106">创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="af116-106">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af116-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="af116-107">Prerequisites</span></span>
<span data-ttu-id="af116-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af116-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="af116-110">Permission type</span></span>|<span data-ttu-id="af116-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af116-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af116-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af116-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af116-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af116-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af116-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af116-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af116-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="af116-115">Not supported.</span></span>|
|<span data-ttu-id="af116-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="af116-116">Application</span></span>|<span data-ttu-id="af116-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="af116-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af116-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af116-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="af116-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="af116-119">Request headers</span></span>
|<span data-ttu-id="af116-120">标头</span><span class="sxs-lookup"><span data-stu-id="af116-120">Header</span></span>|<span data-ttu-id="af116-121">值</span><span class="sxs-lookup"><span data-stu-id="af116-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af116-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af116-122">Authorization</span></span>|<span data-ttu-id="af116-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af116-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af116-124">接受</span><span class="sxs-lookup"><span data-stu-id="af116-124">Accept</span></span>|<span data-ttu-id="af116-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af116-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af116-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af116-126">Request body</span></span>
<span data-ttu-id="af116-127">在请求正文中, 提供 deviceManagementScriptUserState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af116-127">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="af116-128">下表显示创建 deviceManagementScriptUserState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="af116-128">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="af116-129">属性</span><span class="sxs-lookup"><span data-stu-id="af116-129">Property</span></span>|<span data-ttu-id="af116-130">类型</span><span class="sxs-lookup"><span data-stu-id="af116-130">Type</span></span>|<span data-ttu-id="af116-131">说明</span><span class="sxs-lookup"><span data-stu-id="af116-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af116-132">id</span><span class="sxs-lookup"><span data-stu-id="af116-132">id</span></span>|<span data-ttu-id="af116-133">String</span><span class="sxs-lookup"><span data-stu-id="af116-133">String</span></span>|<span data-ttu-id="af116-134">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="af116-134">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="af116-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af116-135">successDeviceCount</span></span>|<span data-ttu-id="af116-136">Int32</span><span class="sxs-lookup"><span data-stu-id="af116-136">Int32</span></span>|<span data-ttu-id="af116-137">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="af116-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="af116-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af116-138">errorDeviceCount</span></span>|<span data-ttu-id="af116-139">Int32</span><span class="sxs-lookup"><span data-stu-id="af116-139">Int32</span></span>|<span data-ttu-id="af116-140">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="af116-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="af116-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af116-141">userPrincipalName</span></span>|<span data-ttu-id="af116-142">String</span><span class="sxs-lookup"><span data-stu-id="af116-142">String</span></span>|<span data-ttu-id="af116-143">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="af116-143">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="af116-144">响应</span><span class="sxs-lookup"><span data-stu-id="af116-144">Response</span></span>
<span data-ttu-id="af116-145">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="af116-145">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af116-146">示例</span><span class="sxs-lookup"><span data-stu-id="af116-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="af116-147">请求</span><span class="sxs-lookup"><span data-stu-id="af116-147">Request</span></span>
<span data-ttu-id="af116-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af116-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="af116-149">响应</span><span class="sxs-lookup"><span data-stu-id="af116-149">Response</span></span>
<span data-ttu-id="af116-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af116-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





