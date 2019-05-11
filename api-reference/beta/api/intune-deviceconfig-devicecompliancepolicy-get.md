---
title: 获取 deviceCompliancePolicy
description: 读取 deviceCompliancePolicy 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47d61c5ccb64b55682d847626c6e4b72978a32af
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927851"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="cff94-103">获取 deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cff94-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="cff94-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cff94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cff94-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cff94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cff94-106">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cff94-106">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cff94-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cff94-107">Prerequisites</span></span>
<span data-ttu-id="cff94-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cff94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cff94-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cff94-110">Permission type</span></span>|<span data-ttu-id="cff94-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cff94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff94-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cff94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cff94-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cff94-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cff94-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cff94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff94-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff94-115">Not supported.</span></span>|
|<span data-ttu-id="cff94-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cff94-116">Application</span></span>|<span data-ttu-id="cff94-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff94-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cff94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cff94-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cff94-119">Optional query parameters</span></span>
<span data-ttu-id="cff94-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cff94-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cff94-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cff94-121">Request headers</span></span>
|<span data-ttu-id="cff94-122">标头</span><span class="sxs-lookup"><span data-stu-id="cff94-122">Header</span></span>|<span data-ttu-id="cff94-123">值</span><span class="sxs-lookup"><span data-stu-id="cff94-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff94-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cff94-124">Authorization</span></span>|<span data-ttu-id="cff94-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cff94-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cff94-126">接受</span><span class="sxs-lookup"><span data-stu-id="cff94-126">Accept</span></span>|<span data-ttu-id="cff94-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cff94-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff94-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cff94-128">Request body</span></span>
<span data-ttu-id="cff94-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cff94-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cff94-130">响应</span><span class="sxs-lookup"><span data-stu-id="cff94-130">Response</span></span>
<span data-ttu-id="cff94-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cff94-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff94-132">示例</span><span class="sxs-lookup"><span data-stu-id="cff94-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cff94-133">请求</span><span class="sxs-lookup"><span data-stu-id="cff94-133">Request</span></span>
<span data-ttu-id="cff94-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cff94-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="cff94-135">响应</span><span class="sxs-lookup"><span data-stu-id="cff94-135">Response</span></span>
<span data-ttu-id="cff94-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cff94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4214b716-b716-4214-16b7-144216b71442",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




