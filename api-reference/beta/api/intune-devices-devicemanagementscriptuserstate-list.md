---
title: 列出 deviceManagementScriptUserStates
description: 列出 deviceManagementScriptUserState 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4d16a8c54a0fc099ef173db8e72ecbed5a11f3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465445"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="e74cc-103">列出 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="e74cc-103">List deviceManagementScriptUserStates</span></span>

> <span data-ttu-id="e74cc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e74cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e74cc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e74cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e74cc-106">列出[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e74cc-106">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e74cc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e74cc-107">Prerequisites</span></span>
<span data-ttu-id="e74cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e74cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74cc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e74cc-110">Permission type</span></span>|<span data-ttu-id="e74cc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e74cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e74cc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e74cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e74cc-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e74cc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e74cc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e74cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e74cc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e74cc-115">Not supported.</span></span>|
|<span data-ttu-id="e74cc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e74cc-116">Application</span></span>|<span data-ttu-id="e74cc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e74cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e74cc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e74cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="e74cc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e74cc-119">Request headers</span></span>
|<span data-ttu-id="e74cc-120">标头</span><span class="sxs-lookup"><span data-stu-id="e74cc-120">Header</span></span>|<span data-ttu-id="e74cc-121">值</span><span class="sxs-lookup"><span data-stu-id="e74cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e74cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e74cc-122">Authorization</span></span>|<span data-ttu-id="e74cc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e74cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e74cc-124">接受</span><span class="sxs-lookup"><span data-stu-id="e74cc-124">Accept</span></span>|<span data-ttu-id="e74cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e74cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e74cc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e74cc-126">Request body</span></span>
<span data-ttu-id="e74cc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e74cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74cc-128">响应</span><span class="sxs-lookup"><span data-stu-id="e74cc-128">Response</span></span>
<span data-ttu-id="e74cc-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e74cc-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e74cc-130">示例</span><span class="sxs-lookup"><span data-stu-id="e74cc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e74cc-131">请求</span><span class="sxs-lookup"><span data-stu-id="e74cc-131">Request</span></span>
<span data-ttu-id="e74cc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e74cc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="e74cc-133">响应</span><span class="sxs-lookup"><span data-stu-id="e74cc-133">Response</span></span>
<span data-ttu-id="e74cc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e74cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
      "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
      "successDeviceCount": 2,
      "errorDeviceCount": 0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





