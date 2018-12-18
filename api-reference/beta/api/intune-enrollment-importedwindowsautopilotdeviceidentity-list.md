---
title: 列表 importedWindowsAutopilotDeviceIdentities
description: 列表属性和importedWindowsAutopilotDeviceIdentity对象关系。
author: tfitzmac
ms.openlocfilehash: c7a2de8f51f7a2c9cf08d1a3ed2618e9f7081cf9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303960"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="ecb99-103">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="ecb99-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="ecb99-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecb99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecb99-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ecb99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecb99-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ecb99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecb99-107">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="ecb99-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecb99-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecb99-108">Prerequisites</span></span>
<span data-ttu-id="ecb99-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ecb99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb99-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecb99-111">Permission type</span></span>|<span data-ttu-id="ecb99-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ecb99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecb99-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecb99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecb99-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecb99-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ecb99-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecb99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecb99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecb99-116">Not supported.</span></span>|
|<span data-ttu-id="ecb99-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecb99-117">Application</span></span>|<span data-ttu-id="ecb99-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecb99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecb99-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecb99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="ecb99-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecb99-120">Request headers</span></span>
|<span data-ttu-id="ecb99-121">标头</span><span class="sxs-lookup"><span data-stu-id="ecb99-121">Header</span></span>|<span data-ttu-id="ecb99-122">值</span><span class="sxs-lookup"><span data-stu-id="ecb99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecb99-123">授权</span><span class="sxs-lookup"><span data-stu-id="ecb99-123">Authorization</span></span>|<span data-ttu-id="ecb99-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecb99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecb99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ecb99-125">Accept</span></span>|<span data-ttu-id="ecb99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecb99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb99-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecb99-127">Request body</span></span>
<span data-ttu-id="ecb99-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecb99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb99-129">响应</span><span class="sxs-lookup"><span data-stu-id="ecb99-129">Response</span></span>
<span data-ttu-id="ecb99-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ecb99-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb99-131">示例</span><span class="sxs-lookup"><span data-stu-id="ecb99-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecb99-132">请求</span><span class="sxs-lookup"><span data-stu-id="ecb99-132">Request</span></span>
<span data-ttu-id="ecb99-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecb99-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="ecb99-134">响应</span><span class="sxs-lookup"><span data-stu-id="ecb99-134">Response</span></span>
<span data-ttu-id="ecb99-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecb99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      }
    }
  ]
}
```





