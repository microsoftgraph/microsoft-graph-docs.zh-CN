---
title: getRoleScopeTagsById 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 295b7e7a0d5825d45a5f4ae6a5aceb4647904ec0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386734"
---
# <a name="getrolescopetagsbyid-action"></a><span data-ttu-id="0810a-103">getRoleScopeTagsById 操作</span><span class="sxs-lookup"><span data-stu-id="0810a-103">getRoleScopeTagsById action</span></span>

<span data-ttu-id="0810a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0810a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0810a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0810a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0810a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0810a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0810a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0810a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0810a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0810a-108">Prerequisites</span></span>
<span data-ttu-id="0810a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0810a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0810a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0810a-111">Permission type</span></span>|<span data-ttu-id="0810a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0810a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0810a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0810a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0810a-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0810a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0810a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0810a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0810a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0810a-116">Not supported.</span></span>|
|<span data-ttu-id="0810a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0810a-117">Application</span></span>|<span data-ttu-id="0810a-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0810a-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0810a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0810a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a><span data-ttu-id="0810a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0810a-120">Request headers</span></span>
|<span data-ttu-id="0810a-121">标头</span><span class="sxs-lookup"><span data-stu-id="0810a-121">Header</span></span>|<span data-ttu-id="0810a-122">值</span><span class="sxs-lookup"><span data-stu-id="0810a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0810a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0810a-123">Authorization</span></span>|<span data-ttu-id="0810a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0810a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0810a-125">接受</span><span class="sxs-lookup"><span data-stu-id="0810a-125">Accept</span></span>|<span data-ttu-id="0810a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0810a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0810a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0810a-127">Request body</span></span>
<span data-ttu-id="0810a-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0810a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0810a-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0810a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0810a-130">属性</span><span class="sxs-lookup"><span data-stu-id="0810a-130">Property</span></span>|<span data-ttu-id="0810a-131">类型</span><span class="sxs-lookup"><span data-stu-id="0810a-131">Type</span></span>|<span data-ttu-id="0810a-132">说明</span><span class="sxs-lookup"><span data-stu-id="0810a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0810a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0810a-133">roleScopeTagIds</span></span>|<span data-ttu-id="0810a-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0810a-134">String collection</span></span>|<span data-ttu-id="0810a-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0810a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0810a-136">响应</span><span class="sxs-lookup"><span data-stu-id="0810a-136">Response</span></span>
<span data-ttu-id="0810a-137">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合。</span><span class="sxs-lookup"><span data-stu-id="0810a-137">If successful, this action returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0810a-138">示例</span><span class="sxs-lookup"><span data-stu-id="0810a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0810a-139">请求</span><span class="sxs-lookup"><span data-stu-id="0810a-139">Request</span></span>
<span data-ttu-id="0810a-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0810a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0810a-141">响应</span><span class="sxs-lookup"><span data-stu-id="0810a-141">Response</span></span>
<span data-ttu-id="0810a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0810a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



