---
title: 获取 deviceComplianceDeviceStatus
description: 读取 deviceComplianceDeviceStatus 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f2ed86505d552e57dd7f83c09acae6c819dbf7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850965"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="890b1-103">获取 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="890b1-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="890b1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="890b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="890b1-105">读取 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="890b1-105">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="890b1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="890b1-106">Prerequisites</span></span>
<span data-ttu-id="890b1-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="890b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="890b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="890b1-109">Permission type</span></span>|<span data-ttu-id="890b1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="890b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="890b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="890b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="890b1-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="890b1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="890b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="890b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="890b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="890b1-114">Not supported.</span></span>|
|<span data-ttu-id="890b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="890b1-115">Application</span></span>|<span data-ttu-id="890b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="890b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="890b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="890b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="890b1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="890b1-118">Optional query parameters</span></span>
<span data-ttu-id="890b1-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="890b1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="890b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="890b1-120">Request headers</span></span>
|<span data-ttu-id="890b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="890b1-121">Header</span></span>|<span data-ttu-id="890b1-122">值</span><span class="sxs-lookup"><span data-stu-id="890b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="890b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="890b1-123">Authorization</span></span>|<span data-ttu-id="890b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="890b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="890b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="890b1-125">Accept</span></span>|<span data-ttu-id="890b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="890b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="890b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="890b1-127">Request body</span></span>
<span data-ttu-id="890b1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="890b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="890b1-129">响应</span><span class="sxs-lookup"><span data-stu-id="890b1-129">Response</span></span>
<span data-ttu-id="890b1-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="890b1-130">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="890b1-131">示例</span><span class="sxs-lookup"><span data-stu-id="890b1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="890b1-132">请求</span><span class="sxs-lookup"><span data-stu-id="890b1-132">Request</span></span>
<span data-ttu-id="890b1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="890b1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="890b1-134">响应</span><span class="sxs-lookup"><span data-stu-id="890b1-134">Response</span></span>
<span data-ttu-id="890b1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="890b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



