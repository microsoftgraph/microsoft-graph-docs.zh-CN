---
title: 获取 importedWindowsAutopilotDeviceIdentity
description: 读取 importedWindowsAutopilotDeviceIdentity 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55b4f4fd17fa7f8ea84fe1175898da371ee66ea9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753015"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="57144-103">获取 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="57144-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="57144-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57144-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57144-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57144-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57144-106">读取 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57144-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57144-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="57144-107">Prerequisites</span></span>
<span data-ttu-id="57144-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57144-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57144-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57144-110">Permission type</span></span>|<span data-ttu-id="57144-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57144-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57144-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57144-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57144-113">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57144-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="57144-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57144-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57144-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57144-115">Not supported.</span></span>|
|<span data-ttu-id="57144-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57144-116">Application</span></span>|<span data-ttu-id="57144-117">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57144-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57144-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57144-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57144-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="57144-119">Optional query parameters</span></span>
<span data-ttu-id="57144-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="57144-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57144-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="57144-121">Request headers</span></span>
|<span data-ttu-id="57144-122">标头</span><span class="sxs-lookup"><span data-stu-id="57144-122">Header</span></span>|<span data-ttu-id="57144-123">值</span><span class="sxs-lookup"><span data-stu-id="57144-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57144-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="57144-124">Authorization</span></span>|<span data-ttu-id="57144-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="57144-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57144-126">接受</span><span class="sxs-lookup"><span data-stu-id="57144-126">Accept</span></span>|<span data-ttu-id="57144-127">application/json</span><span class="sxs-lookup"><span data-stu-id="57144-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57144-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="57144-128">Request body</span></span>
<span data-ttu-id="57144-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="57144-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57144-130">响应</span><span class="sxs-lookup"><span data-stu-id="57144-130">Response</span></span>
<span data-ttu-id="57144-131">如果成功，此方法会在响应正文中返回`200 OK`响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57144-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57144-132">示例</span><span class="sxs-lookup"><span data-stu-id="57144-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="57144-133">请求</span><span class="sxs-lookup"><span data-stu-id="57144-133">Request</span></span>
<span data-ttu-id="57144-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57144-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="57144-135">响应</span><span class="sxs-lookup"><span data-stu-id="57144-135">Response</span></span>
<span data-ttu-id="57144-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57144-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
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




