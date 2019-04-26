---
title: getEffectivePermissions 函数
description: 检索当前验证的用户的有效权限
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d6c58ae88e2b5cf9a6787529868f8cf9e42879be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576956"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="7b8a2-103">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="7b8a2-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="7b8a2-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b8a2-105">检索当前验证的用户的有效权限</span><span class="sxs-lookup"><span data-stu-id="7b8a2-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b8a2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b8a2-106">Prerequisites</span></span>
<span data-ttu-id="7b8a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b8a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b8a2-109">Permission type</span></span>|<span data-ttu-id="7b8a2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b8a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b8a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b8a2-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7b8a2-112">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="7b8a2-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="7b8a2-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b8a2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7b8a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b8a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b8a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-115">Not supported.</span></span>|
|<span data-ttu-id="7b8a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b8a2-116">Application</span></span>|<span data-ttu-id="7b8a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b8a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b8a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="7b8a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b8a2-119">Request headers</span></span>
|<span data-ttu-id="7b8a2-120">标头</span><span class="sxs-lookup"><span data-stu-id="7b8a2-120">Header</span></span>|<span data-ttu-id="7b8a2-121">值</span><span class="sxs-lookup"><span data-stu-id="7b8a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b8a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b8a2-122">Authorization</span></span>|<span data-ttu-id="7b8a2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b8a2-124">接受</span><span class="sxs-lookup"><span data-stu-id="7b8a2-124">Accept</span></span>|<span data-ttu-id="7b8a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b8a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b8a2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b8a2-126">Request body</span></span>
<span data-ttu-id="7b8a2-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7b8a2-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7b8a2-129">属性</span><span class="sxs-lookup"><span data-stu-id="7b8a2-129">Property</span></span>|<span data-ttu-id="7b8a2-130">类型</span><span class="sxs-lookup"><span data-stu-id="7b8a2-130">Type</span></span>|<span data-ttu-id="7b8a2-131">说明</span><span class="sxs-lookup"><span data-stu-id="7b8a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b8a2-132">scope</span><span class="sxs-lookup"><span data-stu-id="7b8a2-132">scope</span></span>|<span data-ttu-id="7b8a2-133">String</span><span class="sxs-lookup"><span data-stu-id="7b8a2-133">String</span></span>|<span data-ttu-id="7b8a2-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7b8a2-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="7b8a2-135">响应</span><span class="sxs-lookup"><span data-stu-id="7b8a2-135">Response</span></span>
<span data-ttu-id="7b8a2-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune-rbac-rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b8a2-137">示例</span><span class="sxs-lookup"><span data-stu-id="7b8a2-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b8a2-138">请求</span><span class="sxs-lookup"><span data-stu-id="7b8a2-138">Request</span></span>
<span data-ttu-id="7b8a2-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7b8a2-140">响应</span><span class="sxs-lookup"><span data-stu-id="7b8a2-140">Response</span></span>
<span data-ttu-id="7b8a2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b8a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



