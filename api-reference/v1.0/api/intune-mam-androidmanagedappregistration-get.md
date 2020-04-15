---
title: 获取 androidManagedAppRegistration
description: 读取 androidManagedAppRegistration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2aa3b9352c3bd3bde82f7b0c7fc0dfcdb8821c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446029"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="ca9ce-103">获取 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ca9ce-103">Get androidManagedAppRegistration</span></span>

<span data-ttu-id="ca9ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca9ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca9ce-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9ce-106">读取 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-106">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca9ce-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca9ce-107">Prerequisites</span></span>
<span data-ttu-id="ca9ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca9ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca9ce-110">Permission type</span></span>|<span data-ttu-id="ca9ce-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca9ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca9ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca9ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca9ce-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca9ce-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ca9ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca9ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca9ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-115">Not supported.</span></span>|
|<span data-ttu-id="ca9ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca9ce-116">Application</span></span>|<span data-ttu-id="ca9ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca9ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca9ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca9ce-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ca9ce-119">Optional query parameters</span></span>
<span data-ttu-id="ca9ce-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca9ce-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca9ce-121">Request headers</span></span>
|<span data-ttu-id="ca9ce-122">标头</span><span class="sxs-lookup"><span data-stu-id="ca9ce-122">Header</span></span>|<span data-ttu-id="ca9ce-123">值</span><span class="sxs-lookup"><span data-stu-id="ca9ce-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca9ce-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca9ce-124">Authorization</span></span>|<span data-ttu-id="ca9ce-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca9ce-126">接受</span><span class="sxs-lookup"><span data-stu-id="ca9ce-126">Accept</span></span>|<span data-ttu-id="ca9ce-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ca9ce-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca9ce-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca9ce-128">Request body</span></span>
<span data-ttu-id="ca9ce-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca9ce-130">响应</span><span class="sxs-lookup"><span data-stu-id="ca9ce-130">Response</span></span>
<span data-ttu-id="ca9ce-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-131">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca9ce-132">示例</span><span class="sxs-lookup"><span data-stu-id="ca9ce-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca9ce-133">请求</span><span class="sxs-lookup"><span data-stu-id="ca9ce-133">Request</span></span>
<span data-ttu-id="ca9ce-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="ca9ce-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca9ce-135">Response</span></span>
<span data-ttu-id="ca9ce-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca9ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
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
}
```






