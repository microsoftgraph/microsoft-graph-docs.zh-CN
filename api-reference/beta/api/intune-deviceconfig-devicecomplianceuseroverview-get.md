---
title: 获取 deviceComplianceUserOverview
description: 读取 deviceComplianceUserOverview 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 38eccb78c8f40e356a41de3f54a411294ac6c321
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327515"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="b1525-103">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="b1525-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="b1525-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1525-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1525-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1525-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1525-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b1525-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1525-107">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1525-107">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1525-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1525-108">Prerequisites</span></span>
<span data-ttu-id="b1525-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b1525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1525-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1525-111">Permission type</span></span>|<span data-ttu-id="b1525-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1525-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1525-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1525-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1525-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1525-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b1525-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1525-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1525-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1525-116">Not supported.</span></span>|
|<span data-ttu-id="b1525-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1525-117">Application</span></span>|<span data-ttu-id="b1525-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1525-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1525-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1525-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1525-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b1525-120">Optional query parameters</span></span>
<span data-ttu-id="b1525-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b1525-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1525-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1525-122">Request headers</span></span>
|<span data-ttu-id="b1525-123">标头</span><span class="sxs-lookup"><span data-stu-id="b1525-123">Header</span></span>|<span data-ttu-id="b1525-124">值</span><span class="sxs-lookup"><span data-stu-id="b1525-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1525-125">授权</span><span class="sxs-lookup"><span data-stu-id="b1525-125">Authorization</span></span>|<span data-ttu-id="b1525-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1525-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1525-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b1525-127">Accept</span></span>|<span data-ttu-id="b1525-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b1525-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1525-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1525-129">Request body</span></span>
<span data-ttu-id="b1525-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1525-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1525-131">响应</span><span class="sxs-lookup"><span data-stu-id="b1525-131">Response</span></span>
<span data-ttu-id="b1525-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1525-132">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1525-133">示例</span><span class="sxs-lookup"><span data-stu-id="b1525-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1525-134">请求</span><span class="sxs-lookup"><span data-stu-id="b1525-134">Request</span></span>
<span data-ttu-id="b1525-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1525-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="b1525-136">响应</span><span class="sxs-lookup"><span data-stu-id="b1525-136">Response</span></span>
<span data-ttu-id="b1525-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1525-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
    "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





