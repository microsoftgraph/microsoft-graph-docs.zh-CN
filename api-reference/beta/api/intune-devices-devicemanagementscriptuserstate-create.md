---
title: 创建 deviceManagementScriptUserState
description: 创建新的 deviceManagementScriptUserState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 93aca9ce1689f3159594963af062616a2b1de7eb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940797"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="80348-103">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="80348-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="80348-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80348-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80348-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80348-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80348-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80348-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80348-107">创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80348-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80348-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="80348-108">Prerequisites</span></span>
<span data-ttu-id="80348-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="80348-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80348-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80348-111">Permission type</span></span>|<span data-ttu-id="80348-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80348-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80348-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80348-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80348-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80348-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="80348-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80348-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80348-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80348-116">Not supported.</span></span>|
|<span data-ttu-id="80348-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80348-117">Application</span></span>|<span data-ttu-id="80348-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="80348-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80348-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80348-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="80348-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80348-120">Request headers</span></span>
|<span data-ttu-id="80348-121">标头</span><span class="sxs-lookup"><span data-stu-id="80348-121">Header</span></span>|<span data-ttu-id="80348-122">值</span><span class="sxs-lookup"><span data-stu-id="80348-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80348-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80348-123">Authorization</span></span>|<span data-ttu-id="80348-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80348-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80348-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80348-125">Accept</span></span>|<span data-ttu-id="80348-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80348-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80348-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80348-127">Request body</span></span>
<span data-ttu-id="80348-128">在请求正文中，提供 deviceManagementScriptUserState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80348-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="80348-129">下表显示时创建 deviceManagementScriptUserState 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80348-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="80348-130">属性</span><span class="sxs-lookup"><span data-stu-id="80348-130">Property</span></span>|<span data-ttu-id="80348-131">类型</span><span class="sxs-lookup"><span data-stu-id="80348-131">Type</span></span>|<span data-ttu-id="80348-132">说明</span><span class="sxs-lookup"><span data-stu-id="80348-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80348-133">id</span><span class="sxs-lookup"><span data-stu-id="80348-133">id</span></span>|<span data-ttu-id="80348-134">字符串</span><span class="sxs-lookup"><span data-stu-id="80348-134">String</span></span>|<span data-ttu-id="80348-135">设备管理脚本的用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="80348-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="80348-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80348-136">successDeviceCount</span></span>|<span data-ttu-id="80348-137">Int32</span><span class="sxs-lookup"><span data-stu-id="80348-137">Int32</span></span>|<span data-ttu-id="80348-138">成功的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="80348-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="80348-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80348-139">errorDeviceCount</span></span>|<span data-ttu-id="80348-140">Int32</span><span class="sxs-lookup"><span data-stu-id="80348-140">Int32</span></span>|<span data-ttu-id="80348-141">错误的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="80348-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="80348-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80348-142">userPrincipalName</span></span>|<span data-ttu-id="80348-143">字符串</span><span class="sxs-lookup"><span data-stu-id="80348-143">String</span></span>|<span data-ttu-id="80348-144">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="80348-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="80348-145">响应</span><span class="sxs-lookup"><span data-stu-id="80348-145">Response</span></span>
<span data-ttu-id="80348-146">如果成功，此方法返回`201 Created`响应代码和响应正文中的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80348-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80348-147">示例</span><span class="sxs-lookup"><span data-stu-id="80348-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="80348-148">请求</span><span class="sxs-lookup"><span data-stu-id="80348-148">Request</span></span>
<span data-ttu-id="80348-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80348-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80348-150">响应</span><span class="sxs-lookup"><span data-stu-id="80348-150">Response</span></span>
<span data-ttu-id="80348-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80348-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





