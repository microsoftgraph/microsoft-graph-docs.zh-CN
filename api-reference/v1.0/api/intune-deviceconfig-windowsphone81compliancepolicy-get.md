---
title: 获取 windowsPhone81CompliancePolicy
description: 读取 windowsPhone81CompliancePolicy 对象的属性和关系。
ms.openlocfilehash: f5135af0bd1e304c569098bde86999933728f769
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009383"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="ffc80-103">获取 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ffc80-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="ffc80-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ffc80-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffc80-105">读取 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffc80-105">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffc80-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffc80-106">Prerequisites</span></span>
<span data-ttu-id="ffc80-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ffc80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffc80-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffc80-109">Permission type</span></span>|<span data-ttu-id="ffc80-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffc80-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffc80-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffc80-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffc80-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ffc80-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc80-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffc80-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffc80-114">Not supported.</span></span>|
|<span data-ttu-id="ffc80-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffc80-115">Application</span></span>|<span data-ttu-id="ffc80-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffc80-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffc80-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffc80-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffc80-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ffc80-118">Optional query parameters</span></span>
<span data-ttu-id="ffc80-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ffc80-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffc80-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffc80-120">Request headers</span></span>
|<span data-ttu-id="ffc80-121">标头</span><span class="sxs-lookup"><span data-stu-id="ffc80-121">Header</span></span>|<span data-ttu-id="ffc80-122">值</span><span class="sxs-lookup"><span data-stu-id="ffc80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffc80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffc80-123">Authorization</span></span>|<span data-ttu-id="ffc80-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffc80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffc80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffc80-125">Accept</span></span>|<span data-ttu-id="ffc80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffc80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffc80-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffc80-127">Request body</span></span>
<span data-ttu-id="ffc80-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffc80-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffc80-129">响应</span><span class="sxs-lookup"><span data-stu-id="ffc80-129">Response</span></span>
<span data-ttu-id="ffc80-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffc80-130">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffc80-131">示例</span><span class="sxs-lookup"><span data-stu-id="ffc80-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffc80-132">请求</span><span class="sxs-lookup"><span data-stu-id="ffc80-132">Request</span></span>
<span data-ttu-id="ffc80-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffc80-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ffc80-134">响应</span><span class="sxs-lookup"><span data-stu-id="ffc80-134">Response</span></span>
<span data-ttu-id="ffc80-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffc80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```



