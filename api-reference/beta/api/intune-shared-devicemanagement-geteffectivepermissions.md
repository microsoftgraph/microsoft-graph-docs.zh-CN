---
title: getEffectivePermissions 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04988c6ab4163021098da609782d7ac8e755af83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527061"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="03a6d-103">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="03a6d-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="03a6d-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03a6d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03a6d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03a6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03a6d-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03a6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03a6d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03a6d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03a6d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03a6d-108">Prerequisites</span></span>
<span data-ttu-id="03a6d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03a6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03a6d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03a6d-111">Permission type</span></span>|<span data-ttu-id="03a6d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03a6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03a6d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03a6d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="03a6d-114">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="03a6d-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="03a6d-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="03a6d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="03a6d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03a6d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03a6d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="03a6d-117">Not supported.</span></span>|
|<span data-ttu-id="03a6d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="03a6d-118">Application</span></span>|<span data-ttu-id="03a6d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="03a6d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03a6d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03a6d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="03a6d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="03a6d-121">Request headers</span></span>
|<span data-ttu-id="03a6d-122">标头</span><span class="sxs-lookup"><span data-stu-id="03a6d-122">Header</span></span>|<span data-ttu-id="03a6d-123">值</span><span class="sxs-lookup"><span data-stu-id="03a6d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03a6d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="03a6d-124">Authorization</span></span>|<span data-ttu-id="03a6d-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03a6d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03a6d-126">接受</span><span class="sxs-lookup"><span data-stu-id="03a6d-126">Accept</span></span>|<span data-ttu-id="03a6d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="03a6d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03a6d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="03a6d-128">Request body</span></span>
<span data-ttu-id="03a6d-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="03a6d-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="03a6d-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="03a6d-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="03a6d-131">属性</span><span class="sxs-lookup"><span data-stu-id="03a6d-131">Property</span></span>|<span data-ttu-id="03a6d-132">类型</span><span class="sxs-lookup"><span data-stu-id="03a6d-132">Type</span></span>|<span data-ttu-id="03a6d-133">说明</span><span class="sxs-lookup"><span data-stu-id="03a6d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a6d-134">scope</span><span class="sxs-lookup"><span data-stu-id="03a6d-134">scope</span></span>|<span data-ttu-id="03a6d-135">String</span><span class="sxs-lookup"><span data-stu-id="03a6d-135">String</span></span>|<span data-ttu-id="03a6d-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03a6d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="03a6d-137">响应</span><span class="sxs-lookup"><span data-stu-id="03a6d-137">Response</span></span>
<span data-ttu-id="03a6d-138">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune-rbac-rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="03a6d-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03a6d-139">示例</span><span class="sxs-lookup"><span data-stu-id="03a6d-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="03a6d-140">请求</span><span class="sxs-lookup"><span data-stu-id="03a6d-140">Request</span></span>
<span data-ttu-id="03a6d-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03a6d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="03a6d-142">响应</span><span class="sxs-lookup"><span data-stu-id="03a6d-142">Response</span></span>
<span data-ttu-id="03a6d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03a6d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```



