---
title: 列出 deviceComplianceUserStatuses
description: 列出 deviceComplianceUserStatus 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb1820e79c940e78a02b9ac5510f935b460f975d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786600"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="ade56-103">列出 deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="ade56-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="ade56-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ade56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ade56-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ade56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ade56-106">列出 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ade56-106">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ade56-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ade56-107">Prerequisites</span></span>
<span data-ttu-id="ade56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ade56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ade56-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ade56-110">Permission type</span></span>|<span data-ttu-id="ade56-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ade56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ade56-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ade56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ade56-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ade56-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ade56-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ade56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ade56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ade56-115">Not supported.</span></span>|
|<span data-ttu-id="ade56-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ade56-116">Application</span></span>|<span data-ttu-id="ade56-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ade56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ade56-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ade56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ade56-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ade56-119">Request headers</span></span>
|<span data-ttu-id="ade56-120">标头</span><span class="sxs-lookup"><span data-stu-id="ade56-120">Header</span></span>|<span data-ttu-id="ade56-121">值</span><span class="sxs-lookup"><span data-stu-id="ade56-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ade56-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade56-122">Authorization</span></span>|<span data-ttu-id="ade56-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ade56-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ade56-124">接受</span><span class="sxs-lookup"><span data-stu-id="ade56-124">Accept</span></span>|<span data-ttu-id="ade56-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ade56-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ade56-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ade56-126">Request body</span></span>
<span data-ttu-id="ade56-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ade56-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ade56-128">响应</span><span class="sxs-lookup"><span data-stu-id="ade56-128">Response</span></span>
<span data-ttu-id="ade56-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ade56-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ade56-130">示例</span><span class="sxs-lookup"><span data-stu-id="ade56-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ade56-131">请求</span><span class="sxs-lookup"><span data-stu-id="ade56-131">Request</span></span>
<span data-ttu-id="ade56-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ade56-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="ade56-133">响应</span><span class="sxs-lookup"><span data-stu-id="ade56-133">Response</span></span>
<span data-ttu-id="ade56-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ade56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





