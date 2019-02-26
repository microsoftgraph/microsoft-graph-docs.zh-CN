---
title: 列出 androidManagedAppRegistrations
description: 列出 androidManagedAppRegistration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24155fe81d6d42c192cedde012bfa0b0e435a85a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152477"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="05c06-103">列出 androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="05c06-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="05c06-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05c06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05c06-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05c06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c06-106">列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05c06-106">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05c06-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="05c06-107">Prerequisites</span></span>
<span data-ttu-id="05c06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="05c06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05c06-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="05c06-110">Permission type</span></span>|<span data-ttu-id="05c06-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05c06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c06-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05c06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05c06-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="05c06-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="05c06-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05c06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05c06-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="05c06-115">Not supported.</span></span>|
|<span data-ttu-id="05c06-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="05c06-116">Application</span></span>|<span data-ttu-id="05c06-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="05c06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c06-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05c06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="05c06-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="05c06-119">Request headers</span></span>
|<span data-ttu-id="05c06-120">标头</span><span class="sxs-lookup"><span data-stu-id="05c06-120">Header</span></span>|<span data-ttu-id="05c06-121">值</span><span class="sxs-lookup"><span data-stu-id="05c06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05c06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05c06-122">Authorization</span></span>|<span data-ttu-id="05c06-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05c06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05c06-124">Accept</span><span class="sxs-lookup"><span data-stu-id="05c06-124">Accept</span></span>|<span data-ttu-id="05c06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05c06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c06-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="05c06-126">Request body</span></span>
<span data-ttu-id="05c06-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05c06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05c06-128">响应</span><span class="sxs-lookup"><span data-stu-id="05c06-128">Response</span></span>
<span data-ttu-id="05c06-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="05c06-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c06-130">示例</span><span class="sxs-lookup"><span data-stu-id="05c06-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="05c06-131">请求</span><span class="sxs-lookup"><span data-stu-id="05c06-131">Request</span></span>
<span data-ttu-id="05c06-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05c06-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="05c06-133">响应</span><span class="sxs-lookup"><span data-stu-id="05c06-133">Response</span></span>
<span data-ttu-id="05c06-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05c06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




