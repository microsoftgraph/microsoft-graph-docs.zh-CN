---
title: 列出 windowsInformationProtectionDeviceRegistrations
description: 列出 windowsInformationProtectionDeviceRegistration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7680e8e3236c6d8a6c735728e70f0f360da5a7ee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465439"
---
# <a name="list-windowsinformationprotectiondeviceregistrations"></a><span data-ttu-id="3909e-103">列出 windowsInformationProtectionDeviceRegistrations</span><span class="sxs-lookup"><span data-stu-id="3909e-103">List windowsInformationProtectionDeviceRegistrations</span></span>

<span data-ttu-id="3909e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3909e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3909e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3909e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3909e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3909e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3909e-107">列出[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3909e-107">List properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3909e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3909e-108">Prerequisites</span></span>
<span data-ttu-id="3909e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3909e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3909e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3909e-111">Permission type</span></span>|<span data-ttu-id="3909e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3909e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3909e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3909e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3909e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3909e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3909e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3909e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3909e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3909e-116">Not supported.</span></span>|
|<span data-ttu-id="3909e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3909e-117">Application</span></span>|<span data-ttu-id="3909e-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3909e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3909e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3909e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="3909e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3909e-120">Request headers</span></span>
|<span data-ttu-id="3909e-121">标头</span><span class="sxs-lookup"><span data-stu-id="3909e-121">Header</span></span>|<span data-ttu-id="3909e-122">值</span><span class="sxs-lookup"><span data-stu-id="3909e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3909e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3909e-123">Authorization</span></span>|<span data-ttu-id="3909e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3909e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3909e-125">接受</span><span class="sxs-lookup"><span data-stu-id="3909e-125">Accept</span></span>|<span data-ttu-id="3909e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3909e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3909e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3909e-127">Request body</span></span>
<span data-ttu-id="3909e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3909e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3909e-129">响应</span><span class="sxs-lookup"><span data-stu-id="3909e-129">Response</span></span>
<span data-ttu-id="3909e-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3909e-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3909e-131">示例</span><span class="sxs-lookup"><span data-stu-id="3909e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3909e-132">请求</span><span class="sxs-lookup"><span data-stu-id="3909e-132">Request</span></span>
<span data-ttu-id="3909e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3909e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

### <a name="response"></a><span data-ttu-id="3909e-134">响应</span><span class="sxs-lookup"><span data-stu-id="3909e-134">Response</span></span>
<span data-ttu-id="3909e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3909e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
      "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
      "userId": "User Id value",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceName": "Device Name value",
      "deviceType": "Device Type value",
      "deviceMacAddress": "Device Mac Address value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
    }
  ]
}
```



