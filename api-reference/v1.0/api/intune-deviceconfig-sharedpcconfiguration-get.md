---
title: 获取 sharedPCConfiguration
description: 读取 sharedPCConfiguration 对象的属性和关系。
ms.openlocfilehash: d0b7350441afd582b64bb2854056f2f0fcdee1b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008649"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="2f343-103">获取 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f343-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="2f343-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2f343-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f343-105">读取 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f343-105">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f343-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f343-106">Prerequisites</span></span>
<span data-ttu-id="2f343-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2f343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f343-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f343-109">Permission type</span></span>|<span data-ttu-id="2f343-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f343-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f343-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f343-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f343-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f343-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2f343-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f343-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f343-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f343-114">Not supported.</span></span>|
|<span data-ttu-id="2f343-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f343-115">Application</span></span>|<span data-ttu-id="2f343-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f343-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f343-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f343-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f343-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2f343-118">Optional query parameters</span></span>
<span data-ttu-id="2f343-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2f343-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2f343-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f343-120">Request headers</span></span>
|<span data-ttu-id="2f343-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f343-121">Header</span></span>|<span data-ttu-id="2f343-122">值</span><span class="sxs-lookup"><span data-stu-id="2f343-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f343-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f343-123">Authorization</span></span>|<span data-ttu-id="2f343-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f343-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f343-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f343-125">Accept</span></span>|<span data-ttu-id="2f343-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f343-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f343-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f343-127">Request body</span></span>
<span data-ttu-id="2f343-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f343-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f343-129">响应</span><span class="sxs-lookup"><span data-stu-id="2f343-129">Response</span></span>
<span data-ttu-id="2f343-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f343-130">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f343-131">示例</span><span class="sxs-lookup"><span data-stu-id="2f343-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f343-132">请求</span><span class="sxs-lookup"><span data-stu-id="2f343-132">Request</span></span>
<span data-ttu-id="2f343-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f343-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2f343-134">响应</span><span class="sxs-lookup"><span data-stu-id="2f343-134">Response</span></span>
<span data-ttu-id="2f343-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f343-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedPCConfiguration",
    "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountManagerPolicy": {
      "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
      "accountDeletionPolicy": "diskSpaceThreshold",
      "cacheAccountsAboveDiskFreePercentage": 4,
      "inactiveThresholdDays": 5,
      "removeAccountsBelowDiskFreePercentage": 5
    },
    "allowedAccounts": "domain",
    "allowLocalStorage": true,
    "disableAccountManager": true,
    "disableEduPolicies": true,
    "disablePowerPolicies": true,
    "disableSignInOnResume": true,
    "enabled": true,
    "idleTimeBeforeSleepInSeconds": 12,
    "kioskAppDisplayName": "Kiosk App Display Name value",
    "kioskAppUserModelId": "Kiosk App User Model Id value",
    "maintenanceStartTime": "11:59:24.7240000"
  }
}
```



