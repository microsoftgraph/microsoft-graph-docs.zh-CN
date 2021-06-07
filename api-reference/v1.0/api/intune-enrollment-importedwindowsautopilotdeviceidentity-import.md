---
title: 导入操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 750b525ec0cdf7c28213787920c8164f7fcb1ac5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753014"
---
# <a name="import-action"></a><span data-ttu-id="21213-103">导入操作</span><span class="sxs-lookup"><span data-stu-id="21213-103">import action</span></span>

<span data-ttu-id="21213-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21213-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21213-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21213-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21213-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="21213-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21213-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="21213-107">Prerequisites</span></span>
<span data-ttu-id="21213-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21213-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="21213-110">Permission type</span></span>|<span data-ttu-id="21213-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21213-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21213-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21213-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21213-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21213-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21213-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21213-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21213-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="21213-115">Not supported.</span></span>|
|<span data-ttu-id="21213-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="21213-116">Application</span></span>|<span data-ttu-id="21213-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21213-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21213-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21213-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="21213-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="21213-119">Request headers</span></span>
|<span data-ttu-id="21213-120">标头</span><span class="sxs-lookup"><span data-stu-id="21213-120">Header</span></span>|<span data-ttu-id="21213-121">值</span><span class="sxs-lookup"><span data-stu-id="21213-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21213-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21213-122">Authorization</span></span>|<span data-ttu-id="21213-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21213-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21213-124">接受</span><span class="sxs-lookup"><span data-stu-id="21213-124">Accept</span></span>|<span data-ttu-id="21213-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21213-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21213-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="21213-126">Request body</span></span>
<span data-ttu-id="21213-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21213-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="21213-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="21213-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="21213-129">属性</span><span class="sxs-lookup"><span data-stu-id="21213-129">Property</span></span>|<span data-ttu-id="21213-130">类型</span><span class="sxs-lookup"><span data-stu-id="21213-130">Type</span></span>|<span data-ttu-id="21213-131">说明</span><span class="sxs-lookup"><span data-stu-id="21213-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21213-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="21213-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="21213-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21213-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="21213-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="21213-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="21213-135">响应</span><span class="sxs-lookup"><span data-stu-id="21213-135">Response</span></span>
<span data-ttu-id="21213-136">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="21213-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21213-137">示例</span><span class="sxs-lookup"><span data-stu-id="21213-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="21213-138">请求</span><span class="sxs-lookup"><span data-stu-id="21213-138">Request</span></span>
<span data-ttu-id="21213-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21213-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 808

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="21213-140">响应</span><span class="sxs-lookup"><span data-stu-id="21213-140">Response</span></span>
<span data-ttu-id="21213-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21213-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 773

{
  "value": [
    {
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
  ]
}
```




