---
title: 列出 iosManagedAppRegistrations
description: 列出 iosManagedAppRegistration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: febf67b40ad00687f347d3d84e8fecc3531ffbe9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256446"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="ececb-103">列出 iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="ececb-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="ececb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ececb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ececb-105">列出 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ececb-105">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ececb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ececb-106">Prerequisites</span></span>
<span data-ttu-id="ececb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ececb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ececb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ececb-109">Permission type</span></span>|<span data-ttu-id="ececb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ececb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ececb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ececb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ececb-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ececb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ececb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ececb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ececb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ececb-114">Not supported.</span></span>|
|<span data-ttu-id="ececb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ececb-115">Application</span></span>|<span data-ttu-id="ececb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ececb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ececb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ececb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="ececb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ececb-118">Request headers</span></span>
|<span data-ttu-id="ececb-119">标头</span><span class="sxs-lookup"><span data-stu-id="ececb-119">Header</span></span>|<span data-ttu-id="ececb-120">值</span><span class="sxs-lookup"><span data-stu-id="ececb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ececb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ececb-121">Authorization</span></span>|<span data-ttu-id="ececb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ececb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ececb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ececb-123">Accept</span></span>|<span data-ttu-id="ececb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ececb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ececb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ececb-125">Request body</span></span>
<span data-ttu-id="ececb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ececb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ececb-127">响应</span><span class="sxs-lookup"><span data-stu-id="ececb-127">Response</span></span>
<span data-ttu-id="ececb-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ececb-128">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ececb-129">示例</span><span class="sxs-lookup"><span data-stu-id="ececb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ececb-130">请求</span><span class="sxs-lookup"><span data-stu-id="ececb-130">Request</span></span>
<span data-ttu-id="ececb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ececb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="ececb-132">响应</span><span class="sxs-lookup"><span data-stu-id="ececb-132">Response</span></span>
<span data-ttu-id="ececb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ececb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
        "bundleId": "Bundle Id value"
      },
      "id": "47632c19-2c19-4763-192c-6347192c6347",
      "version": "Version value"
    }
  ]
}
```



