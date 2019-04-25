---
title: 更新 deviceAndAppManagementRoleDefinition
description: 更新 deviceAndAppManagementRoleDefinition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2279a89aa47802b94f58f92851014d1e0b0eb312
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527593"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="a4c15-103">更新 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a4c15-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="a4c15-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4c15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4c15-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4c15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4c15-106">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4c15-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4c15-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4c15-107">Prerequisites</span></span>
<span data-ttu-id="a4c15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4c15-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4c15-110">Permission type</span></span>|<span data-ttu-id="a4c15-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4c15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4c15-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4c15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4c15-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4c15-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a4c15-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4c15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4c15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4c15-115">Not supported.</span></span>|
|<span data-ttu-id="a4c15-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4c15-116">Application</span></span>|<span data-ttu-id="a4c15-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4c15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4c15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4c15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="a4c15-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4c15-119">Request headers</span></span>
|<span data-ttu-id="a4c15-120">标头</span><span class="sxs-lookup"><span data-stu-id="a4c15-120">Header</span></span>|<span data-ttu-id="a4c15-121">值</span><span class="sxs-lookup"><span data-stu-id="a4c15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4c15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4c15-122">Authorization</span></span>|<span data-ttu-id="a4c15-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4c15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4c15-124">接受</span><span class="sxs-lookup"><span data-stu-id="a4c15-124">Accept</span></span>|<span data-ttu-id="a4c15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4c15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4c15-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4c15-126">Request body</span></span>
<span data-ttu-id="a4c15-127">在请求正文中，提供 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4c15-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="a4c15-128">下表显示创建 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4c15-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="a4c15-129">属性</span><span class="sxs-lookup"><span data-stu-id="a4c15-129">Property</span></span>|<span data-ttu-id="a4c15-130">类型</span><span class="sxs-lookup"><span data-stu-id="a4c15-130">Type</span></span>|<span data-ttu-id="a4c15-131">说明</span><span class="sxs-lookup"><span data-stu-id="a4c15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c15-132">id</span><span class="sxs-lookup"><span data-stu-id="a4c15-132">id</span></span>|<span data-ttu-id="a4c15-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a4c15-133">String</span></span>|<span data-ttu-id="a4c15-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a4c15-134">Key of the entity.</span></span> <span data-ttu-id="a4c15-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a4c15-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="a4c15-136">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a4c15-137">displayName</span></span>|<span data-ttu-id="a4c15-138">String</span><span class="sxs-lookup"><span data-stu-id="a4c15-138">String</span></span>|<span data-ttu-id="a4c15-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a4c15-139">Display Name of the Role definition.</span></span> <span data-ttu-id="a4c15-140">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-141">description</span><span class="sxs-lookup"><span data-stu-id="a4c15-141">description</span></span>|<span data-ttu-id="a4c15-142">String</span><span class="sxs-lookup"><span data-stu-id="a4c15-142">String</span></span>|<span data-ttu-id="a4c15-143">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="a4c15-143">Description of the Role definition.</span></span> <span data-ttu-id="a4c15-144">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-145">permissions</span><span class="sxs-lookup"><span data-stu-id="a4c15-145">permissions</span></span>|<span data-ttu-id="a4c15-146">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4c15-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a4c15-147">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="a4c15-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a4c15-148">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="a4c15-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="a4c15-149">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a4c15-150">rolePermissions</span></span>|<span data-ttu-id="a4c15-151">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4c15-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a4c15-152">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="a4c15-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a4c15-153">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="a4c15-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="a4c15-154">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a4c15-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="a4c15-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4c15-156">Boolean</span></span>|<span data-ttu-id="a4c15-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="a4c15-157">Type of Role.</span></span> <span data-ttu-id="a4c15-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="a4c15-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="a4c15-159">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a4c15-160">isBuiltIn</span></span>|<span data-ttu-id="a4c15-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4c15-161">Boolean</span></span>|<span data-ttu-id="a4c15-162">角色类型。</span><span class="sxs-lookup"><span data-stu-id="a4c15-162">Type of Role.</span></span> <span data-ttu-id="a4c15-163">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="a4c15-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="a4c15-164">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a4c15-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4c15-165">roleScopeTagIds</span></span>|<span data-ttu-id="a4c15-166">String collection</span><span class="sxs-lookup"><span data-stu-id="a4c15-166">String collection</span></span>|<span data-ttu-id="a4c15-167">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a4c15-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4c15-168">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a4c15-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a4c15-169">响应</span><span class="sxs-lookup"><span data-stu-id="a4c15-169">Response</span></span>
<span data-ttu-id="a4c15-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4c15-170">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4c15-171">示例</span><span class="sxs-lookup"><span data-stu-id="a4c15-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4c15-172">请求</span><span class="sxs-lookup"><span data-stu-id="a4c15-172">Request</span></span>
<span data-ttu-id="a4c15-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4c15-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1229

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
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

### <a name="response"></a><span data-ttu-id="a4c15-174">响应</span><span class="sxs-lookup"><span data-stu-id="a4c15-174">Response</span></span>
<span data-ttu-id="a4c15-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4c15-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1278

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
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





