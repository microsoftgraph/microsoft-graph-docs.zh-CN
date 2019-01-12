---
title: 获取 managedDeviceMobileAppConfigurationDeviceStatus
description: 读取属性和 managedDeviceMobileAppConfigurationDeviceStatus 对象的关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dccd5f0bc51c80f627120d22a314d77b127b6090
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986108"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="4b77c-103">获取 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4b77c-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="4b77c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4b77c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b77c-105">读取属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="4b77c-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b77c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b77c-106">Prerequisites</span></span>
<span data-ttu-id="4b77c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4b77c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b77c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b77c-109">Permission type</span></span>|<span data-ttu-id="4b77c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b77c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b77c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b77c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4b77c-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b77c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4b77c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b77c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b77c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b77c-114">Not supported.</span></span>|
|<span data-ttu-id="4b77c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b77c-115">Application</span></span>|<span data-ttu-id="4b77c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b77c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b77c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b77c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b77c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b77c-118">Optional query parameters</span></span>
<span data-ttu-id="4b77c-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b77c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4b77c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b77c-120">Request headers</span></span>
|<span data-ttu-id="4b77c-121">标头</span><span class="sxs-lookup"><span data-stu-id="4b77c-121">Header</span></span>|<span data-ttu-id="4b77c-122">值</span><span class="sxs-lookup"><span data-stu-id="4b77c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b77c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b77c-123">Authorization</span></span>|<span data-ttu-id="4b77c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b77c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b77c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b77c-125">Accept</span></span>|<span data-ttu-id="4b77c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b77c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b77c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b77c-127">Request body</span></span>
<span data-ttu-id="4b77c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b77c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b77c-129">响应</span><span class="sxs-lookup"><span data-stu-id="4b77c-129">Response</span></span>
<span data-ttu-id="4b77c-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4b77c-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b77c-131">示例</span><span class="sxs-lookup"><span data-stu-id="4b77c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b77c-132">请求</span><span class="sxs-lookup"><span data-stu-id="4b77c-132">Request</span></span>
<span data-ttu-id="4b77c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b77c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="4b77c-134">响应</span><span class="sxs-lookup"><span data-stu-id="4b77c-134">Response</span></span>
<span data-ttu-id="4b77c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b77c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "477d3651-3651-477d-5136-7d4751367d47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



