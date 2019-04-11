---
title: 更新 roleDefinition
description: 更新 roleDefinition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e787c326a862b1d2bbbda50ed3106fdfdcf235ca
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805885"
---
# <a name="update-roledefinition"></a><span data-ttu-id="a40dd-103">更新 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a40dd-103">Update roleDefinition</span></span>

> <span data-ttu-id="a40dd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a40dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a40dd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a40dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a40dd-106">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a40dd-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a40dd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a40dd-107">Prerequisites</span></span>
<span data-ttu-id="a40dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a40dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a40dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a40dd-110">Permission type</span></span>|<span data-ttu-id="a40dd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a40dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a40dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a40dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a40dd-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a40dd-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a40dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a40dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a40dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a40dd-115">Not supported.</span></span>|
|<span data-ttu-id="a40dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a40dd-116">Application</span></span>|<span data-ttu-id="a40dd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a40dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a40dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a40dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="a40dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a40dd-119">Request headers</span></span>
|<span data-ttu-id="a40dd-120">标头</span><span class="sxs-lookup"><span data-stu-id="a40dd-120">Header</span></span>|<span data-ttu-id="a40dd-121">值</span><span class="sxs-lookup"><span data-stu-id="a40dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a40dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a40dd-122">Authorization</span></span>|<span data-ttu-id="a40dd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a40dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a40dd-124">接受</span><span class="sxs-lookup"><span data-stu-id="a40dd-124">Accept</span></span>|<span data-ttu-id="a40dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a40dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a40dd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a40dd-126">Request body</span></span>
<span data-ttu-id="a40dd-127">在请求正文中，提供 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a40dd-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="a40dd-128">下表显示创建 [roleDefinition](../resources/intune-rbac-roledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a40dd-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="a40dd-129">属性</span><span class="sxs-lookup"><span data-stu-id="a40dd-129">Property</span></span>|<span data-ttu-id="a40dd-130">类型</span><span class="sxs-lookup"><span data-stu-id="a40dd-130">Type</span></span>|<span data-ttu-id="a40dd-131">说明</span><span class="sxs-lookup"><span data-stu-id="a40dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a40dd-132">id</span><span class="sxs-lookup"><span data-stu-id="a40dd-132">id</span></span>|<span data-ttu-id="a40dd-133">String</span><span class="sxs-lookup"><span data-stu-id="a40dd-133">String</span></span>|<span data-ttu-id="a40dd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a40dd-134">Key of the entity.</span></span> <span data-ttu-id="a40dd-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a40dd-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a40dd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a40dd-136">displayName</span></span>|<span data-ttu-id="a40dd-137">String</span><span class="sxs-lookup"><span data-stu-id="a40dd-137">String</span></span>|<span data-ttu-id="a40dd-138">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a40dd-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="a40dd-139">description</span><span class="sxs-lookup"><span data-stu-id="a40dd-139">description</span></span>|<span data-ttu-id="a40dd-140">String</span><span class="sxs-lookup"><span data-stu-id="a40dd-140">String</span></span>|<span data-ttu-id="a40dd-141">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="a40dd-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="a40dd-142">permissions</span><span class="sxs-lookup"><span data-stu-id="a40dd-142">permissions</span></span>|<span data-ttu-id="a40dd-143">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a40dd-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a40dd-144">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="a40dd-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a40dd-145">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="a40dd-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a40dd-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a40dd-146">rolePermissions</span></span>|<span data-ttu-id="a40dd-147">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a40dd-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a40dd-148">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="a40dd-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a40dd-149">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="a40dd-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a40dd-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a40dd-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="a40dd-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a40dd-151">Boolean</span></span>|<span data-ttu-id="a40dd-152">角色类型。</span><span class="sxs-lookup"><span data-stu-id="a40dd-152">Type of Role.</span></span> <span data-ttu-id="a40dd-153">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="a40dd-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a40dd-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a40dd-154">isBuiltIn</span></span>|<span data-ttu-id="a40dd-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="a40dd-155">Boolean</span></span>|<span data-ttu-id="a40dd-156">角色类型。</span><span class="sxs-lookup"><span data-stu-id="a40dd-156">Type of Role.</span></span> <span data-ttu-id="a40dd-157">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="a40dd-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a40dd-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a40dd-158">roleScopeTagIds</span></span>|<span data-ttu-id="a40dd-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="a40dd-159">String collection</span></span>|<span data-ttu-id="a40dd-160">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a40dd-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a40dd-161">响应</span><span class="sxs-lookup"><span data-stu-id="a40dd-161">Response</span></span>
<span data-ttu-id="a40dd-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a40dd-162">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a40dd-163">示例</span><span class="sxs-lookup"><span data-stu-id="a40dd-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a40dd-164">请求</span><span class="sxs-lookup"><span data-stu-id="a40dd-164">Request</span></span>
<span data-ttu-id="a40dd-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a40dd-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a40dd-166">响应</span><span class="sxs-lookup"><span data-stu-id="a40dd-166">Response</span></span>
<span data-ttu-id="a40dd-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a40dd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





