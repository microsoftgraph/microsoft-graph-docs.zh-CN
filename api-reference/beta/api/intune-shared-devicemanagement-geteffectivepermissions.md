---
title: getEffectivePermissions 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e480b90dba719f52d49c4afb8fc2646be7d4660
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801059"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="176d3-103">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="176d3-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="176d3-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="176d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="176d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="176d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="176d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="176d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="176d3-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="176d3-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="176d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="176d3-108">Prerequisites</span></span>
<span data-ttu-id="176d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="176d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="176d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="176d3-111">Permission type</span></span>|<span data-ttu-id="176d3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="176d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="176d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="176d3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="176d3-114">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="176d3-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="176d3-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="176d3-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="176d3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="176d3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="176d3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="176d3-117">Not supported.</span></span>|
|<span data-ttu-id="176d3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="176d3-118">Application</span></span>||
| <span data-ttu-id="176d3-119">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="176d3-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="176d3-120">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="176d3-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="176d3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="176d3-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="176d3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="176d3-122">Request headers</span></span>
|<span data-ttu-id="176d3-123">标头</span><span class="sxs-lookup"><span data-stu-id="176d3-123">Header</span></span>|<span data-ttu-id="176d3-124">值</span><span class="sxs-lookup"><span data-stu-id="176d3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="176d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="176d3-125">Authorization</span></span>|<span data-ttu-id="176d3-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="176d3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="176d3-127">接受</span><span class="sxs-lookup"><span data-stu-id="176d3-127">Accept</span></span>|<span data-ttu-id="176d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="176d3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="176d3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="176d3-129">Request body</span></span>
<span data-ttu-id="176d3-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="176d3-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="176d3-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="176d3-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="176d3-132">属性</span><span class="sxs-lookup"><span data-stu-id="176d3-132">Property</span></span>|<span data-ttu-id="176d3-133">类型</span><span class="sxs-lookup"><span data-stu-id="176d3-133">Type</span></span>|<span data-ttu-id="176d3-134">说明</span><span class="sxs-lookup"><span data-stu-id="176d3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176d3-135">scope</span><span class="sxs-lookup"><span data-stu-id="176d3-135">scope</span></span>|<span data-ttu-id="176d3-136">String</span><span class="sxs-lookup"><span data-stu-id="176d3-136">String</span></span>|<span data-ttu-id="176d3-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="176d3-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="176d3-138">响应</span><span class="sxs-lookup"><span data-stu-id="176d3-138">Response</span></span>
<span data-ttu-id="176d3-139">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune-rbac-rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="176d3-139">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="176d3-140">示例</span><span class="sxs-lookup"><span data-stu-id="176d3-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="176d3-141">请求</span><span class="sxs-lookup"><span data-stu-id="176d3-141">Request</span></span>
<span data-ttu-id="176d3-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="176d3-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="176d3-143">响应</span><span class="sxs-lookup"><span data-stu-id="176d3-143">Response</span></span>
<span data-ttu-id="176d3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="176d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










