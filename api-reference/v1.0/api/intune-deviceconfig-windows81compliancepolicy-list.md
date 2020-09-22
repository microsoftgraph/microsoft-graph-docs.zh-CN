---
title: 列出 windows81CompliancePolicies
description: 列出 windows81CompliancePolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e133b2c7cd1ef5193b29df29de9c6914ef959f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063301"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="1328e-103">列出 windows81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="1328e-103">List windows81CompliancePolicies</span></span>

<span data-ttu-id="1328e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1328e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1328e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1328e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1328e-106">列出 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1328e-106">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1328e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1328e-107">Prerequisites</span></span>
<span data-ttu-id="1328e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1328e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1328e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1328e-110">Permission type</span></span>|<span data-ttu-id="1328e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1328e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1328e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1328e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1328e-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1328e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1328e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1328e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1328e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1328e-115">Not supported.</span></span>|
|<span data-ttu-id="1328e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1328e-116">Application</span></span>|<span data-ttu-id="1328e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1328e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1328e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1328e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1328e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1328e-119">Request headers</span></span>
|<span data-ttu-id="1328e-120">标头</span><span class="sxs-lookup"><span data-stu-id="1328e-120">Header</span></span>|<span data-ttu-id="1328e-121">值</span><span class="sxs-lookup"><span data-stu-id="1328e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1328e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1328e-122">Authorization</span></span>|<span data-ttu-id="1328e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1328e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1328e-124">接受</span><span class="sxs-lookup"><span data-stu-id="1328e-124">Accept</span></span>|<span data-ttu-id="1328e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1328e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1328e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1328e-126">Request body</span></span>
<span data-ttu-id="1328e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1328e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1328e-128">响应</span><span class="sxs-lookup"><span data-stu-id="1328e-128">Response</span></span>
<span data-ttu-id="1328e-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1328e-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1328e-130">示例</span><span class="sxs-lookup"><span data-stu-id="1328e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1328e-131">请求</span><span class="sxs-lookup"><span data-stu-id="1328e-131">Request</span></span>
<span data-ttu-id="1328e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1328e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="1328e-133">响应</span><span class="sxs-lookup"><span data-stu-id="1328e-133">Response</span></span>
<span data-ttu-id="1328e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1328e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": [
    {
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
  ]
}
```









