---
title: 列出 deviceManagementIntentDeviceStates
description: 列出 deviceManagementIntentDeviceState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad27abc8388e7479cf44340b1bc925d9a6a31da4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690922"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="ab226-103">列出 deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="ab226-103">List deviceManagementIntentDeviceStates</span></span>

<span data-ttu-id="ab226-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab226-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab226-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab226-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab226-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab226-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab226-107">列出 [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab226-107">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab226-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab226-108">Prerequisites</span></span>
<span data-ttu-id="ab226-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab226-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab226-111">Permission type</span></span>|<span data-ttu-id="ab226-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab226-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab226-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab226-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab226-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab226-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab226-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab226-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab226-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab226-116">Not supported.</span></span>|
|<span data-ttu-id="ab226-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab226-117">Application</span></span>|<span data-ttu-id="ab226-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab226-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab226-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab226-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="ab226-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab226-120">Request headers</span></span>
|<span data-ttu-id="ab226-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab226-121">Header</span></span>|<span data-ttu-id="ab226-122">值</span><span class="sxs-lookup"><span data-stu-id="ab226-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab226-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab226-123">Authorization</span></span>|<span data-ttu-id="ab226-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab226-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab226-125">接受</span><span class="sxs-lookup"><span data-stu-id="ab226-125">Accept</span></span>|<span data-ttu-id="ab226-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab226-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab226-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab226-127">Request body</span></span>
<span data-ttu-id="ab226-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab226-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab226-129">响应</span><span class="sxs-lookup"><span data-stu-id="ab226-129">Response</span></span>
<span data-ttu-id="ab226-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab226-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab226-131">示例</span><span class="sxs-lookup"><span data-stu-id="ab226-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab226-132">请求</span><span class="sxs-lookup"><span data-stu-id="ab226-132">Request</span></span>
<span data-ttu-id="ab226-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab226-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="ab226-134">响应</span><span class="sxs-lookup"><span data-stu-id="ab226-134">Response</span></span>
<span data-ttu-id="ab226-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab226-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
      "id": "8db75881-5881-8db7-8158-b78d8158b78d",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceDisplayName": "Device Display Name value",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable",
      "deviceId": "Device Id value"
    }
  ]
}
```





