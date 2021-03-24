---
title: 创建 deviceAndAppManagementRoleDefinition
description: 创建新的 deviceAndAppManagementRoleDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc2d0b6ed04ec8517fee21db099692351d511703
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145003"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ce47b-103">创建 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ce47b-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="ce47b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce47b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce47b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce47b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce47b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce47b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce47b-107">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce47b-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce47b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce47b-108">Prerequisites</span></span>
<span data-ttu-id="ce47b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce47b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce47b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce47b-111">Permission type</span></span>|<span data-ttu-id="ce47b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce47b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce47b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce47b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce47b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce47b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ce47b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce47b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce47b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce47b-116">Not supported.</span></span>|
|<span data-ttu-id="ce47b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce47b-117">Application</span></span>|<span data-ttu-id="ce47b-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce47b-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce47b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce47b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ce47b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce47b-120">Request headers</span></span>
|<span data-ttu-id="ce47b-121">标头</span><span class="sxs-lookup"><span data-stu-id="ce47b-121">Header</span></span>|<span data-ttu-id="ce47b-122">值</span><span class="sxs-lookup"><span data-stu-id="ce47b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce47b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce47b-123">Authorization</span></span>|<span data-ttu-id="ce47b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce47b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce47b-125">接受</span><span class="sxs-lookup"><span data-stu-id="ce47b-125">Accept</span></span>|<span data-ttu-id="ce47b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce47b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce47b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce47b-127">Request body</span></span>
<span data-ttu-id="ce47b-128">在请求正文中，提供 deviceAndAppManagementRoleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce47b-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="ce47b-129">下表显示创建 deviceAndAppManagementRoleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce47b-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="ce47b-130">属性</span><span class="sxs-lookup"><span data-stu-id="ce47b-130">Property</span></span>|<span data-ttu-id="ce47b-131">类型</span><span class="sxs-lookup"><span data-stu-id="ce47b-131">Type</span></span>|<span data-ttu-id="ce47b-132">说明</span><span class="sxs-lookup"><span data-stu-id="ce47b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce47b-133">id</span><span class="sxs-lookup"><span data-stu-id="ce47b-133">id</span></span>|<span data-ttu-id="ce47b-134">String</span><span class="sxs-lookup"><span data-stu-id="ce47b-134">String</span></span>|<span data-ttu-id="ce47b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce47b-135">Key of the entity.</span></span> <span data-ttu-id="ce47b-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="ce47b-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="ce47b-137">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ce47b-138">displayName</span></span>|<span data-ttu-id="ce47b-139">String</span><span class="sxs-lookup"><span data-stu-id="ce47b-139">String</span></span>|<span data-ttu-id="ce47b-140">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ce47b-140">Display Name of the Role definition.</span></span> <span data-ttu-id="ce47b-141">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-142">说明</span><span class="sxs-lookup"><span data-stu-id="ce47b-142">description</span></span>|<span data-ttu-id="ce47b-143">String</span><span class="sxs-lookup"><span data-stu-id="ce47b-143">String</span></span>|<span data-ttu-id="ce47b-144">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="ce47b-144">Description of the Role definition.</span></span> <span data-ttu-id="ce47b-145">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-146">权限</span><span class="sxs-lookup"><span data-stu-id="ce47b-146">permissions</span></span>|<span data-ttu-id="ce47b-147">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ce47b-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ce47b-148">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="ce47b-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ce47b-149">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="ce47b-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ce47b-150">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ce47b-151">rolePermissions</span></span>|<span data-ttu-id="ce47b-152">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ce47b-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ce47b-153">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="ce47b-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ce47b-154">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="ce47b-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ce47b-155">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ce47b-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="ce47b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce47b-157">Boolean</span></span>|<span data-ttu-id="ce47b-158">角色类型。</span><span class="sxs-lookup"><span data-stu-id="ce47b-158">Type of Role.</span></span> <span data-ttu-id="ce47b-159">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="ce47b-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ce47b-160">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ce47b-161">isBuiltIn</span></span>|<span data-ttu-id="ce47b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce47b-162">Boolean</span></span>|<span data-ttu-id="ce47b-163">角色类型。</span><span class="sxs-lookup"><span data-stu-id="ce47b-163">Type of Role.</span></span> <span data-ttu-id="ce47b-164">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="ce47b-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ce47b-165">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ce47b-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce47b-166">roleScopeTagIds</span></span>|<span data-ttu-id="ce47b-167">String collection</span><span class="sxs-lookup"><span data-stu-id="ce47b-167">String collection</span></span>|<span data-ttu-id="ce47b-168">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ce47b-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce47b-169">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce47b-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ce47b-170">响应</span><span class="sxs-lookup"><span data-stu-id="ce47b-170">Response</span></span>
<span data-ttu-id="ce47b-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce47b-171">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce47b-172">示例</span><span class="sxs-lookup"><span data-stu-id="ce47b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce47b-173">请求</span><span class="sxs-lookup"><span data-stu-id="ce47b-173">Request</span></span>
<span data-ttu-id="ce47b-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce47b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="ce47b-175">响应</span><span class="sxs-lookup"><span data-stu-id="ce47b-175">Response</span></span>
<span data-ttu-id="ce47b-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce47b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




