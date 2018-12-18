---
title: 获取 deviceManagementScriptUserState
description: 读取属性和 deviceManagementScriptUserState 对象的关系。
author: tfitzmac
ms.openlocfilehash: a1dbe0bf839c52dc8b1d8c4834188154a0bd1095
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356775"
---
# <a name="get-devicemanagementscriptuserstate"></a><span data-ttu-id="6dd93-103">获取 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="6dd93-103">Get deviceManagementScriptUserState</span></span>

> <span data-ttu-id="6dd93-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6dd93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dd93-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6dd93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6dd93-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6dd93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dd93-107">读取属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="6dd93-107">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6dd93-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6dd93-108">Prerequisites</span></span>
<span data-ttu-id="6dd93-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6dd93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd93-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dd93-111">Permission type</span></span>|<span data-ttu-id="6dd93-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6dd93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dd93-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dd93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dd93-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dd93-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6dd93-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dd93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dd93-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dd93-116">Not supported.</span></span>|
|<span data-ttu-id="6dd93-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dd93-117">Application</span></span>|<span data-ttu-id="6dd93-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dd93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dd93-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dd93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dd93-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6dd93-120">Optional query parameters</span></span>
<span data-ttu-id="6dd93-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6dd93-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6dd93-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dd93-122">Request headers</span></span>
|<span data-ttu-id="6dd93-123">标头</span><span class="sxs-lookup"><span data-stu-id="6dd93-123">Header</span></span>|<span data-ttu-id="6dd93-124">值</span><span class="sxs-lookup"><span data-stu-id="6dd93-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dd93-125">授权</span><span class="sxs-lookup"><span data-stu-id="6dd93-125">Authorization</span></span>|<span data-ttu-id="6dd93-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6dd93-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dd93-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6dd93-127">Accept</span></span>|<span data-ttu-id="6dd93-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6dd93-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dd93-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dd93-129">Request body</span></span>
<span data-ttu-id="6dd93-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6dd93-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dd93-131">响应</span><span class="sxs-lookup"><span data-stu-id="6dd93-131">Response</span></span>
<span data-ttu-id="6dd93-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6dd93-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dd93-133">示例</span><span class="sxs-lookup"><span data-stu-id="6dd93-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6dd93-134">请求</span><span class="sxs-lookup"><span data-stu-id="6dd93-134">Request</span></span>
<span data-ttu-id="6dd93-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dd93-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="6dd93-136">响应</span><span class="sxs-lookup"><span data-stu-id="6dd93-136">Response</span></span>
<span data-ttu-id="6dd93-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dd93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 258

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
    "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "userPrincipalName": "User Principal Name value"
  }
}
```





