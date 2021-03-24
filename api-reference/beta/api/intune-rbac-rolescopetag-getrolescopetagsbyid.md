---
title: getRoleScopeTagsById 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da3aa6217e48fc618e01226ca74bda17f8b0e1e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148314"
---
# <a name="getrolescopetagsbyid-action"></a><span data-ttu-id="fdfc7-103">getRoleScopeTagsById 操作</span><span class="sxs-lookup"><span data-stu-id="fdfc7-103">getRoleScopeTagsById action</span></span>

<span data-ttu-id="fdfc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdfc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdfc7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdfc7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdfc7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fdfc7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdfc7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fdfc7-108">Prerequisites</span></span>
<span data-ttu-id="fdfc7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdfc7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdfc7-111">Permission type</span></span>|<span data-ttu-id="fdfc7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fdfc7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdfc7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdfc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdfc7-114">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdfc7-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fdfc7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdfc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdfc7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-116">Not supported.</span></span>|
|<span data-ttu-id="fdfc7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdfc7-117">Application</span></span>|<span data-ttu-id="fdfc7-118">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdfc7-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdfc7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdfc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a><span data-ttu-id="fdfc7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdfc7-120">Request headers</span></span>
|<span data-ttu-id="fdfc7-121">标头</span><span class="sxs-lookup"><span data-stu-id="fdfc7-121">Header</span></span>|<span data-ttu-id="fdfc7-122">值</span><span class="sxs-lookup"><span data-stu-id="fdfc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdfc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdfc7-123">Authorization</span></span>|<span data-ttu-id="fdfc7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdfc7-125">接受</span><span class="sxs-lookup"><span data-stu-id="fdfc7-125">Accept</span></span>|<span data-ttu-id="fdfc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdfc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdfc7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdfc7-127">Request body</span></span>
<span data-ttu-id="fdfc7-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fdfc7-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fdfc7-130">属性</span><span class="sxs-lookup"><span data-stu-id="fdfc7-130">Property</span></span>|<span data-ttu-id="fdfc7-131">类型</span><span class="sxs-lookup"><span data-stu-id="fdfc7-131">Type</span></span>|<span data-ttu-id="fdfc7-132">说明</span><span class="sxs-lookup"><span data-stu-id="fdfc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdfc7-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fdfc7-133">roleScopeTagIds</span></span>|<span data-ttu-id="fdfc7-134">String collection</span><span class="sxs-lookup"><span data-stu-id="fdfc7-134">String collection</span></span>|<span data-ttu-id="fdfc7-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fdfc7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fdfc7-136">响应</span><span class="sxs-lookup"><span data-stu-id="fdfc7-136">Response</span></span>
<span data-ttu-id="fdfc7-137">如果成功，此操作在响应 `200 OK` 正文中返回 响应代码和 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-137">If successful, this action returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdfc7-138">示例</span><span class="sxs-lookup"><span data-stu-id="fdfc7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdfc7-139">请求</span><span class="sxs-lookup"><span data-stu-id="fdfc7-139">Request</span></span>
<span data-ttu-id="fdfc7-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdfc7-141">响应</span><span class="sxs-lookup"><span data-stu-id="fdfc7-141">Response</span></span>
<span data-ttu-id="fdfc7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fdfc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




