---
title: assign 操作
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 70d66bfda498c6fbfa7065e0d35006563567bb08
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362697"
---
# <a name="assign-action"></a><span data-ttu-id="5e589-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="5e589-103">assign action</span></span>

> <span data-ttu-id="5e589-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e589-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e589-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e589-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e589-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5e589-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e589-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5e589-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e589-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e589-108">Prerequisites</span></span>
<span data-ttu-id="5e589-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5e589-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e589-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e589-111">Permission type</span></span>|<span data-ttu-id="5e589-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e589-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e589-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e589-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e589-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e589-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e589-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e589-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e589-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e589-116">Not supported.</span></span>|
|<span data-ttu-id="5e589-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e589-117">Application</span></span>|<span data-ttu-id="5e589-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e589-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e589-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e589-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5e589-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e589-120">Request headers</span></span>
|<span data-ttu-id="5e589-121">标头</span><span class="sxs-lookup"><span data-stu-id="5e589-121">Header</span></span>|<span data-ttu-id="5e589-122">值</span><span class="sxs-lookup"><span data-stu-id="5e589-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e589-123">授权</span><span class="sxs-lookup"><span data-stu-id="5e589-123">Authorization</span></span>|<span data-ttu-id="5e589-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e589-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e589-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e589-125">Accept</span></span>|<span data-ttu-id="5e589-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e589-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e589-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e589-127">Request body</span></span>
<span data-ttu-id="5e589-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e589-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5e589-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5e589-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5e589-130">属性</span><span class="sxs-lookup"><span data-stu-id="5e589-130">Property</span></span>|<span data-ttu-id="5e589-131">类型</span><span class="sxs-lookup"><span data-stu-id="5e589-131">Type</span></span>|<span data-ttu-id="5e589-132">说明</span><span class="sxs-lookup"><span data-stu-id="5e589-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e589-133">assignments</span><span class="sxs-lookup"><span data-stu-id="5e589-133">assignments</span></span>|<span data-ttu-id="5e589-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e589-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="5e589-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5e589-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5e589-136">响应</span><span class="sxs-lookup"><span data-stu-id="5e589-136">Response</span></span>
<span data-ttu-id="5e589-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e589-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e589-138">示例</span><span class="sxs-lookup"><span data-stu-id="5e589-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e589-139">请求</span><span class="sxs-lookup"><span data-stu-id="5e589-139">Request</span></span>
<span data-ttu-id="5e589-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e589-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="5e589-141">响应</span><span class="sxs-lookup"><span data-stu-id="5e589-141">Response</span></span>
<span data-ttu-id="5e589-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e589-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





