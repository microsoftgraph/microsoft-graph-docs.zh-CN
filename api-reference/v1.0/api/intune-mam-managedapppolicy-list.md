---
title: 列出 managedAppPolicies
description: 列出 managedAppPolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b82396e9001ff08337b4a4e6862e060e9e09b1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965951"
---
# <a name="list-managedapppolicies"></a><span data-ttu-id="2d8b7-103">列出 managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="2d8b7-103">List managedAppPolicies</span></span>

<span data-ttu-id="2d8b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d8b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d8b7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d8b7-106">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-106">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d8b7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d8b7-107">Prerequisites</span></span>
<span data-ttu-id="2d8b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d8b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d8b7-110">Permission type</span></span>|<span data-ttu-id="2d8b7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d8b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d8b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d8b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d8b7-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d8b7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2d8b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d8b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d8b7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-115">Not supported.</span></span>|
|<span data-ttu-id="2d8b7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d8b7-116">Application</span></span>|<span data-ttu-id="2d8b7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d8b7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d8b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2d8b7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d8b7-119">Request headers</span></span>
|<span data-ttu-id="2d8b7-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d8b7-120">Header</span></span>|<span data-ttu-id="2d8b7-121">值</span><span class="sxs-lookup"><span data-stu-id="2d8b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d8b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d8b7-122">Authorization</span></span>|<span data-ttu-id="2d8b7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d8b7-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d8b7-124">Accept</span></span>|<span data-ttu-id="2d8b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d8b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d8b7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d8b7-126">Request body</span></span>
<span data-ttu-id="2d8b7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d8b7-128">响应</span><span class="sxs-lookup"><span data-stu-id="2d8b7-128">Response</span></span>
<span data-ttu-id="2d8b7-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d8b7-130">示例</span><span class="sxs-lookup"><span data-stu-id="2d8b7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d8b7-131">请求</span><span class="sxs-lookup"><span data-stu-id="2d8b7-131">Request</span></span>
<span data-ttu-id="2d8b7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="2d8b7-133">响应</span><span class="sxs-lookup"><span data-stu-id="2d8b7-133">Response</span></span>
<span data-ttu-id="2d8b7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d8b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```









