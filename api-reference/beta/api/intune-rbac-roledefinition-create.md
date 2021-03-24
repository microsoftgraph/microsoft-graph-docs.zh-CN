---
title: 创建 roleDefinition
description: 创建新的 roleDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f7d31dd9dab0219af303c5d03950fd572d8ebc1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141587"
---
# <a name="create-roledefinition"></a><span data-ttu-id="1dccc-103">创建 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1dccc-103">Create roleDefinition</span></span>

<span data-ttu-id="1dccc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dccc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dccc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1dccc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dccc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dccc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dccc-107">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dccc-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dccc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1dccc-108">Prerequisites</span></span>
<span data-ttu-id="1dccc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dccc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dccc-111">Permission type</span></span>|<span data-ttu-id="1dccc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1dccc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dccc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dccc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1dccc-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dccc-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1dccc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dccc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dccc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dccc-116">Not supported.</span></span>|
|<span data-ttu-id="1dccc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dccc-117">Application</span></span>|<span data-ttu-id="1dccc-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dccc-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dccc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dccc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="1dccc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dccc-120">Request headers</span></span>
|<span data-ttu-id="1dccc-121">标头</span><span class="sxs-lookup"><span data-stu-id="1dccc-121">Header</span></span>|<span data-ttu-id="1dccc-122">值</span><span class="sxs-lookup"><span data-stu-id="1dccc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dccc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dccc-123">Authorization</span></span>|<span data-ttu-id="1dccc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1dccc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dccc-125">接受</span><span class="sxs-lookup"><span data-stu-id="1dccc-125">Accept</span></span>|<span data-ttu-id="1dccc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1dccc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dccc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dccc-127">Request body</span></span>
<span data-ttu-id="1dccc-128">在请求正文中，提供 roleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dccc-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="1dccc-129">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1dccc-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="1dccc-130">属性</span><span class="sxs-lookup"><span data-stu-id="1dccc-130">Property</span></span>|<span data-ttu-id="1dccc-131">类型</span><span class="sxs-lookup"><span data-stu-id="1dccc-131">Type</span></span>|<span data-ttu-id="1dccc-132">说明</span><span class="sxs-lookup"><span data-stu-id="1dccc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dccc-133">id</span><span class="sxs-lookup"><span data-stu-id="1dccc-133">id</span></span>|<span data-ttu-id="1dccc-134">String</span><span class="sxs-lookup"><span data-stu-id="1dccc-134">String</span></span>|<span data-ttu-id="1dccc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1dccc-135">Key of the entity.</span></span> <span data-ttu-id="1dccc-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="1dccc-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="1dccc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1dccc-137">displayName</span></span>|<span data-ttu-id="1dccc-138">String</span><span class="sxs-lookup"><span data-stu-id="1dccc-138">String</span></span>|<span data-ttu-id="1dccc-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1dccc-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="1dccc-140">说明</span><span class="sxs-lookup"><span data-stu-id="1dccc-140">description</span></span>|<span data-ttu-id="1dccc-141">String</span><span class="sxs-lookup"><span data-stu-id="1dccc-141">String</span></span>|<span data-ttu-id="1dccc-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="1dccc-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="1dccc-143">权限</span><span class="sxs-lookup"><span data-stu-id="1dccc-143">permissions</span></span>|<span data-ttu-id="1dccc-144">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1dccc-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="1dccc-145">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="1dccc-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="1dccc-146">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="1dccc-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="1dccc-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="1dccc-147">rolePermissions</span></span>|<span data-ttu-id="1dccc-148">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1dccc-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="1dccc-149">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="1dccc-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="1dccc-150">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="1dccc-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="1dccc-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1dccc-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="1dccc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dccc-152">Boolean</span></span>|<span data-ttu-id="1dccc-153">角色类型。</span><span class="sxs-lookup"><span data-stu-id="1dccc-153">Type of Role.</span></span> <span data-ttu-id="1dccc-154">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="1dccc-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="1dccc-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="1dccc-155">isBuiltIn</span></span>|<span data-ttu-id="1dccc-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dccc-156">Boolean</span></span>|<span data-ttu-id="1dccc-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="1dccc-157">Type of Role.</span></span> <span data-ttu-id="1dccc-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="1dccc-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="1dccc-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1dccc-159">roleScopeTagIds</span></span>|<span data-ttu-id="1dccc-160">String collection</span><span class="sxs-lookup"><span data-stu-id="1dccc-160">String collection</span></span>|<span data-ttu-id="1dccc-161">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1dccc-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1dccc-162">响应</span><span class="sxs-lookup"><span data-stu-id="1dccc-162">Response</span></span>
<span data-ttu-id="1dccc-163">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dccc-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dccc-164">示例</span><span class="sxs-lookup"><span data-stu-id="1dccc-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dccc-165">请求</span><span class="sxs-lookup"><span data-stu-id="1dccc-165">Request</span></span>
<span data-ttu-id="1dccc-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1dccc-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dccc-167">响应</span><span class="sxs-lookup"><span data-stu-id="1dccc-167">Response</span></span>
<span data-ttu-id="1dccc-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1dccc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




