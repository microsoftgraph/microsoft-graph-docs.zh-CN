---
title: 获取 mobileAppIntentAndState
description: 读取属性和 mobileAppIntentAndState 对象的关系。
ms.openlocfilehash: 837165f713aea00061b721a41003adc479a46b4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044034"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="00c75-103">获取 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="00c75-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="00c75-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00c75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00c75-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00c75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00c75-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00c75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00c75-107">读取属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="00c75-107">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00c75-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="00c75-108">Prerequisites</span></span>
<span data-ttu-id="00c75-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="00c75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00c75-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="00c75-111">Permission type</span></span>|<span data-ttu-id="00c75-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="00c75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00c75-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00c75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00c75-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="00c75-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="00c75-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00c75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00c75-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="00c75-116">Not supported.</span></span>|
|<span data-ttu-id="00c75-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="00c75-117">Application</span></span>|<span data-ttu-id="00c75-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="00c75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00c75-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00c75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00c75-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="00c75-120">Optional query parameters</span></span>
<span data-ttu-id="00c75-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="00c75-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00c75-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="00c75-122">Request headers</span></span>
|<span data-ttu-id="00c75-123">标头</span><span class="sxs-lookup"><span data-stu-id="00c75-123">Header</span></span>|<span data-ttu-id="00c75-124">值</span><span class="sxs-lookup"><span data-stu-id="00c75-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00c75-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="00c75-125">Authorization</span></span>|<span data-ttu-id="00c75-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00c75-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00c75-127">Accept</span><span class="sxs-lookup"><span data-stu-id="00c75-127">Accept</span></span>|<span data-ttu-id="00c75-128">application/json</span><span class="sxs-lookup"><span data-stu-id="00c75-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00c75-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="00c75-129">Request body</span></span>
<span data-ttu-id="00c75-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="00c75-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00c75-131">响应</span><span class="sxs-lookup"><span data-stu-id="00c75-131">Response</span></span>
<span data-ttu-id="00c75-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00c75-132">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00c75-133">示例</span><span class="sxs-lookup"><span data-stu-id="00c75-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="00c75-134">请求</span><span class="sxs-lookup"><span data-stu-id="00c75-134">Request</span></span>
<span data-ttu-id="00c75-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00c75-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="00c75-136">响应</span><span class="sxs-lookup"><span data-stu-id="00c75-136">Response</span></span>
<span data-ttu-id="00c75-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00c75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 943

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
    "id": "45a775d6-75d6-45a7-d675-a745d675a745",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "mobileAppList": [
      {
        "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
        "applicationId": "Application Id value",
        "displayName": "Display Name value",
        "mobileAppIntent": "notAvailable",
        "displayVersion": "Display Version value",
        "installState": "failed",
        "supportedDeviceTypes": [
          {
            "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
            "type": "windowsRT",
            "minimumOperatingSystemVersion": "Minimum Operating System Version value",
            "maximumOperatingSystemVersion": "Maximum Operating System Version value"
          }
        ]
      }
    ]
  }
}
```





