---
title: getEffectivePermissions 函数
description: 检索当前验证的用户的有效权限
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bed8a2fd1baf8396bd49801a9bbfb41276bda9e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732381"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="a66ab-103">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="a66ab-103">getEffectivePermissions function</span></span>

<span data-ttu-id="a66ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a66ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a66ab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a66ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a66ab-106">检索当前验证的用户的有效权限</span><span class="sxs-lookup"><span data-stu-id="a66ab-106">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a66ab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a66ab-107">Prerequisites</span></span>
<span data-ttu-id="a66ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a66ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a66ab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a66ab-110">Permission type</span></span>|<span data-ttu-id="a66ab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a66ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a66ab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a66ab-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a66ab-113">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="a66ab-113">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="a66ab-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a66ab-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a66ab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a66ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a66ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a66ab-116">Not supported.</span></span>|
|<span data-ttu-id="a66ab-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a66ab-117">Application</span></span>|<span data-ttu-id="a66ab-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a66ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a66ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a66ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="a66ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a66ab-120">Request headers</span></span>
|<span data-ttu-id="a66ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="a66ab-121">Header</span></span>|<span data-ttu-id="a66ab-122">值</span><span class="sxs-lookup"><span data-stu-id="a66ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a66ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a66ab-123">Authorization</span></span>|<span data-ttu-id="a66ab-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a66ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a66ab-125">接受</span><span class="sxs-lookup"><span data-stu-id="a66ab-125">Accept</span></span>|<span data-ttu-id="a66ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a66ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a66ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a66ab-127">Request body</span></span>
<span data-ttu-id="a66ab-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="a66ab-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a66ab-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="a66ab-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a66ab-130">属性</span><span class="sxs-lookup"><span data-stu-id="a66ab-130">Property</span></span>|<span data-ttu-id="a66ab-131">类型</span><span class="sxs-lookup"><span data-stu-id="a66ab-131">Type</span></span>|<span data-ttu-id="a66ab-132">Description</span><span class="sxs-lookup"><span data-stu-id="a66ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a66ab-133">scope</span><span class="sxs-lookup"><span data-stu-id="a66ab-133">scope</span></span>|<span data-ttu-id="a66ab-134">String</span><span class="sxs-lookup"><span data-stu-id="a66ab-134">String</span></span>|<span data-ttu-id="a66ab-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a66ab-135">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="a66ab-136">响应</span><span class="sxs-lookup"><span data-stu-id="a66ab-136">Response</span></span>
<span data-ttu-id="a66ab-137">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune-rbac-rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="a66ab-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a66ab-138">示例</span><span class="sxs-lookup"><span data-stu-id="a66ab-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="a66ab-139">请求</span><span class="sxs-lookup"><span data-stu-id="a66ab-139">Request</span></span>
<span data-ttu-id="a66ab-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a66ab-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a66ab-141">响应</span><span class="sxs-lookup"><span data-stu-id="a66ab-141">Response</span></span>
<span data-ttu-id="a66ab-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a66ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









