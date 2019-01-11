---
title: getEffectivePermissions 函数
description: 检索当前验证的用户的有效权限
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5c887aebdba69048ded387371ad2534ce4173668
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850776"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="41184-103">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="41184-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="41184-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41184-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41184-105">检索当前验证的用户的有效权限</span><span class="sxs-lookup"><span data-stu-id="41184-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41184-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="41184-106">Prerequisites</span></span>
<span data-ttu-id="41184-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="41184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41184-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="41184-109">Permission type</span></span>|<span data-ttu-id="41184-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41184-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41184-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41184-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="41184-112">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="41184-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="41184-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="41184-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="41184-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41184-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41184-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41184-115">Not supported.</span></span>|
|<span data-ttu-id="41184-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41184-116">Application</span></span>|<span data-ttu-id="41184-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41184-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41184-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41184-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="41184-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41184-119">Request headers</span></span>
|<span data-ttu-id="41184-120">标头</span><span class="sxs-lookup"><span data-stu-id="41184-120">Header</span></span>|<span data-ttu-id="41184-121">值</span><span class="sxs-lookup"><span data-stu-id="41184-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41184-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41184-122">Authorization</span></span>|<span data-ttu-id="41184-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41184-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41184-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41184-124">Accept</span></span>|<span data-ttu-id="41184-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41184-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41184-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41184-126">Request body</span></span>
<span data-ttu-id="41184-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="41184-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="41184-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="41184-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="41184-129">属性</span><span class="sxs-lookup"><span data-stu-id="41184-129">Property</span></span>|<span data-ttu-id="41184-130">类型</span><span class="sxs-lookup"><span data-stu-id="41184-130">Type</span></span>|<span data-ttu-id="41184-131">说明</span><span class="sxs-lookup"><span data-stu-id="41184-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41184-132">scope</span><span class="sxs-lookup"><span data-stu-id="41184-132">scope</span></span>|<span data-ttu-id="41184-133">字符串</span><span class="sxs-lookup"><span data-stu-id="41184-133">String</span></span>|<span data-ttu-id="41184-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="41184-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="41184-135">响应</span><span class="sxs-lookup"><span data-stu-id="41184-135">Response</span></span>
<span data-ttu-id="41184-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune-rbac-rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="41184-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41184-137">示例</span><span class="sxs-lookup"><span data-stu-id="41184-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="41184-138">请求</span><span class="sxs-lookup"><span data-stu-id="41184-138">Request</span></span>
<span data-ttu-id="41184-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41184-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="41184-140">响应</span><span class="sxs-lookup"><span data-stu-id="41184-140">Response</span></span>
<span data-ttu-id="41184-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41184-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



