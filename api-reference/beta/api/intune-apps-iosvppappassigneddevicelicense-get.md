---
title: 获取 iosVppAppAssignedDeviceLicense
description: 读取 iosVppAppAssignedDeviceLicense 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8342c075487dd445ea80e2a343f70b29b6505f11
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39925471"
---
# <a name="get-iosvppappassigneddevicelicense"></a><span data-ttu-id="ddcdd-103">获取 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="ddcdd-103">Get iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="ddcdd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddcdd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddcdd-106">读取[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-106">Read properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddcdd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddcdd-107">Prerequisites</span></span>
<span data-ttu-id="ddcdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddcdd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddcdd-110">Permission type</span></span>|<span data-ttu-id="ddcdd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddcdd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddcdd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddcdd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddcdd-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddcdd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ddcdd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddcdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddcdd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-115">Not supported.</span></span>|
|<span data-ttu-id="ddcdd-116">Application</span><span class="sxs-lookup"><span data-stu-id="ddcdd-116">Application</span></span>|<span data-ttu-id="ddcdd-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddcdd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddcdd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddcdd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddcdd-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ddcdd-119">Optional query parameters</span></span>
<span data-ttu-id="ddcdd-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddcdd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddcdd-121">Request headers</span></span>
|<span data-ttu-id="ddcdd-122">标头</span><span class="sxs-lookup"><span data-stu-id="ddcdd-122">Header</span></span>|<span data-ttu-id="ddcdd-123">值</span><span class="sxs-lookup"><span data-stu-id="ddcdd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddcdd-124">授权</span><span class="sxs-lookup"><span data-stu-id="ddcdd-124">Authorization</span></span>|<span data-ttu-id="ddcdd-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddcdd-126">接受</span><span class="sxs-lookup"><span data-stu-id="ddcdd-126">Accept</span></span>|<span data-ttu-id="ddcdd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ddcdd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddcdd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddcdd-128">Request body</span></span>
<span data-ttu-id="ddcdd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddcdd-130">响应</span><span class="sxs-lookup"><span data-stu-id="ddcdd-130">Response</span></span>
<span data-ttu-id="ddcdd-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-131">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddcdd-132">示例</span><span class="sxs-lookup"><span data-stu-id="ddcdd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddcdd-133">请求</span><span class="sxs-lookup"><span data-stu-id="ddcdd-133">Request</span></span>
<span data-ttu-id="ddcdd-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="ddcdd-135">响应</span><span class="sxs-lookup"><span data-stu-id="ddcdd-135">Response</span></span>
<span data-ttu-id="ddcdd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddcdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
    "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "managedDeviceId": "Managed Device Id value",
    "deviceName": "Device Name value"
  }
}
```





