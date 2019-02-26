---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a1da65f013bfc94a28625c398c5cdf070ae0c77
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260107"
---
# <a name="assign-action"></a><span data-ttu-id="6f76d-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="6f76d-103">assign action</span></span>

> <span data-ttu-id="6f76d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f76d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f76d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6f76d-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f76d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f76d-106">Prerequisites</span></span>
<span data-ttu-id="6f76d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6f76d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f76d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f76d-109">Permission type</span></span>|<span data-ttu-id="6f76d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f76d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f76d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f76d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f76d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f76d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f76d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f76d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f76d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f76d-114">Not supported.</span></span>|
|<span data-ttu-id="6f76d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f76d-115">Application</span></span>|<span data-ttu-id="6f76d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f76d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f76d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f76d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="6f76d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f76d-118">Request headers</span></span>
|<span data-ttu-id="6f76d-119">标头</span><span class="sxs-lookup"><span data-stu-id="6f76d-119">Header</span></span>|<span data-ttu-id="6f76d-120">值</span><span class="sxs-lookup"><span data-stu-id="6f76d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f76d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f76d-121">Authorization</span></span>|<span data-ttu-id="6f76d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f76d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f76d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6f76d-123">Accept</span></span>|<span data-ttu-id="6f76d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f76d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f76d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f76d-125">Request body</span></span>
<span data-ttu-id="6f76d-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f76d-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6f76d-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6f76d-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6f76d-128">属性</span><span class="sxs-lookup"><span data-stu-id="6f76d-128">Property</span></span>|<span data-ttu-id="6f76d-129">类型</span><span class="sxs-lookup"><span data-stu-id="6f76d-129">Type</span></span>|<span data-ttu-id="6f76d-130">说明</span><span class="sxs-lookup"><span data-stu-id="6f76d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f76d-131">assignments</span><span class="sxs-lookup"><span data-stu-id="6f76d-131">assignments</span></span>|<span data-ttu-id="6f76d-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f76d-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="6f76d-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6f76d-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f76d-134">响应</span><span class="sxs-lookup"><span data-stu-id="6f76d-134">Response</span></span>
<span data-ttu-id="6f76d-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6f76d-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6f76d-136">示例</span><span class="sxs-lookup"><span data-stu-id="6f76d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f76d-137">请求</span><span class="sxs-lookup"><span data-stu-id="6f76d-137">Request</span></span>
<span data-ttu-id="6f76d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f76d-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6f76d-139">响应</span><span class="sxs-lookup"><span data-stu-id="6f76d-139">Response</span></span>
<span data-ttu-id="6f76d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f76d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



