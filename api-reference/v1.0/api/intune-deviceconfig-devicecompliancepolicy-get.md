---
title: 获取 deviceCompliancePolicy
description: 读取 deviceCompliancePolicy 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e3722dd926972d43c98b862cce1c34c5a68db6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969672"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="2df7d-103">获取 deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2df7d-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="2df7d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2df7d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df7d-105">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2df7d-105">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df7d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2df7d-106">Prerequisites</span></span>
<span data-ttu-id="2df7d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2df7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df7d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2df7d-109">Permission type</span></span>|<span data-ttu-id="2df7d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2df7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df7d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2df7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2df7d-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df7d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2df7d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2df7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df7d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df7d-114">Not supported.</span></span>|
|<span data-ttu-id="2df7d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2df7d-115">Application</span></span>|<span data-ttu-id="2df7d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df7d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2df7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2df7d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2df7d-118">Optional query parameters</span></span>
<span data-ttu-id="2df7d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2df7d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2df7d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2df7d-120">Request headers</span></span>
|<span data-ttu-id="2df7d-121">标头</span><span class="sxs-lookup"><span data-stu-id="2df7d-121">Header</span></span>|<span data-ttu-id="2df7d-122">值</span><span class="sxs-lookup"><span data-stu-id="2df7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df7d-123">Authorization</span></span>|<span data-ttu-id="2df7d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2df7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df7d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2df7d-125">Accept</span></span>|<span data-ttu-id="2df7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2df7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df7d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2df7d-127">Request body</span></span>
<span data-ttu-id="2df7d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2df7d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df7d-129">响应</span><span class="sxs-lookup"><span data-stu-id="2df7d-129">Response</span></span>
<span data-ttu-id="2df7d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2df7d-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df7d-131">示例</span><span class="sxs-lookup"><span data-stu-id="2df7d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df7d-132">请求</span><span class="sxs-lookup"><span data-stu-id="2df7d-132">Request</span></span>
<span data-ttu-id="2df7d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2df7d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="2df7d-134">响应</span><span class="sxs-lookup"><span data-stu-id="2df7d-134">Response</span></span>
<span data-ttu-id="2df7d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2df7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
    "id": "4214b716-b716-4214-16b7-144216b71442",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



