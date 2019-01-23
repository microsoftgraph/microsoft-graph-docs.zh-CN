---
title: 更新 deviceManagementScriptUserState
description: 更新 deviceManagementScriptUserState 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c2f25746d54bf1d7c8f9a03fcefc9cecb826de68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419938"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="86fca-103">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="86fca-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="86fca-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="86fca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86fca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86fca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86fca-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86fca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86fca-107">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86fca-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86fca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="86fca-108">Prerequisites</span></span>
<span data-ttu-id="86fca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="86fca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86fca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86fca-111">Permission type</span></span>|<span data-ttu-id="86fca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86fca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86fca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86fca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86fca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86fca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="86fca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86fca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86fca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86fca-116">Not supported.</span></span>|
|<span data-ttu-id="86fca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86fca-117">Application</span></span>|<span data-ttu-id="86fca-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="86fca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86fca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86fca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="86fca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86fca-120">Request headers</span></span>
|<span data-ttu-id="86fca-121">标头</span><span class="sxs-lookup"><span data-stu-id="86fca-121">Header</span></span>|<span data-ttu-id="86fca-122">值</span><span class="sxs-lookup"><span data-stu-id="86fca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86fca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86fca-123">Authorization</span></span>|<span data-ttu-id="86fca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86fca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86fca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86fca-125">Accept</span></span>|<span data-ttu-id="86fca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86fca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86fca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86fca-127">Request body</span></span>
<span data-ttu-id="86fca-128">在请求正文中，提供[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86fca-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="86fca-129">下表显示时创建[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86fca-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="86fca-130">属性</span><span class="sxs-lookup"><span data-stu-id="86fca-130">Property</span></span>|<span data-ttu-id="86fca-131">类型</span><span class="sxs-lookup"><span data-stu-id="86fca-131">Type</span></span>|<span data-ttu-id="86fca-132">说明</span><span class="sxs-lookup"><span data-stu-id="86fca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86fca-133">id</span><span class="sxs-lookup"><span data-stu-id="86fca-133">id</span></span>|<span data-ttu-id="86fca-134">String</span><span class="sxs-lookup"><span data-stu-id="86fca-134">String</span></span>|<span data-ttu-id="86fca-135">设备管理脚本的用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="86fca-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="86fca-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86fca-136">successDeviceCount</span></span>|<span data-ttu-id="86fca-137">Int32</span><span class="sxs-lookup"><span data-stu-id="86fca-137">Int32</span></span>|<span data-ttu-id="86fca-138">成功的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="86fca-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="86fca-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86fca-139">errorDeviceCount</span></span>|<span data-ttu-id="86fca-140">Int32</span><span class="sxs-lookup"><span data-stu-id="86fca-140">Int32</span></span>|<span data-ttu-id="86fca-141">错误的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="86fca-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="86fca-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86fca-142">userPrincipalName</span></span>|<span data-ttu-id="86fca-143">String</span><span class="sxs-lookup"><span data-stu-id="86fca-143">String</span></span>|<span data-ttu-id="86fca-144">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="86fca-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="86fca-145">响应</span><span class="sxs-lookup"><span data-stu-id="86fca-145">Response</span></span>
<span data-ttu-id="86fca-146">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86fca-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86fca-147">示例</span><span class="sxs-lookup"><span data-stu-id="86fca-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="86fca-148">请求</span><span class="sxs-lookup"><span data-stu-id="86fca-148">Request</span></span>
<span data-ttu-id="86fca-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86fca-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="86fca-150">响应</span><span class="sxs-lookup"><span data-stu-id="86fca-150">Response</span></span>
<span data-ttu-id="86fca-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86fca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




