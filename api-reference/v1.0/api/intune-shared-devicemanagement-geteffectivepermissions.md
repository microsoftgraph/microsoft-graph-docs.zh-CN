---
title: getEffectivePermissions 函数
description: 检索当前验证的用户的有效权限
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d03ab6dd6633de58df090710e1ecae7bb216804
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512067"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="fcaa4-103">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="fcaa4-103">getEffectivePermissions function</span></span>

<span data-ttu-id="fcaa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcaa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcaa4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcaa4-106">检索当前验证的用户的有效权限</span><span class="sxs-lookup"><span data-stu-id="fcaa4-106">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcaa4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fcaa4-107">Prerequisites</span></span>
<span data-ttu-id="fcaa4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcaa4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fcaa4-110">Permission type</span></span>|<span data-ttu-id="fcaa4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fcaa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcaa4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fcaa4-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fcaa4-113">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="fcaa4-113">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="fcaa4-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcaa4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fcaa4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fcaa4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcaa4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-116">Not supported.</span></span>|
|<span data-ttu-id="fcaa4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fcaa4-117">Application</span></span>|<span data-ttu-id="fcaa4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcaa4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fcaa4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="fcaa4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fcaa4-120">Request headers</span></span>
|<span data-ttu-id="fcaa4-121">标头</span><span class="sxs-lookup"><span data-stu-id="fcaa4-121">Header</span></span>|<span data-ttu-id="fcaa4-122">值</span><span class="sxs-lookup"><span data-stu-id="fcaa4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcaa4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcaa4-123">Authorization</span></span>|<span data-ttu-id="fcaa4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcaa4-125">接受</span><span class="sxs-lookup"><span data-stu-id="fcaa4-125">Accept</span></span>|<span data-ttu-id="fcaa4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcaa4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcaa4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fcaa4-127">Request body</span></span>
<span data-ttu-id="fcaa4-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fcaa4-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fcaa4-130">属性</span><span class="sxs-lookup"><span data-stu-id="fcaa4-130">Property</span></span>|<span data-ttu-id="fcaa4-131">类型</span><span class="sxs-lookup"><span data-stu-id="fcaa4-131">Type</span></span>|<span data-ttu-id="fcaa4-132">说明</span><span class="sxs-lookup"><span data-stu-id="fcaa4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcaa4-133">scope</span><span class="sxs-lookup"><span data-stu-id="fcaa4-133">scope</span></span>|<span data-ttu-id="fcaa4-134">String</span><span class="sxs-lookup"><span data-stu-id="fcaa4-134">String</span></span>|<span data-ttu-id="fcaa4-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fcaa4-135">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="fcaa4-136">响应</span><span class="sxs-lookup"><span data-stu-id="fcaa4-136">Response</span></span>
<span data-ttu-id="fcaa4-137">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune-rbac-rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcaa4-138">示例</span><span class="sxs-lookup"><span data-stu-id="fcaa4-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcaa4-139">请求</span><span class="sxs-lookup"><span data-stu-id="fcaa4-139">Request</span></span>
<span data-ttu-id="fcaa4-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fcaa4-141">响应</span><span class="sxs-lookup"><span data-stu-id="fcaa4-141">Response</span></span>
<span data-ttu-id="fcaa4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fcaa4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




