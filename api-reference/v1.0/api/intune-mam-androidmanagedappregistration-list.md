---
title: 列出 androidManagedAppRegistrations
description: 列出 androidManagedAppRegistration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cc251ed1aa33902784e33c2c23bb948ad0385f7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968271"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="c9e59-103">列出 androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c9e59-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="c9e59-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9e59-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9e59-105">列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9e59-105">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9e59-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9e59-106">Prerequisites</span></span>
<span data-ttu-id="c9e59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9e59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9e59-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9e59-109">Permission type</span></span>|<span data-ttu-id="c9e59-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9e59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9e59-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9e59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9e59-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9e59-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c9e59-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9e59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9e59-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9e59-114">Not supported.</span></span>|
|<span data-ttu-id="c9e59-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9e59-115">Application</span></span>|<span data-ttu-id="c9e59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9e59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9e59-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9e59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="c9e59-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9e59-118">Request headers</span></span>
|<span data-ttu-id="c9e59-119">标头</span><span class="sxs-lookup"><span data-stu-id="c9e59-119">Header</span></span>|<span data-ttu-id="c9e59-120">值</span><span class="sxs-lookup"><span data-stu-id="c9e59-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9e59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9e59-121">Authorization</span></span>|<span data-ttu-id="c9e59-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9e59-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9e59-123">接受</span><span class="sxs-lookup"><span data-stu-id="c9e59-123">Accept</span></span>|<span data-ttu-id="c9e59-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c9e59-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9e59-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9e59-125">Request body</span></span>
<span data-ttu-id="c9e59-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9e59-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e59-127">响应</span><span class="sxs-lookup"><span data-stu-id="c9e59-127">Response</span></span>
<span data-ttu-id="c9e59-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c9e59-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9e59-129">示例</span><span class="sxs-lookup"><span data-stu-id="c9e59-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9e59-130">请求</span><span class="sxs-lookup"><span data-stu-id="c9e59-130">Request</span></span>
<span data-ttu-id="c9e59-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9e59-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="c9e59-132">响应</span><span class="sxs-lookup"><span data-stu-id="c9e59-132">Response</span></span>
<span data-ttu-id="c9e59-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9e59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

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
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```



