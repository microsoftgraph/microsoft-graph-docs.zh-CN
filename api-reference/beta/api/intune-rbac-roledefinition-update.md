---
title: 更新 roleDefinition
description: 更新 roleDefinition 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e05136a24bbac8d9b646ea3b213884ca77355782
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459637"
---
# <a name="update-roledefinition"></a><span data-ttu-id="e873e-103">更新 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e873e-103">Update roleDefinition</span></span>

<span data-ttu-id="e873e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e873e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e873e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e873e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e873e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e873e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e873e-107">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e873e-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e873e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e873e-108">Prerequisites</span></span>
<span data-ttu-id="e873e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e873e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e873e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e873e-111">Permission type</span></span>|<span data-ttu-id="e873e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e873e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e873e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e873e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e873e-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e873e-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e873e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e873e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e873e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e873e-116">Not supported.</span></span>|
|<span data-ttu-id="e873e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e873e-117">Application</span></span>|<span data-ttu-id="e873e-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e873e-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e873e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e873e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="e873e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e873e-120">Request headers</span></span>
|<span data-ttu-id="e873e-121">标头</span><span class="sxs-lookup"><span data-stu-id="e873e-121">Header</span></span>|<span data-ttu-id="e873e-122">值</span><span class="sxs-lookup"><span data-stu-id="e873e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e873e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e873e-123">Authorization</span></span>|<span data-ttu-id="e873e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e873e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e873e-125">接受</span><span class="sxs-lookup"><span data-stu-id="e873e-125">Accept</span></span>|<span data-ttu-id="e873e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e873e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e873e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e873e-127">Request body</span></span>
<span data-ttu-id="e873e-128">在请求正文中，提供 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e873e-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="e873e-129">下表显示创建 [roleDefinition](../resources/intune-rbac-roledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e873e-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="e873e-130">属性</span><span class="sxs-lookup"><span data-stu-id="e873e-130">Property</span></span>|<span data-ttu-id="e873e-131">类型</span><span class="sxs-lookup"><span data-stu-id="e873e-131">Type</span></span>|<span data-ttu-id="e873e-132">说明</span><span class="sxs-lookup"><span data-stu-id="e873e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e873e-133">id</span><span class="sxs-lookup"><span data-stu-id="e873e-133">id</span></span>|<span data-ttu-id="e873e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e873e-134">String</span></span>|<span data-ttu-id="e873e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e873e-135">Key of the entity.</span></span> <span data-ttu-id="e873e-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="e873e-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e873e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e873e-137">displayName</span></span>|<span data-ttu-id="e873e-138">String</span><span class="sxs-lookup"><span data-stu-id="e873e-138">String</span></span>|<span data-ttu-id="e873e-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e873e-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="e873e-140">说明</span><span class="sxs-lookup"><span data-stu-id="e873e-140">description</span></span>|<span data-ttu-id="e873e-141">String</span><span class="sxs-lookup"><span data-stu-id="e873e-141">String</span></span>|<span data-ttu-id="e873e-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="e873e-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="e873e-143">permissions</span><span class="sxs-lookup"><span data-stu-id="e873e-143">permissions</span></span>|<span data-ttu-id="e873e-144">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e873e-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e873e-145">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="e873e-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e873e-146">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="e873e-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e873e-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e873e-147">rolePermissions</span></span>|<span data-ttu-id="e873e-148">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e873e-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e873e-149">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="e873e-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e873e-150">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="e873e-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e873e-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e873e-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="e873e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e873e-152">Boolean</span></span>|<span data-ttu-id="e873e-153">角色类型。</span><span class="sxs-lookup"><span data-stu-id="e873e-153">Type of Role.</span></span> <span data-ttu-id="e873e-154">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="e873e-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="e873e-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e873e-155">isBuiltIn</span></span>|<span data-ttu-id="e873e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e873e-156">Boolean</span></span>|<span data-ttu-id="e873e-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="e873e-157">Type of Role.</span></span> <span data-ttu-id="e873e-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="e873e-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="e873e-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e873e-159">roleScopeTagIds</span></span>|<span data-ttu-id="e873e-160">String 集合</span><span class="sxs-lookup"><span data-stu-id="e873e-160">String collection</span></span>|<span data-ttu-id="e873e-161">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e873e-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e873e-162">响应</span><span class="sxs-lookup"><span data-stu-id="e873e-162">Response</span></span>
<span data-ttu-id="e873e-163">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e873e-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e873e-164">示例</span><span class="sxs-lookup"><span data-stu-id="e873e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e873e-165">请求</span><span class="sxs-lookup"><span data-stu-id="e873e-165">Request</span></span>
<span data-ttu-id="e873e-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e873e-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1207

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
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
  ],
  "rolePermissions": [
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
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e873e-167">响应</span><span class="sxs-lookup"><span data-stu-id="e873e-167">Response</span></span>
<span data-ttu-id="e873e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e873e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
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
  ],
  "rolePermissions": [
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
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





