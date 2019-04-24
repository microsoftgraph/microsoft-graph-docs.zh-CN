---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6186afa6e535f6089709572205b85015bb29d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453721"
---
# <a name="assign-action"></a><span data-ttu-id="e222f-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="e222f-103">assign action</span></span>

> <span data-ttu-id="e222f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e222f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e222f-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e222f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e222f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e222f-106">Prerequisites</span></span>
<span data-ttu-id="e222f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e222f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e222f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e222f-109">Permission type</span></span>|<span data-ttu-id="e222f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e222f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e222f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e222f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e222f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e222f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e222f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e222f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e222f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e222f-114">Not supported.</span></span>|
|<span data-ttu-id="e222f-115">Application</span><span class="sxs-lookup"><span data-stu-id="e222f-115">Application</span></span>|<span data-ttu-id="e222f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e222f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e222f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e222f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e222f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e222f-118">Request headers</span></span>
|<span data-ttu-id="e222f-119">标头</span><span class="sxs-lookup"><span data-stu-id="e222f-119">Header</span></span>|<span data-ttu-id="e222f-120">值</span><span class="sxs-lookup"><span data-stu-id="e222f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e222f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e222f-121">Authorization</span></span>|<span data-ttu-id="e222f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e222f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e222f-123">接受</span><span class="sxs-lookup"><span data-stu-id="e222f-123">Accept</span></span>|<span data-ttu-id="e222f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e222f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e222f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e222f-125">Request body</span></span>
<span data-ttu-id="e222f-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e222f-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e222f-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e222f-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e222f-128">属性</span><span class="sxs-lookup"><span data-stu-id="e222f-128">Property</span></span>|<span data-ttu-id="e222f-129">类型</span><span class="sxs-lookup"><span data-stu-id="e222f-129">Type</span></span>|<span data-ttu-id="e222f-130">描述</span><span class="sxs-lookup"><span data-stu-id="e222f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e222f-131">assignments</span><span class="sxs-lookup"><span data-stu-id="e222f-131">assignments</span></span>|<span data-ttu-id="e222f-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e222f-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e222f-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e222f-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e222f-134">响应</span><span class="sxs-lookup"><span data-stu-id="e222f-134">Response</span></span>
<span data-ttu-id="e222f-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e222f-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e222f-136">示例</span><span class="sxs-lookup"><span data-stu-id="e222f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="e222f-137">请求</span><span class="sxs-lookup"><span data-stu-id="e222f-137">Request</span></span>
<span data-ttu-id="e222f-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e222f-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e222f-139">响应</span><span class="sxs-lookup"><span data-stu-id="e222f-139">Response</span></span>
<span data-ttu-id="e222f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e222f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



