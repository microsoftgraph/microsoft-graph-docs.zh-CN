---
title: 列出 androidManagedAppRegistrations
description: 列出 androidManagedAppRegistration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cfd1b42f7c6ea8d03b53fde825df5212eddb1b1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391746"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="64d21-103">列出 androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="64d21-103">List androidManagedAppRegistrations</span></span>

<span data-ttu-id="64d21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64d21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64d21-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64d21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64d21-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64d21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64d21-107">列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="64d21-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64d21-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64d21-108">Prerequisites</span></span>
<span data-ttu-id="64d21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64d21-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="64d21-111">Permission type</span></span>|<span data-ttu-id="64d21-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64d21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64d21-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64d21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64d21-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d21-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64d21-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64d21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64d21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64d21-116">Not supported.</span></span>|
|<span data-ttu-id="64d21-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="64d21-117">Application</span></span>|<span data-ttu-id="64d21-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d21-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64d21-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64d21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="64d21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64d21-120">Request headers</span></span>
|<span data-ttu-id="64d21-121">标头</span><span class="sxs-lookup"><span data-stu-id="64d21-121">Header</span></span>|<span data-ttu-id="64d21-122">值</span><span class="sxs-lookup"><span data-stu-id="64d21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64d21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64d21-123">Authorization</span></span>|<span data-ttu-id="64d21-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64d21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64d21-125">接受</span><span class="sxs-lookup"><span data-stu-id="64d21-125">Accept</span></span>|<span data-ttu-id="64d21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64d21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64d21-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64d21-127">Request body</span></span>
<span data-ttu-id="64d21-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64d21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64d21-129">响应</span><span class="sxs-lookup"><span data-stu-id="64d21-129">Response</span></span>
<span data-ttu-id="64d21-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="64d21-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64d21-131">示例</span><span class="sxs-lookup"><span data-stu-id="64d21-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64d21-132">请求</span><span class="sxs-lookup"><span data-stu-id="64d21-132">Request</span></span>
<span data-ttu-id="64d21-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64d21-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="64d21-134">响应</span><span class="sxs-lookup"><span data-stu-id="64d21-134">Response</span></span>
<span data-ttu-id="64d21-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64d21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1116

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "managedDeviceId": "Managed Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value",
      "patchVersion": "Patch Version value"
    }
  ]
}
```



