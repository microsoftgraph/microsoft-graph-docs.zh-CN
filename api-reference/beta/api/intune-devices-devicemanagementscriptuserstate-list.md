---
title: 列出 deviceManagementScriptUserStates
description: 列出 deviceManagementScriptUserState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 989ba836f3e109673509b93c82a6b1f0c17589e8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310550"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="99e37-103">列出 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="99e37-103">List deviceManagementScriptUserStates</span></span>

<span data-ttu-id="99e37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99e37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99e37-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99e37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99e37-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99e37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99e37-107">列出 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99e37-107">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99e37-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="99e37-108">Prerequisites</span></span>
<span data-ttu-id="99e37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e37-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99e37-111">Permission type</span></span>|<span data-ttu-id="99e37-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99e37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99e37-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99e37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99e37-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99e37-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="99e37-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99e37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99e37-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99e37-116">Not supported.</span></span>|
|<span data-ttu-id="99e37-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="99e37-117">Application</span></span>|<span data-ttu-id="99e37-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99e37-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99e37-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99e37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="99e37-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99e37-120">Request headers</span></span>
|<span data-ttu-id="99e37-121">标头</span><span class="sxs-lookup"><span data-stu-id="99e37-121">Header</span></span>|<span data-ttu-id="99e37-122">值</span><span class="sxs-lookup"><span data-stu-id="99e37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99e37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e37-123">Authorization</span></span>|<span data-ttu-id="99e37-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99e37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99e37-125">接受</span><span class="sxs-lookup"><span data-stu-id="99e37-125">Accept</span></span>|<span data-ttu-id="99e37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99e37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99e37-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="99e37-127">Request body</span></span>
<span data-ttu-id="99e37-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99e37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99e37-129">响应</span><span class="sxs-lookup"><span data-stu-id="99e37-129">Response</span></span>
<span data-ttu-id="99e37-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="99e37-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e37-131">示例</span><span class="sxs-lookup"><span data-stu-id="99e37-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="99e37-132">请求</span><span class="sxs-lookup"><span data-stu-id="99e37-132">Request</span></span>
<span data-ttu-id="99e37-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99e37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="99e37-134">响应</span><span class="sxs-lookup"><span data-stu-id="99e37-134">Response</span></span>
<span data-ttu-id="99e37-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99e37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




