---
title: 列出 managedDeviceMobileAppConfigurationUserStatuses
description: 列出 managedDeviceMobileAppConfigurationUserStatus 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64895bbfa5ef46e05931e1f14774fed864e09ae6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355293"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="9e09b-103">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="9e09b-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="9e09b-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e09b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e09b-105">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e09b-105">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e09b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e09b-106">Prerequisites</span></span>
<span data-ttu-id="9e09b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e09b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e09b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e09b-109">Permission type</span></span>|<span data-ttu-id="9e09b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e09b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e09b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e09b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e09b-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e09b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9e09b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e09b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e09b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e09b-114">Not supported.</span></span>|
|<span data-ttu-id="9e09b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e09b-115">Application</span></span>|<span data-ttu-id="9e09b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e09b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e09b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e09b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9e09b-118">请求头</span><span class="sxs-lookup"><span data-stu-id="9e09b-118">Request headers</span></span>
|<span data-ttu-id="9e09b-119">标头</span><span class="sxs-lookup"><span data-stu-id="9e09b-119">Header</span></span>|<span data-ttu-id="9e09b-120">值</span><span class="sxs-lookup"><span data-stu-id="9e09b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e09b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e09b-121">Authorization</span></span>|<span data-ttu-id="9e09b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e09b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e09b-123">接受</span><span class="sxs-lookup"><span data-stu-id="9e09b-123">Accept</span></span>|<span data-ttu-id="9e09b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e09b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e09b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e09b-125">Request body</span></span>
<span data-ttu-id="9e09b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e09b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e09b-127">响应</span><span class="sxs-lookup"><span data-stu-id="9e09b-127">Response</span></span>
<span data-ttu-id="9e09b-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9e09b-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e09b-129">示例</span><span class="sxs-lookup"><span data-stu-id="9e09b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e09b-130">请求</span><span class="sxs-lookup"><span data-stu-id="9e09b-130">Request</span></span>
<span data-ttu-id="9e09b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e09b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="9e09b-132">响应</span><span class="sxs-lookup"><span data-stu-id="9e09b-132">Response</span></span>
<span data-ttu-id="9e09b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e09b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




