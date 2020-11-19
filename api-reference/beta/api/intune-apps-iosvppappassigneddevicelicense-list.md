---
title: 列出 iosVppAppAssignedDeviceLicenses
description: 列出 iosVppAppAssignedDeviceLicense 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 246ea3ed33426f8b7c4a733d8aa3c8053b20c51b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252018"
---
# <a name="list-iosvppappassigneddevicelicenses"></a><span data-ttu-id="58a39-103">列出 iosVppAppAssignedDeviceLicenses</span><span class="sxs-lookup"><span data-stu-id="58a39-103">List iosVppAppAssignedDeviceLicenses</span></span>

<span data-ttu-id="58a39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58a39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58a39-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58a39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a39-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58a39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a39-107">列出 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58a39-107">List properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a39-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="58a39-108">Prerequisites</span></span>
<span data-ttu-id="58a39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="58a39-111">Permission type</span></span>|<span data-ttu-id="58a39-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58a39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58a39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58a39-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a39-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="58a39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58a39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58a39-116">Not supported.</span></span>|
|<span data-ttu-id="58a39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="58a39-117">Application</span></span>|<span data-ttu-id="58a39-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a39-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58a39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="58a39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="58a39-120">Request headers</span></span>
|<span data-ttu-id="58a39-121">标头</span><span class="sxs-lookup"><span data-stu-id="58a39-121">Header</span></span>|<span data-ttu-id="58a39-122">值</span><span class="sxs-lookup"><span data-stu-id="58a39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a39-123">Authorization</span></span>|<span data-ttu-id="58a39-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58a39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a39-125">接受</span><span class="sxs-lookup"><span data-stu-id="58a39-125">Accept</span></span>|<span data-ttu-id="58a39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58a39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58a39-127">Request body</span></span>
<span data-ttu-id="58a39-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58a39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58a39-129">响应</span><span class="sxs-lookup"><span data-stu-id="58a39-129">Response</span></span>
<span data-ttu-id="58a39-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="58a39-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a39-131">示例</span><span class="sxs-lookup"><span data-stu-id="58a39-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a39-132">请求</span><span class="sxs-lookup"><span data-stu-id="58a39-132">Request</span></span>
<span data-ttu-id="58a39-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58a39-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="58a39-134">响应</span><span class="sxs-lookup"><span data-stu-id="58a39-134">Response</span></span>
<span data-ttu-id="58a39-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58a39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
      "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value"
    }
  ]
}
```




