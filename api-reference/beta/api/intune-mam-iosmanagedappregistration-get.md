---
title: 获取 iosManagedAppRegistration
description: 读取 iosManagedAppRegistration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5365d6d653ce35fd1ffedc857abcd098a0c8b5b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821950"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="20683-103">获取 iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="20683-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="20683-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="20683-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20683-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="20683-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20683-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20683-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20683-107">读取 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="20683-107">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20683-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="20683-108">Prerequisites</span></span>
<span data-ttu-id="20683-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="20683-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20683-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="20683-111">Permission type</span></span>|<span data-ttu-id="20683-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="20683-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20683-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20683-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20683-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20683-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="20683-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20683-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20683-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20683-116">Not supported.</span></span>|
|<span data-ttu-id="20683-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="20683-117">Application</span></span>|<span data-ttu-id="20683-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="20683-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20683-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20683-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20683-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20683-120">Optional query parameters</span></span>
<span data-ttu-id="20683-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="20683-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20683-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="20683-122">Request headers</span></span>
|<span data-ttu-id="20683-123">标头</span><span class="sxs-lookup"><span data-stu-id="20683-123">Header</span></span>|<span data-ttu-id="20683-124">值</span><span class="sxs-lookup"><span data-stu-id="20683-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20683-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="20683-125">Authorization</span></span>|<span data-ttu-id="20683-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20683-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20683-127">Accept</span><span class="sxs-lookup"><span data-stu-id="20683-127">Accept</span></span>|<span data-ttu-id="20683-128">application/json</span><span class="sxs-lookup"><span data-stu-id="20683-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20683-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="20683-129">Request body</span></span>
<span data-ttu-id="20683-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20683-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20683-131">响应</span><span class="sxs-lookup"><span data-stu-id="20683-131">Response</span></span>
<span data-ttu-id="20683-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20683-132">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20683-133">示例</span><span class="sxs-lookup"><span data-stu-id="20683-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="20683-134">请求</span><span class="sxs-lookup"><span data-stu-id="20683-134">Request</span></span>
<span data-ttu-id="20683-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20683-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="20683-136">响应</span><span class="sxs-lookup"><span data-stu-id="20683-136">Response</span></span>
<span data-ttu-id="20683-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20683-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```





