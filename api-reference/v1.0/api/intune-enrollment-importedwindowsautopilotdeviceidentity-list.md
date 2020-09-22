---
title: 列表 importedWindowsAutopilotDeviceIdentities
description: 列表属性和importedWindowsAutopilotDeviceIdentity对象关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d3a91bcac93fe9d754d86db735793467b995315
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094622"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="e71eb-103">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="e71eb-103">List importedWindowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="e71eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e71eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e71eb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e71eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e71eb-106">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="e71eb-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e71eb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e71eb-107">Prerequisites</span></span>
<span data-ttu-id="e71eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e71eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e71eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e71eb-110">Permission type</span></span>|<span data-ttu-id="e71eb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e71eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e71eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e71eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e71eb-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e71eb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e71eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e71eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e71eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e71eb-115">Not supported.</span></span>|
|<span data-ttu-id="e71eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e71eb-116">Application</span></span>|<span data-ttu-id="e71eb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e71eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e71eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e71eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e71eb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e71eb-119">Request headers</span></span>
|<span data-ttu-id="e71eb-120">标头</span><span class="sxs-lookup"><span data-stu-id="e71eb-120">Header</span></span>|<span data-ttu-id="e71eb-121">值</span><span class="sxs-lookup"><span data-stu-id="e71eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e71eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e71eb-122">Authorization</span></span>|<span data-ttu-id="e71eb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e71eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e71eb-124">接受</span><span class="sxs-lookup"><span data-stu-id="e71eb-124">Accept</span></span>|<span data-ttu-id="e71eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e71eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e71eb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e71eb-126">Request body</span></span>
<span data-ttu-id="e71eb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e71eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e71eb-128">响应</span><span class="sxs-lookup"><span data-stu-id="e71eb-128">Response</span></span>
<span data-ttu-id="e71eb-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e71eb-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e71eb-130">示例</span><span class="sxs-lookup"><span data-stu-id="e71eb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e71eb-131">请求</span><span class="sxs-lookup"><span data-stu-id="e71eb-131">Request</span></span>
<span data-ttu-id="e71eb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e71eb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="e71eb-133">响应</span><span class="sxs-lookup"><span data-stu-id="e71eb-133">Response</span></span>
<span data-ttu-id="e71eb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e71eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









