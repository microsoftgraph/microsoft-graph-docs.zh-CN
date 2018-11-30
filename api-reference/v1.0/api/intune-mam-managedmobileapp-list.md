---
title: 列出 managedMobileApps
description: 列出 managedMobileApp 对象的属性和关系。
ms.openlocfilehash: 7f0c9fce4ee4feeab3a78615c9f87db5b4d5775e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009060"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="bb7bd-103">列出 managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="bb7bd-103">List managedMobileApps</span></span>

> <span data-ttu-id="bb7bd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb7bd-105">列出 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-105">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb7bd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb7bd-106">Prerequisites</span></span>
<span data-ttu-id="bb7bd-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bb7bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb7bd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb7bd-109">Permission type</span></span>|<span data-ttu-id="bb7bd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb7bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb7bd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb7bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb7bd-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb7bd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bb7bd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb7bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb7bd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-114">Not supported.</span></span>|
|<span data-ttu-id="bb7bd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb7bd-115">Application</span></span>|<span data-ttu-id="bb7bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb7bd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb7bd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="bb7bd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb7bd-118">Request headers</span></span>
|<span data-ttu-id="bb7bd-119">标头</span><span class="sxs-lookup"><span data-stu-id="bb7bd-119">Header</span></span>|<span data-ttu-id="bb7bd-120">值</span><span class="sxs-lookup"><span data-stu-id="bb7bd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb7bd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb7bd-121">Authorization</span></span>|<span data-ttu-id="bb7bd-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb7bd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb7bd-123">Accept</span></span>|<span data-ttu-id="bb7bd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb7bd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb7bd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb7bd-125">Request body</span></span>
<span data-ttu-id="bb7bd-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb7bd-127">响应</span><span class="sxs-lookup"><span data-stu-id="bb7bd-127">Response</span></span>
<span data-ttu-id="bb7bd-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-128">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb7bd-129">示例</span><span class="sxs-lookup"><span data-stu-id="bb7bd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb7bd-130">请求</span><span class="sxs-lookup"><span data-stu-id="bb7bd-130">Request</span></span>
<span data-ttu-id="bb7bd-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="bb7bd-132">响应</span><span class="sxs-lookup"><span data-stu-id="bb7bd-132">Response</span></span>
<span data-ttu-id="bb7bd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb7bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```



