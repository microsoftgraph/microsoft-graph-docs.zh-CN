---
title: getRoleScopeTagsByResource 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 248027085635c02cff0fb0e4247896e9134d14ae
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210294"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="670c6-103">getRoleScopeTagsByResource 函数</span><span class="sxs-lookup"><span data-stu-id="670c6-103">getRoleScopeTagsByResource function</span></span>

<span data-ttu-id="670c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="670c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="670c6-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="670c6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="670c6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="670c6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="670c6-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="670c6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="670c6-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="670c6-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="670c6-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="670c6-109">Prerequisites</span></span>
<span data-ttu-id="670c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="670c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="670c6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="670c6-112">Permission type</span></span>|<span data-ttu-id="670c6-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="670c6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="670c6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="670c6-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="670c6-115">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="670c6-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="670c6-116">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="670c6-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="670c6-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="670c6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="670c6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="670c6-118">Not supported.</span></span>|
|<span data-ttu-id="670c6-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="670c6-119">Application</span></span>||
| <span data-ttu-id="670c6-120">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="670c6-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="670c6-121">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="670c6-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="670c6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="670c6-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="670c6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="670c6-123">Request headers</span></span>
|<span data-ttu-id="670c6-124">标头</span><span class="sxs-lookup"><span data-stu-id="670c6-124">Header</span></span>|<span data-ttu-id="670c6-125">值</span><span class="sxs-lookup"><span data-stu-id="670c6-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="670c6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="670c6-126">Authorization</span></span>|<span data-ttu-id="670c6-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="670c6-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="670c6-128">接受</span><span class="sxs-lookup"><span data-stu-id="670c6-128">Accept</span></span>|<span data-ttu-id="670c6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="670c6-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="670c6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="670c6-130">Request body</span></span>
<span data-ttu-id="670c6-131">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="670c6-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="670c6-132">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="670c6-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="670c6-133">属性</span><span class="sxs-lookup"><span data-stu-id="670c6-133">Property</span></span>|<span data-ttu-id="670c6-134">类型</span><span class="sxs-lookup"><span data-stu-id="670c6-134">Type</span></span>|<span data-ttu-id="670c6-135">说明</span><span class="sxs-lookup"><span data-stu-id="670c6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="670c6-136">资源</span><span class="sxs-lookup"><span data-stu-id="670c6-136">resource</span></span>|<span data-ttu-id="670c6-137">String</span><span class="sxs-lookup"><span data-stu-id="670c6-137">String</span></span>|<span data-ttu-id="670c6-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="670c6-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="670c6-139">响应</span><span class="sxs-lookup"><span data-stu-id="670c6-139">Response</span></span>
<span data-ttu-id="670c6-140">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="670c6-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="670c6-141">示例</span><span class="sxs-lookup"><span data-stu-id="670c6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="670c6-142">请求</span><span class="sxs-lookup"><span data-stu-id="670c6-142">Request</span></span>
<span data-ttu-id="670c6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="670c6-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="670c6-144">响应</span><span class="sxs-lookup"><span data-stu-id="670c6-144">Response</span></span>
<span data-ttu-id="670c6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="670c6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```










