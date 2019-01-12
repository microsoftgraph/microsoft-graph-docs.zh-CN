---
title: 获取 restrictedAppsViolation
description: 读取属性和 restrictedAppsViolation 对象的关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0dd407e71f0ed777bceb1e8711df522230961ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950317"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="bf50d-103">获取 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="bf50d-103">Get restrictedAppsViolation</span></span>

> <span data-ttu-id="bf50d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf50d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf50d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf50d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf50d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bf50d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf50d-107">读取属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="bf50d-107">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf50d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf50d-108">Prerequisites</span></span>
<span data-ttu-id="bf50d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bf50d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf50d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf50d-111">Permission type</span></span>|<span data-ttu-id="bf50d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf50d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf50d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf50d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf50d-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf50d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bf50d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf50d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf50d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf50d-116">Not supported.</span></span>|
|<span data-ttu-id="bf50d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf50d-117">Application</span></span>|<span data-ttu-id="bf50d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf50d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf50d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf50d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf50d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bf50d-120">Optional query parameters</span></span>
<span data-ttu-id="bf50d-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bf50d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bf50d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf50d-122">Request headers</span></span>
|<span data-ttu-id="bf50d-123">标头</span><span class="sxs-lookup"><span data-stu-id="bf50d-123">Header</span></span>|<span data-ttu-id="bf50d-124">值</span><span class="sxs-lookup"><span data-stu-id="bf50d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf50d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf50d-125">Authorization</span></span>|<span data-ttu-id="bf50d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf50d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf50d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bf50d-127">Accept</span></span>|<span data-ttu-id="bf50d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bf50d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf50d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf50d-129">Request body</span></span>
<span data-ttu-id="bf50d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf50d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf50d-131">响应</span><span class="sxs-lookup"><span data-stu-id="bf50d-131">Response</span></span>
<span data-ttu-id="bf50d-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf50d-132">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf50d-133">示例</span><span class="sxs-lookup"><span data-stu-id="bf50d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf50d-134">请求</span><span class="sxs-lookup"><span data-stu-id="bf50d-134">Request</span></span>
<span data-ttu-id="bf50d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf50d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="bf50d-136">响应</span><span class="sxs-lookup"><span data-stu-id="bf50d-136">Response</span></span>
<span data-ttu-id="bf50d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf50d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 664

{
  "value": {
    "@odata.type": "#microsoft.graph.restrictedAppsViolation",
    "id": "53f99903-9903-53f9-0399-f9530399f953",
    "userId": "User Id value",
    "userName": "User Name value",
    "managedDeviceId": "Managed Device Id value",
    "deviceName": "Device Name value",
    "deviceConfigurationId": "Device Configuration Id value",
    "deviceConfigurationName": "Device Configuration Name value",
    "platformType": "androidForWork",
    "restrictedAppsState": "notApprovedApps",
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.managedDeviceReportedApp",
        "appId": "App Id value"
      }
    ]
  }
}
```





