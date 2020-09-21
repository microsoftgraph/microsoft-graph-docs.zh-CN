---
title: targetApps 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d68d46eb78c34a73acb4f0a9b0759c5fcddaacd8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965944"
---
# <a name="targetapps-action"></a><span data-ttu-id="43c4c-103">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="43c4c-103">targetApps action</span></span>

<span data-ttu-id="43c4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43c4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43c4c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43c4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c4c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43c4c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43c4c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="43c4c-107">Prerequisites</span></span>
<span data-ttu-id="43c4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c4c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="43c4c-110">Permission type</span></span>|<span data-ttu-id="43c4c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43c4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43c4c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43c4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43c4c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c4c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43c4c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43c4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43c4c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43c4c-115">Not supported.</span></span>|
|<span data-ttu-id="43c4c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="43c4c-116">Application</span></span>|<span data-ttu-id="43c4c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="43c4c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43c4c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43c4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="43c4c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="43c4c-119">Request headers</span></span>
|<span data-ttu-id="43c4c-120">标头</span><span class="sxs-lookup"><span data-stu-id="43c4c-120">Header</span></span>|<span data-ttu-id="43c4c-121">值</span><span class="sxs-lookup"><span data-stu-id="43c4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43c4c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c4c-122">Authorization</span></span>|<span data-ttu-id="43c4c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43c4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43c4c-124">接受</span><span class="sxs-lookup"><span data-stu-id="43c4c-124">Accept</span></span>|<span data-ttu-id="43c4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43c4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c4c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="43c4c-126">Request body</span></span>
<span data-ttu-id="43c4c-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43c4c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43c4c-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="43c4c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43c4c-129">属性</span><span class="sxs-lookup"><span data-stu-id="43c4c-129">Property</span></span>|<span data-ttu-id="43c4c-130">类型</span><span class="sxs-lookup"><span data-stu-id="43c4c-130">Type</span></span>|<span data-ttu-id="43c4c-131">说明</span><span class="sxs-lookup"><span data-stu-id="43c4c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43c4c-132">apps</span><span class="sxs-lookup"><span data-stu-id="43c4c-132">apps</span></span>|<span data-ttu-id="43c4c-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43c4c-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="43c4c-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43c4c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43c4c-135">响应</span><span class="sxs-lookup"><span data-stu-id="43c4c-135">Response</span></span>
<span data-ttu-id="43c4c-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="43c4c-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43c4c-137">示例</span><span class="sxs-lookup"><span data-stu-id="43c4c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c4c-138">请求</span><span class="sxs-lookup"><span data-stu-id="43c4c-138">Request</span></span>
<span data-ttu-id="43c4c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43c4c-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="43c4c-140">响应</span><span class="sxs-lookup"><span data-stu-id="43c4c-140">Response</span></span>
<span data-ttu-id="43c4c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43c4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









