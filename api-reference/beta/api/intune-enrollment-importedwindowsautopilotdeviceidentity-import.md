---
title: 导入操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ad866ad8180a6e65d7dafe2628bcb9e9be2921b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943773"
---
# <a name="import-action"></a><span data-ttu-id="dfd18-103">导入操作</span><span class="sxs-lookup"><span data-stu-id="dfd18-103">import action</span></span>

> <span data-ttu-id="dfd18-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfd18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfd18-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfd18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfd18-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dfd18-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfd18-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfd18-107">Prerequisites</span></span>
<span data-ttu-id="dfd18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfd18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd18-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfd18-110">Permission type</span></span>|<span data-ttu-id="dfd18-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfd18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfd18-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfd18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfd18-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd18-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dfd18-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfd18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfd18-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfd18-115">Not supported.</span></span>|
|<span data-ttu-id="dfd18-116">Application</span><span class="sxs-lookup"><span data-stu-id="dfd18-116">Application</span></span>|<span data-ttu-id="dfd18-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd18-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfd18-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfd18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="dfd18-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfd18-119">Request headers</span></span>
|<span data-ttu-id="dfd18-120">标头</span><span class="sxs-lookup"><span data-stu-id="dfd18-120">Header</span></span>|<span data-ttu-id="dfd18-121">值</span><span class="sxs-lookup"><span data-stu-id="dfd18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfd18-122">授权</span><span class="sxs-lookup"><span data-stu-id="dfd18-122">Authorization</span></span>|<span data-ttu-id="dfd18-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfd18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfd18-124">接受</span><span class="sxs-lookup"><span data-stu-id="dfd18-124">Accept</span></span>|<span data-ttu-id="dfd18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfd18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfd18-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfd18-126">Request body</span></span>
<span data-ttu-id="dfd18-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfd18-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dfd18-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="dfd18-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dfd18-129">属性</span><span class="sxs-lookup"><span data-stu-id="dfd18-129">Property</span></span>|<span data-ttu-id="dfd18-130">类型</span><span class="sxs-lookup"><span data-stu-id="dfd18-130">Type</span></span>|<span data-ttu-id="dfd18-131">说明</span><span class="sxs-lookup"><span data-stu-id="dfd18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfd18-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="dfd18-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="dfd18-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfd18-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="dfd18-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dfd18-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dfd18-135">响应</span><span class="sxs-lookup"><span data-stu-id="dfd18-135">Response</span></span>
<span data-ttu-id="dfd18-136">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)集合。</span><span class="sxs-lookup"><span data-stu-id="dfd18-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfd18-137">示例</span><span class="sxs-lookup"><span data-stu-id="dfd18-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfd18-138">请求</span><span class="sxs-lookup"><span data-stu-id="dfd18-138">Request</span></span>
<span data-ttu-id="dfd18-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfd18-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 860

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="dfd18-140">响应</span><span class="sxs-lookup"><span data-stu-id="dfd18-140">Response</span></span>
<span data-ttu-id="dfd18-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfd18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 825

{
  "value": [
    {
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
  ]
}
```





