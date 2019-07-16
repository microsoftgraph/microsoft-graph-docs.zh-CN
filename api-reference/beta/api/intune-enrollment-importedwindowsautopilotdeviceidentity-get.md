---
title: 获取 importedWindowsAutopilotDeviceIdentity
description: 读取 importedWindowsAutopilotDeviceIdentity 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 384cdbf7032a18c44e9f217634f7da53cc8f08b9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729983"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="08cda-103">获取 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="08cda-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="08cda-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08cda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08cda-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08cda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08cda-106">读取 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="08cda-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08cda-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08cda-107">Prerequisites</span></span>
<span data-ttu-id="08cda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08cda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08cda-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08cda-110">Permission type</span></span>|<span data-ttu-id="08cda-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08cda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08cda-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08cda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08cda-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="08cda-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="08cda-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08cda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08cda-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08cda-115">Not supported.</span></span>|
|<span data-ttu-id="08cda-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="08cda-116">Application</span></span>|<span data-ttu-id="08cda-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="08cda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08cda-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08cda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08cda-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="08cda-119">Optional query parameters</span></span>
<span data-ttu-id="08cda-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="08cda-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08cda-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="08cda-121">Request headers</span></span>
|<span data-ttu-id="08cda-122">标头</span><span class="sxs-lookup"><span data-stu-id="08cda-122">Header</span></span>|<span data-ttu-id="08cda-123">值</span><span class="sxs-lookup"><span data-stu-id="08cda-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08cda-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="08cda-124">Authorization</span></span>|<span data-ttu-id="08cda-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08cda-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08cda-126">接受</span><span class="sxs-lookup"><span data-stu-id="08cda-126">Accept</span></span>|<span data-ttu-id="08cda-127">application/json</span><span class="sxs-lookup"><span data-stu-id="08cda-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08cda-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="08cda-128">Request body</span></span>
<span data-ttu-id="08cda-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08cda-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08cda-130">响应</span><span class="sxs-lookup"><span data-stu-id="08cda-130">Response</span></span>
<span data-ttu-id="08cda-131">如果成功，此方法会在响应正文中返回`200 OK`响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08cda-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08cda-132">示例</span><span class="sxs-lookup"><span data-stu-id="08cda-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="08cda-133">请求</span><span class="sxs-lookup"><span data-stu-id="08cda-133">Request</span></span>
<span data-ttu-id="08cda-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08cda-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="08cda-135">响应</span><span class="sxs-lookup"><span data-stu-id="08cda-135">Response</span></span>
<span data-ttu-id="08cda-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08cda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "orderIdentifier": "Order Identifier value",
    "groupTag": "Group Tag value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "importId": "Import Id value",
    "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
    "state": {
      "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
      "deviceImportStatus": "pending",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceErrorCode": 15,
      "deviceErrorName": "Device Error Name value"
    },
    "assignedUserPrincipalName": "Assigned User Principal Name value"
  }
}
```





