---
title: getRoleScopeTagsByIds 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 764bfd10fdfde445d38dbf5eb4f2552f02a8231f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403873"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="24362-103">getRoleScopeTagsByIds 函数</span><span class="sxs-lookup"><span data-stu-id="24362-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="24362-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="24362-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24362-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24362-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24362-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24362-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24362-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24362-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24362-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="24362-108">Prerequisites</span></span>
<span data-ttu-id="24362-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24362-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24362-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24362-111">Permission type</span></span>|<span data-ttu-id="24362-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24362-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24362-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24362-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="24362-114">&nbsp;&nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="24362-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="24362-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="24362-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="24362-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24362-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24362-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="24362-117">Not supported.</span></span>|
|<span data-ttu-id="24362-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="24362-118">Application</span></span>|<span data-ttu-id="24362-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="24362-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24362-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24362-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="24362-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="24362-121">Request headers</span></span>
|<span data-ttu-id="24362-122">标头</span><span class="sxs-lookup"><span data-stu-id="24362-122">Header</span></span>|<span data-ttu-id="24362-123">值</span><span class="sxs-lookup"><span data-stu-id="24362-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24362-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="24362-124">Authorization</span></span>|<span data-ttu-id="24362-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24362-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24362-126">Accept</span><span class="sxs-lookup"><span data-stu-id="24362-126">Accept</span></span>|<span data-ttu-id="24362-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24362-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24362-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="24362-128">Request body</span></span>
<span data-ttu-id="24362-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="24362-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="24362-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="24362-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="24362-131">属性</span><span class="sxs-lookup"><span data-stu-id="24362-131">Property</span></span>|<span data-ttu-id="24362-132">类型</span><span class="sxs-lookup"><span data-stu-id="24362-132">Type</span></span>|<span data-ttu-id="24362-133">说明</span><span class="sxs-lookup"><span data-stu-id="24362-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24362-134">ids</span><span class="sxs-lookup"><span data-stu-id="24362-134">ids</span></span>|<span data-ttu-id="24362-135">String collection</span><span class="sxs-lookup"><span data-stu-id="24362-135">String collection</span></span>|<span data-ttu-id="24362-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24362-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="24362-137">响应</span><span class="sxs-lookup"><span data-stu-id="24362-137">Response</span></span>
<span data-ttu-id="24362-138">如果成功，此函数返回`200 OK`响应代码和响应正文中的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合。</span><span class="sxs-lookup"><span data-stu-id="24362-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24362-139">示例</span><span class="sxs-lookup"><span data-stu-id="24362-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="24362-140">请求</span><span class="sxs-lookup"><span data-stu-id="24362-140">Request</span></span>
<span data-ttu-id="24362-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24362-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="24362-142">响应</span><span class="sxs-lookup"><span data-stu-id="24362-142">Response</span></span>
<span data-ttu-id="24362-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24362-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



