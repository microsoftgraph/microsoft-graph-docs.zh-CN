---
title: getRoleScopeTagsByIds 函数
description: 尚未记录
ms.openlocfilehash: 67722ad61a71f8d8572a95c5972992d4e0818931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046645"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="12021-103">getRoleScopeTagsByIds 函数</span><span class="sxs-lookup"><span data-stu-id="12021-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="12021-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12021-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12021-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12021-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12021-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12021-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12021-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12021-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12021-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12021-108">Prerequisites</span></span>
<span data-ttu-id="12021-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="12021-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12021-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12021-111">Permission type</span></span>|<span data-ttu-id="12021-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12021-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12021-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12021-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="12021-114">&nbsp;&nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="12021-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="12021-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="12021-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="12021-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12021-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12021-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="12021-117">Not supported.</span></span>|
|<span data-ttu-id="12021-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="12021-118">Application</span></span>|<span data-ttu-id="12021-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="12021-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12021-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12021-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="12021-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="12021-121">Request headers</span></span>
|<span data-ttu-id="12021-122">标头</span><span class="sxs-lookup"><span data-stu-id="12021-122">Header</span></span>|<span data-ttu-id="12021-123">值</span><span class="sxs-lookup"><span data-stu-id="12021-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12021-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="12021-124">Authorization</span></span>|<span data-ttu-id="12021-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12021-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12021-126">Accept</span><span class="sxs-lookup"><span data-stu-id="12021-126">Accept</span></span>|<span data-ttu-id="12021-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12021-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12021-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="12021-128">Request body</span></span>
<span data-ttu-id="12021-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="12021-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="12021-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="12021-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="12021-131">属性</span><span class="sxs-lookup"><span data-stu-id="12021-131">Property</span></span>|<span data-ttu-id="12021-132">类型</span><span class="sxs-lookup"><span data-stu-id="12021-132">Type</span></span>|<span data-ttu-id="12021-133">说明</span><span class="sxs-lookup"><span data-stu-id="12021-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12021-134">ids</span><span class="sxs-lookup"><span data-stu-id="12021-134">ids</span></span>|<span data-ttu-id="12021-135">String collection</span><span class="sxs-lookup"><span data-stu-id="12021-135">String collection</span></span>|<span data-ttu-id="12021-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12021-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="12021-137">响应</span><span class="sxs-lookup"><span data-stu-id="12021-137">Response</span></span>
<span data-ttu-id="12021-138">如果成功，此函数返回`200 OK`响应代码和响应正文中的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合。</span><span class="sxs-lookup"><span data-stu-id="12021-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12021-139">示例</span><span class="sxs-lookup"><span data-stu-id="12021-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="12021-140">请求</span><span class="sxs-lookup"><span data-stu-id="12021-140">Request</span></span>
<span data-ttu-id="12021-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12021-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="12021-142">响应</span><span class="sxs-lookup"><span data-stu-id="12021-142">Response</span></span>
<span data-ttu-id="12021-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12021-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



