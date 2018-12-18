---
title: 获取 windows81CompliancePolicy
description: 读取 windows81CompliancePolicy 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: a156ec9d40d3e952b635a8a0dccbf2e46a4001d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301202"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="a4e9d-103">获取 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a4e9d-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="a4e9d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4e9d-105">读取 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-105">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4e9d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4e9d-106">Prerequisites</span></span>
<span data-ttu-id="a4e9d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a4e9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e9d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4e9d-109">Permission type</span></span>|<span data-ttu-id="a4e9d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4e9d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4e9d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4e9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4e9d-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4e9d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a4e9d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4e9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4e9d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-114">Not supported.</span></span>|
|<span data-ttu-id="a4e9d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4e9d-115">Application</span></span>|<span data-ttu-id="a4e9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4e9d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4e9d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4e9d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4e9d-118">Optional query parameters</span></span>
<span data-ttu-id="a4e9d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a4e9d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4e9d-120">Request headers</span></span>
|<span data-ttu-id="a4e9d-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4e9d-121">Header</span></span>|<span data-ttu-id="a4e9d-122">值</span><span class="sxs-lookup"><span data-stu-id="a4e9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4e9d-123">授权</span><span class="sxs-lookup"><span data-stu-id="a4e9d-123">Authorization</span></span>|<span data-ttu-id="a4e9d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4e9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4e9d-125">Accept</span></span>|<span data-ttu-id="a4e9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4e9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4e9d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4e9d-127">Request body</span></span>
<span data-ttu-id="a4e9d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4e9d-129">响应</span><span class="sxs-lookup"><span data-stu-id="a4e9d-129">Response</span></span>
<span data-ttu-id="a4e9d-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-130">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4e9d-131">示例</span><span class="sxs-lookup"><span data-stu-id="a4e9d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4e9d-132">请求</span><span class="sxs-lookup"><span data-stu-id="a4e9d-132">Request</span></span>
<span data-ttu-id="a4e9d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a4e9d-134">响应</span><span class="sxs-lookup"><span data-stu-id="a4e9d-134">Response</span></span>
<span data-ttu-id="a4e9d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4e9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
    "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```



