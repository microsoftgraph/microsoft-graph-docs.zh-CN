---
title: 列表 managedDeviceMobileAppConfigurationDeviceStatuses
description: 列出属性和 managedDeviceMobileAppConfigurationDeviceStatus 对象之间的关系。
ms.openlocfilehash: 2765b4640d5991c7833f18da33f89937729eac96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048491"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="923c2-103">列表 managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="923c2-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="923c2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="923c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="923c2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="923c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="923c2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="923c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="923c2-107">列出属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="923c2-107">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="923c2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="923c2-108">Prerequisites</span></span>
<span data-ttu-id="923c2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="923c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="923c2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="923c2-111">Permission type</span></span>|<span data-ttu-id="923c2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="923c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="923c2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="923c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="923c2-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="923c2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="923c2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="923c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="923c2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="923c2-116">Not supported.</span></span>|
|<span data-ttu-id="923c2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="923c2-117">Application</span></span>|<span data-ttu-id="923c2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="923c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="923c2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="923c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="923c2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="923c2-120">Request headers</span></span>
|<span data-ttu-id="923c2-121">标头</span><span class="sxs-lookup"><span data-stu-id="923c2-121">Header</span></span>|<span data-ttu-id="923c2-122">值</span><span class="sxs-lookup"><span data-stu-id="923c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="923c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="923c2-123">Authorization</span></span>|<span data-ttu-id="923c2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="923c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="923c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="923c2-125">Accept</span></span>|<span data-ttu-id="923c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="923c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="923c2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="923c2-127">Request body</span></span>
<span data-ttu-id="923c2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="923c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="923c2-129">响应</span><span class="sxs-lookup"><span data-stu-id="923c2-129">Response</span></span>
<span data-ttu-id="923c2-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="923c2-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="923c2-131">示例</span><span class="sxs-lookup"><span data-stu-id="923c2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="923c2-132">请求</span><span class="sxs-lookup"><span data-stu-id="923c2-132">Request</span></span>
<span data-ttu-id="923c2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="923c2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="923c2-134">响应</span><span class="sxs-lookup"><span data-stu-id="923c2-134">Response</span></span>
<span data-ttu-id="923c2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="923c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
      "id": "477d3651-3651-477d-5136-7d4751367d47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





