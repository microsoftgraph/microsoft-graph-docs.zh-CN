---
title: getRoleScopeTagsByResource 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54cc2ba137a3c4a45fc3ca724fa47c1f3f3e0490
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140661"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="d5c14-103">getRoleScopeTagsByResource 函数</span><span class="sxs-lookup"><span data-stu-id="d5c14-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="d5c14-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5c14-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5c14-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5c14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c14-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5c14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5c14-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d5c14-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5c14-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5c14-108">Prerequisites</span></span>
<span data-ttu-id="d5c14-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5c14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="d5c14-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5c14-111">Permission type</span></span>|<span data-ttu-id="d5c14-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5c14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c14-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c14-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5c14-114">&nbsp;&nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="d5c14-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="d5c14-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d5c14-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c14-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c14-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c14-117">Not supported.</span></span>|
|<span data-ttu-id="d5c14-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5c14-118">Application</span></span>|<span data-ttu-id="d5c14-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c14-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c14-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5c14-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="d5c14-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5c14-121">Request headers</span></span>
|<span data-ttu-id="d5c14-122">标头</span><span class="sxs-lookup"><span data-stu-id="d5c14-122">Header</span></span>|<span data-ttu-id="d5c14-123">值</span><span class="sxs-lookup"><span data-stu-id="d5c14-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c14-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c14-124">Authorization</span></span>|<span data-ttu-id="d5c14-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5c14-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c14-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d5c14-126">Accept</span></span>|<span data-ttu-id="d5c14-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c14-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c14-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5c14-128">Request body</span></span>
<span data-ttu-id="d5c14-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="d5c14-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d5c14-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d5c14-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d5c14-131">属性</span><span class="sxs-lookup"><span data-stu-id="d5c14-131">Property</span></span>|<span data-ttu-id="d5c14-132">类型</span><span class="sxs-lookup"><span data-stu-id="d5c14-132">Type</span></span>|<span data-ttu-id="d5c14-133">说明</span><span class="sxs-lookup"><span data-stu-id="d5c14-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c14-134">资源</span><span class="sxs-lookup"><span data-stu-id="d5c14-134">resource</span></span>|<span data-ttu-id="d5c14-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d5c14-135">String</span></span>|<span data-ttu-id="d5c14-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d5c14-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5c14-137">响应</span><span class="sxs-lookup"><span data-stu-id="d5c14-137">Response</span></span>
<span data-ttu-id="d5c14-138">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合。</span><span class="sxs-lookup"><span data-stu-id="d5c14-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c14-139">示例</span><span class="sxs-lookup"><span data-stu-id="d5c14-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5c14-140">请求</span><span class="sxs-lookup"><span data-stu-id="d5c14-140">Request</span></span>
<span data-ttu-id="d5c14-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5c14-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d5c14-142">响应</span><span class="sxs-lookup"><span data-stu-id="d5c14-142">Response</span></span>
<span data-ttu-id="d5c14-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5c14-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



