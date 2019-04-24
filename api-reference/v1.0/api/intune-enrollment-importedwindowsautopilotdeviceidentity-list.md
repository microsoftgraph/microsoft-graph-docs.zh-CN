---
title: 列表 importedWindowsAutopilotDeviceIdentities
description: 列表属性和importedWindowsAutopilotDeviceIdentity对象关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e65a91af12b7f1689253ed95da341abd9d1aee36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459694"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="2c019-103">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2c019-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="2c019-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c019-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c019-105">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="2c019-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c019-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c019-106">Prerequisites</span></span>
<span data-ttu-id="2c019-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c019-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c019-109">Permission type</span></span>|<span data-ttu-id="2c019-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c019-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c019-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c019-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2c019-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c019-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2c019-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c019-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c019-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c019-114">Not supported.</span></span>|
|<span data-ttu-id="2c019-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c019-115">Application</span></span>|<span data-ttu-id="2c019-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c019-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c019-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c019-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="2c019-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c019-118">Request headers</span></span>
|<span data-ttu-id="2c019-119">标头</span><span class="sxs-lookup"><span data-stu-id="2c019-119">Header</span></span>|<span data-ttu-id="2c019-120">值</span><span class="sxs-lookup"><span data-stu-id="2c019-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c019-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c019-121">Authorization</span></span>|<span data-ttu-id="2c019-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c019-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c019-123">接受</span><span class="sxs-lookup"><span data-stu-id="2c019-123">Accept</span></span>|<span data-ttu-id="2c019-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2c019-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c019-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c019-125">Request body</span></span>
<span data-ttu-id="2c019-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c019-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c019-127">响应</span><span class="sxs-lookup"><span data-stu-id="2c019-127">Response</span></span>
<span data-ttu-id="2c019-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c019-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c019-129">示例</span><span class="sxs-lookup"><span data-stu-id="2c019-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c019-130">请求</span><span class="sxs-lookup"><span data-stu-id="2c019-130">Request</span></span>
<span data-ttu-id="2c019-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c019-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="2c019-132">响应</span><span class="sxs-lookup"><span data-stu-id="2c019-132">Response</span></span>
<span data-ttu-id="2c019-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c019-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



