---
title: 列表 importedWindowsAutopilotDeviceIdentities
description: 列表属性和importedWindowsAutopilotDeviceIdentity对象关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3e41dddd5c5fd1dd46f6df67376b5215f563e3a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159023"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="1b11d-103">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="1b11d-103">List importedWindowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="1b11d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b11d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b11d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b11d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b11d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b11d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b11d-107">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="1b11d-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b11d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1b11d-108">Prerequisites</span></span>
<span data-ttu-id="1b11d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b11d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b11d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b11d-111">Permission type</span></span>|<span data-ttu-id="1b11d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b11d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b11d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b11d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b11d-114">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b11d-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b11d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b11d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b11d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b11d-116">Not supported.</span></span>|
|<span data-ttu-id="1b11d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b11d-117">Application</span></span>|<span data-ttu-id="1b11d-118">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b11d-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b11d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b11d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1b11d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b11d-120">Request headers</span></span>
|<span data-ttu-id="1b11d-121">标头</span><span class="sxs-lookup"><span data-stu-id="1b11d-121">Header</span></span>|<span data-ttu-id="1b11d-122">值</span><span class="sxs-lookup"><span data-stu-id="1b11d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b11d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b11d-123">Authorization</span></span>|<span data-ttu-id="1b11d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1b11d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b11d-125">接受</span><span class="sxs-lookup"><span data-stu-id="1b11d-125">Accept</span></span>|<span data-ttu-id="1b11d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b11d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b11d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b11d-127">Request body</span></span>
<span data-ttu-id="1b11d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b11d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b11d-129">响应</span><span class="sxs-lookup"><span data-stu-id="1b11d-129">Response</span></span>
<span data-ttu-id="1b11d-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1b11d-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b11d-131">示例</span><span class="sxs-lookup"><span data-stu-id="1b11d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b11d-132">请求</span><span class="sxs-lookup"><span data-stu-id="1b11d-132">Request</span></span>
<span data-ttu-id="1b11d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b11d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="1b11d-134">响应</span><span class="sxs-lookup"><span data-stu-id="1b11d-134">Response</span></span>
<span data-ttu-id="1b11d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b11d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




