---
title: executeAction 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 23d34a999fdc874126fee527c7c62b32d859d953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912993"
---
# <a name="executeaction-action"></a><span data-ttu-id="fae1e-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="fae1e-103">executeAction action</span></span>

> <span data-ttu-id="fae1e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fae1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fae1e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fae1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fae1e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fae1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fae1e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fae1e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fae1e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fae1e-108">Prerequisites</span></span>
<span data-ttu-id="fae1e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fae1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fae1e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fae1e-111">Permission type</span></span>|<span data-ttu-id="fae1e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fae1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fae1e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fae1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fae1e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fae1e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fae1e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fae1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fae1e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fae1e-116">Not supported.</span></span>|
|<span data-ttu-id="fae1e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fae1e-117">Application</span></span>|<span data-ttu-id="fae1e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fae1e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fae1e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fae1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="fae1e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fae1e-120">Request headers</span></span>
|<span data-ttu-id="fae1e-121">标头</span><span class="sxs-lookup"><span data-stu-id="fae1e-121">Header</span></span>|<span data-ttu-id="fae1e-122">值</span><span class="sxs-lookup"><span data-stu-id="fae1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fae1e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fae1e-123">Authorization</span></span>|<span data-ttu-id="fae1e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fae1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fae1e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fae1e-125">Accept</span></span>|<span data-ttu-id="fae1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fae1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fae1e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fae1e-127">Request body</span></span>
<span data-ttu-id="fae1e-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fae1e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fae1e-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="fae1e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fae1e-130">属性</span><span class="sxs-lookup"><span data-stu-id="fae1e-130">Property</span></span>|<span data-ttu-id="fae1e-131">类型</span><span class="sxs-lookup"><span data-stu-id="fae1e-131">Type</span></span>|<span data-ttu-id="fae1e-132">说明</span><span class="sxs-lookup"><span data-stu-id="fae1e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fae1e-133">actionName</span><span class="sxs-lookup"><span data-stu-id="fae1e-133">actionName</span></span>|[<span data-ttu-id="fae1e-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="fae1e-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="fae1e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fae1e-135">Not yet documented</span></span>|
|<span data-ttu-id="fae1e-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="fae1e-136">deviceIds</span></span>|<span data-ttu-id="fae1e-137">String collection</span><span class="sxs-lookup"><span data-stu-id="fae1e-137">String collection</span></span>|<span data-ttu-id="fae1e-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fae1e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fae1e-139">响应</span><span class="sxs-lookup"><span data-stu-id="fae1e-139">Response</span></span>
<span data-ttu-id="fae1e-140">如果成功，此操作将返回`200 OK`响应代码和响应正文中[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="fae1e-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fae1e-141">示例</span><span class="sxs-lookup"><span data-stu-id="fae1e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="fae1e-142">请求</span><span class="sxs-lookup"><span data-stu-id="fae1e-142">Request</span></span>
<span data-ttu-id="fae1e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fae1e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/executeAction

Content-type: application/json
Content-length: 78

{
  "actionName": "delete",
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fae1e-144">响应</span><span class="sxs-lookup"><span data-stu-id="fae1e-144">Response</span></span>
<span data-ttu-id="fae1e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fae1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```





