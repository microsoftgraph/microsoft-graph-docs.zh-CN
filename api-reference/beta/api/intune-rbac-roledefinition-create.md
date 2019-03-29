---
title: 创建 roleDefinition
description: 创建新的 roleDefinition 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3f23888e92909c629a7b91f010d64f9e184f0b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960193"
---
# <a name="create-roledefinition"></a><span data-ttu-id="2a7ac-103">创建 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2a7ac-103">Create roleDefinition</span></span>

> <span data-ttu-id="2a7ac-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a7ac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a7ac-106">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a7ac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a7ac-107">Prerequisites</span></span>
<span data-ttu-id="2a7ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a7ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a7ac-110">Permission type</span></span>|<span data-ttu-id="2a7ac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a7ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a7ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a7ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a7ac-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a7ac-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2a7ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a7ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a7ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-115">Not supported.</span></span>|
|<span data-ttu-id="2a7ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a7ac-116">Application</span></span>|<span data-ttu-id="2a7ac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a7ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a7ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="2a7ac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a7ac-119">Request headers</span></span>
|<span data-ttu-id="2a7ac-120">标头</span><span class="sxs-lookup"><span data-stu-id="2a7ac-120">Header</span></span>|<span data-ttu-id="2a7ac-121">值</span><span class="sxs-lookup"><span data-stu-id="2a7ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a7ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a7ac-122">Authorization</span></span>|<span data-ttu-id="2a7ac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a7ac-124">接受</span><span class="sxs-lookup"><span data-stu-id="2a7ac-124">Accept</span></span>|<span data-ttu-id="2a7ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a7ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a7ac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a7ac-126">Request body</span></span>
<span data-ttu-id="2a7ac-127">在请求正文中，提供 roleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="2a7ac-128">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="2a7ac-129">属性</span><span class="sxs-lookup"><span data-stu-id="2a7ac-129">Property</span></span>|<span data-ttu-id="2a7ac-130">类型</span><span class="sxs-lookup"><span data-stu-id="2a7ac-130">Type</span></span>|<span data-ttu-id="2a7ac-131">说明</span><span class="sxs-lookup"><span data-stu-id="2a7ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a7ac-132">id</span><span class="sxs-lookup"><span data-stu-id="2a7ac-132">id</span></span>|<span data-ttu-id="2a7ac-133">String</span><span class="sxs-lookup"><span data-stu-id="2a7ac-133">String</span></span>|<span data-ttu-id="2a7ac-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-134">Key of the entity.</span></span> <span data-ttu-id="2a7ac-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2a7ac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2a7ac-136">displayName</span></span>|<span data-ttu-id="2a7ac-137">String</span><span class="sxs-lookup"><span data-stu-id="2a7ac-137">String</span></span>|<span data-ttu-id="2a7ac-138">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="2a7ac-139">description</span><span class="sxs-lookup"><span data-stu-id="2a7ac-139">description</span></span>|<span data-ttu-id="2a7ac-140">String</span><span class="sxs-lookup"><span data-stu-id="2a7ac-140">String</span></span>|<span data-ttu-id="2a7ac-141">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="2a7ac-142">permissions</span><span class="sxs-lookup"><span data-stu-id="2a7ac-142">permissions</span></span>|<span data-ttu-id="2a7ac-143">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a7ac-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2a7ac-144">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2a7ac-145">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="2a7ac-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="2a7ac-146">rolePermissions</span></span>|<span data-ttu-id="2a7ac-147">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a7ac-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2a7ac-148">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2a7ac-149">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="2a7ac-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2a7ac-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="2a7ac-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a7ac-151">Boolean</span></span>|<span data-ttu-id="2a7ac-152">角色类型。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-152">Type of Role.</span></span> <span data-ttu-id="2a7ac-153">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="2a7ac-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2a7ac-154">isBuiltIn</span></span>|<span data-ttu-id="2a7ac-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a7ac-155">Boolean</span></span>|<span data-ttu-id="2a7ac-156">角色类型。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-156">Type of Role.</span></span> <span data-ttu-id="2a7ac-157">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="2a7ac-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2a7ac-158">roleScopeTagIds</span></span>|<span data-ttu-id="2a7ac-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="2a7ac-159">String collection</span></span>|<span data-ttu-id="2a7ac-160">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2a7ac-161">响应</span><span class="sxs-lookup"><span data-stu-id="2a7ac-161">Response</span></span>
<span data-ttu-id="2a7ac-162">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-162">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a7ac-163">示例</span><span class="sxs-lookup"><span data-stu-id="2a7ac-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a7ac-164">请求</span><span class="sxs-lookup"><span data-stu-id="2a7ac-164">Request</span></span>
<span data-ttu-id="2a7ac-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="2a7ac-166">响应</span><span class="sxs-lookup"><span data-stu-id="2a7ac-166">Response</span></span>
<span data-ttu-id="2a7ac-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a7ac-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




