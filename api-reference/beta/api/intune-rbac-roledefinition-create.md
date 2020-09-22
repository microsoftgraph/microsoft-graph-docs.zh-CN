---
title: 创建 roleDefinition
description: 创建新的 roleDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 232bbb563f0ef687f222bb6a2509616110d19646
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056000"
---
# <a name="create-roledefinition"></a><span data-ttu-id="4b9be-103">创建 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4b9be-103">Create roleDefinition</span></span>

<span data-ttu-id="4b9be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b9be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b9be-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b9be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b9be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b9be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b9be-107">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b9be-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b9be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b9be-108">Prerequisites</span></span>
<span data-ttu-id="4b9be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b9be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b9be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b9be-111">Permission type</span></span>|<span data-ttu-id="4b9be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b9be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b9be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b9be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b9be-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b9be-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4b9be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b9be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b9be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b9be-116">Not supported.</span></span>|
|<span data-ttu-id="4b9be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b9be-117">Application</span></span>|<span data-ttu-id="4b9be-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b9be-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b9be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b9be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="4b9be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b9be-120">Request headers</span></span>
|<span data-ttu-id="4b9be-121">标头</span><span class="sxs-lookup"><span data-stu-id="4b9be-121">Header</span></span>|<span data-ttu-id="4b9be-122">值</span><span class="sxs-lookup"><span data-stu-id="4b9be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b9be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b9be-123">Authorization</span></span>|<span data-ttu-id="4b9be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b9be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b9be-125">接受</span><span class="sxs-lookup"><span data-stu-id="4b9be-125">Accept</span></span>|<span data-ttu-id="4b9be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b9be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b9be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b9be-127">Request body</span></span>
<span data-ttu-id="4b9be-128">在请求正文中，提供 roleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b9be-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="4b9be-129">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4b9be-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="4b9be-130">属性</span><span class="sxs-lookup"><span data-stu-id="4b9be-130">Property</span></span>|<span data-ttu-id="4b9be-131">类型</span><span class="sxs-lookup"><span data-stu-id="4b9be-131">Type</span></span>|<span data-ttu-id="4b9be-132">说明</span><span class="sxs-lookup"><span data-stu-id="4b9be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b9be-133">id</span><span class="sxs-lookup"><span data-stu-id="4b9be-133">id</span></span>|<span data-ttu-id="4b9be-134">String</span><span class="sxs-lookup"><span data-stu-id="4b9be-134">String</span></span>|<span data-ttu-id="4b9be-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4b9be-135">Key of the entity.</span></span> <span data-ttu-id="4b9be-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="4b9be-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="4b9be-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4b9be-137">displayName</span></span>|<span data-ttu-id="4b9be-138">String</span><span class="sxs-lookup"><span data-stu-id="4b9be-138">String</span></span>|<span data-ttu-id="4b9be-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4b9be-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="4b9be-140">说明</span><span class="sxs-lookup"><span data-stu-id="4b9be-140">description</span></span>|<span data-ttu-id="4b9be-141">String</span><span class="sxs-lookup"><span data-stu-id="4b9be-141">String</span></span>|<span data-ttu-id="4b9be-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="4b9be-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="4b9be-143">permissions</span><span class="sxs-lookup"><span data-stu-id="4b9be-143">permissions</span></span>|<span data-ttu-id="4b9be-144">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b9be-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4b9be-145">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="4b9be-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4b9be-146">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="4b9be-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4b9be-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="4b9be-147">rolePermissions</span></span>|<span data-ttu-id="4b9be-148">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b9be-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4b9be-149">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="4b9be-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4b9be-150">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="4b9be-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4b9be-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4b9be-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="4b9be-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b9be-152">Boolean</span></span>|<span data-ttu-id="4b9be-153">角色类型。</span><span class="sxs-lookup"><span data-stu-id="4b9be-153">Type of Role.</span></span> <span data-ttu-id="4b9be-154">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="4b9be-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="4b9be-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4b9be-155">isBuiltIn</span></span>|<span data-ttu-id="4b9be-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b9be-156">Boolean</span></span>|<span data-ttu-id="4b9be-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="4b9be-157">Type of Role.</span></span> <span data-ttu-id="4b9be-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="4b9be-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="4b9be-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b9be-159">roleScopeTagIds</span></span>|<span data-ttu-id="4b9be-160">String 集合</span><span class="sxs-lookup"><span data-stu-id="4b9be-160">String collection</span></span>|<span data-ttu-id="4b9be-161">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4b9be-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="4b9be-162">响应</span><span class="sxs-lookup"><span data-stu-id="4b9be-162">Response</span></span>
<span data-ttu-id="4b9be-163">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b9be-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b9be-164">示例</span><span class="sxs-lookup"><span data-stu-id="4b9be-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b9be-165">请求</span><span class="sxs-lookup"><span data-stu-id="4b9be-165">Request</span></span>
<span data-ttu-id="4b9be-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b9be-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b9be-167">响应</span><span class="sxs-lookup"><span data-stu-id="4b9be-167">Response</span></span>
<span data-ttu-id="4b9be-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b9be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






