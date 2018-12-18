---
title: 获取 iosUpdateDeviceStatus
description: 读取 iosUpdateDeviceStatus 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: e49af975fc6eed33d5b0de506927f3eca4e4741e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332996"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="8c068-103">获取 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8c068-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="8c068-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8c068-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c068-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8c068-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c068-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c068-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c068-107">读取 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8c068-107">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c068-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c068-108">Prerequisites</span></span>
<span data-ttu-id="8c068-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8c068-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c068-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c068-111">Permission type</span></span>|<span data-ttu-id="8c068-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c068-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c068-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c068-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c068-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8c068-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c068-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c068-116">Not supported.</span></span>|
|<span data-ttu-id="8c068-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c068-117">Application</span></span>|<span data-ttu-id="8c068-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c068-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c068-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c068-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c068-120">Optional query parameters</span></span>
<span data-ttu-id="8c068-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c068-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c068-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c068-122">Request headers</span></span>
|<span data-ttu-id="8c068-123">标头</span><span class="sxs-lookup"><span data-stu-id="8c068-123">Header</span></span>|<span data-ttu-id="8c068-124">值</span><span class="sxs-lookup"><span data-stu-id="8c068-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c068-125">授权</span><span class="sxs-lookup"><span data-stu-id="8c068-125">Authorization</span></span>|<span data-ttu-id="8c068-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c068-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c068-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8c068-127">Accept</span></span>|<span data-ttu-id="8c068-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8c068-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c068-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c068-129">Request body</span></span>
<span data-ttu-id="8c068-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c068-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c068-131">响应</span><span class="sxs-lookup"><span data-stu-id="8c068-131">Response</span></span>
<span data-ttu-id="8c068-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c068-132">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c068-133">示例</span><span class="sxs-lookup"><span data-stu-id="8c068-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c068-134">请求</span><span class="sxs-lookup"><span data-stu-id="8c068-134">Request</span></span>
<span data-ttu-id="8c068-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c068-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8c068-136">响应</span><span class="sxs-lookup"><span data-stu-id="8c068-136">Response</span></span>
<span data-ttu-id="8c068-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c068-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
    "id": "63a79499-9499-63a7-9994-a7639994a763",
    "installStatus": "available",
    "osVersion": "Os Version value",
    "deviceId": "Device Id value",
    "userId": "User Id value",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





