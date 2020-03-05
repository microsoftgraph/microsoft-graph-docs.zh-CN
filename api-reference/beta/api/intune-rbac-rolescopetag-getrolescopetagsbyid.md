---
title: getRoleScopeTagsById 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: acb8f73b73099cc618275bc7d39809af2df22e2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459480"
---
# <a name="getrolescopetagsbyid-action"></a><span data-ttu-id="248b6-103">getRoleScopeTagsById 操作</span><span class="sxs-lookup"><span data-stu-id="248b6-103">getRoleScopeTagsById action</span></span>

<span data-ttu-id="248b6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="248b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="248b6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="248b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="248b6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="248b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="248b6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="248b6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="248b6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="248b6-108">Prerequisites</span></span>
<span data-ttu-id="248b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="248b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="248b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="248b6-111">Permission type</span></span>|<span data-ttu-id="248b6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="248b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="248b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="248b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="248b6-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="248b6-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="248b6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="248b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="248b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="248b6-116">Not supported.</span></span>|
|<span data-ttu-id="248b6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="248b6-117">Application</span></span>|<span data-ttu-id="248b6-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="248b6-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="248b6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="248b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a><span data-ttu-id="248b6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="248b6-120">Request headers</span></span>
|<span data-ttu-id="248b6-121">标头</span><span class="sxs-lookup"><span data-stu-id="248b6-121">Header</span></span>|<span data-ttu-id="248b6-122">值</span><span class="sxs-lookup"><span data-stu-id="248b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="248b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="248b6-123">Authorization</span></span>|<span data-ttu-id="248b6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="248b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="248b6-125">接受</span><span class="sxs-lookup"><span data-stu-id="248b6-125">Accept</span></span>|<span data-ttu-id="248b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="248b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="248b6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="248b6-127">Request body</span></span>
<span data-ttu-id="248b6-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="248b6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="248b6-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="248b6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="248b6-130">属性</span><span class="sxs-lookup"><span data-stu-id="248b6-130">Property</span></span>|<span data-ttu-id="248b6-131">类型</span><span class="sxs-lookup"><span data-stu-id="248b6-131">Type</span></span>|<span data-ttu-id="248b6-132">说明</span><span class="sxs-lookup"><span data-stu-id="248b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="248b6-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="248b6-133">roleScopeTagIds</span></span>|<span data-ttu-id="248b6-134">String collection</span><span class="sxs-lookup"><span data-stu-id="248b6-134">String collection</span></span>|<span data-ttu-id="248b6-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="248b6-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="248b6-136">响应</span><span class="sxs-lookup"><span data-stu-id="248b6-136">Response</span></span>
<span data-ttu-id="248b6-137">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合。</span><span class="sxs-lookup"><span data-stu-id="248b6-137">If successful, this action returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="248b6-138">示例</span><span class="sxs-lookup"><span data-stu-id="248b6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="248b6-139">请求</span><span class="sxs-lookup"><span data-stu-id="248b6-139">Request</span></span>
<span data-ttu-id="248b6-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="248b6-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/getRoleScopeTagsById

Content-type: application/json
Content-length: 65

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="248b6-141">响应</span><span class="sxs-lookup"><span data-stu-id="248b6-141">Response</span></span>
<span data-ttu-id="248b6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="248b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value",
      "isBuiltIn": true
    }
  ]
}
```





