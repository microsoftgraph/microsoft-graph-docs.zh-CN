---
title: 创建 deviceAndAppManagementRoleDefinition
description: 创建新的 deviceAndAppManagementRoleDefinition 对象。
author: tfitzmac
ms.openlocfilehash: fdf6e4b1a4c80456c51b8a155974c5cd8d9728bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339940"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="3b08d-103">创建 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b08d-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="3b08d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3b08d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b08d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b08d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b08d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3b08d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b08d-107">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b08d-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b08d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b08d-108">Prerequisites</span></span>
<span data-ttu-id="3b08d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3b08d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b08d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b08d-111">Permission type</span></span>|<span data-ttu-id="3b08d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b08d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b08d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b08d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b08d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b08d-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3b08d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b08d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b08d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b08d-116">Not supported.</span></span>|
|<span data-ttu-id="3b08d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b08d-117">Application</span></span>|<span data-ttu-id="3b08d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b08d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b08d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b08d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3b08d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b08d-120">Request headers</span></span>
|<span data-ttu-id="3b08d-121">标头</span><span class="sxs-lookup"><span data-stu-id="3b08d-121">Header</span></span>|<span data-ttu-id="3b08d-122">值</span><span class="sxs-lookup"><span data-stu-id="3b08d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b08d-123">授权</span><span class="sxs-lookup"><span data-stu-id="3b08d-123">Authorization</span></span>|<span data-ttu-id="3b08d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b08d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b08d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b08d-125">Accept</span></span>|<span data-ttu-id="3b08d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b08d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b08d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b08d-127">Request body</span></span>
<span data-ttu-id="3b08d-128">在请求正文中，提供 deviceAndAppManagementRoleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b08d-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="3b08d-129">下表显示创建 deviceAndAppManagementRoleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b08d-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="3b08d-130">属性</span><span class="sxs-lookup"><span data-stu-id="3b08d-130">Property</span></span>|<span data-ttu-id="3b08d-131">类型</span><span class="sxs-lookup"><span data-stu-id="3b08d-131">Type</span></span>|<span data-ttu-id="3b08d-132">说明</span><span class="sxs-lookup"><span data-stu-id="3b08d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b08d-133">id</span><span class="sxs-lookup"><span data-stu-id="3b08d-133">id</span></span>|<span data-ttu-id="3b08d-134">String</span><span class="sxs-lookup"><span data-stu-id="3b08d-134">String</span></span>|<span data-ttu-id="3b08d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b08d-135">Key of the entity.</span></span> <span data-ttu-id="3b08d-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="3b08d-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="3b08d-137">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3b08d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3b08d-138">displayName</span></span>|<span data-ttu-id="3b08d-139">String</span><span class="sxs-lookup"><span data-stu-id="3b08d-139">String</span></span>|<span data-ttu-id="3b08d-140">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3b08d-140">Display Name of the Role definition.</span></span> <span data-ttu-id="3b08d-141">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3b08d-142">description</span><span class="sxs-lookup"><span data-stu-id="3b08d-142">description</span></span>|<span data-ttu-id="3b08d-143">String</span><span class="sxs-lookup"><span data-stu-id="3b08d-143">String</span></span>|<span data-ttu-id="3b08d-144">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="3b08d-144">Description of the Role definition.</span></span> <span data-ttu-id="3b08d-145">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3b08d-146">permissions</span><span class="sxs-lookup"><span data-stu-id="3b08d-146">permissions</span></span>|<span data-ttu-id="3b08d-147">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b08d-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3b08d-148">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="3b08d-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3b08d-149">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="3b08d-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3b08d-150">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3b08d-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3b08d-151">rolePermissions</span></span>|<span data-ttu-id="3b08d-152">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b08d-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3b08d-153">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="3b08d-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3b08d-154">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="3b08d-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3b08d-155">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3b08d-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b08d-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3b08d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b08d-157">Boolean</span></span>|<span data-ttu-id="3b08d-158">角色类型。</span><span class="sxs-lookup"><span data-stu-id="3b08d-158">Type of Role.</span></span> <span data-ttu-id="3b08d-159">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="3b08d-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3b08d-160">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3b08d-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3b08d-161">isBuiltIn</span></span>|<span data-ttu-id="3b08d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b08d-162">Boolean</span></span>|<span data-ttu-id="3b08d-163">角色类型。</span><span class="sxs-lookup"><span data-stu-id="3b08d-163">Type of Role.</span></span> <span data-ttu-id="3b08d-164">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="3b08d-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3b08d-165">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b08d-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3b08d-166">响应</span><span class="sxs-lookup"><span data-stu-id="3b08d-166">Response</span></span>
<span data-ttu-id="3b08d-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b08d-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b08d-168">示例</span><span class="sxs-lookup"><span data-stu-id="3b08d-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b08d-169">请求</span><span class="sxs-lookup"><span data-stu-id="3b08d-169">Request</span></span>
<span data-ttu-id="3b08d-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b08d-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1167

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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="3b08d-171">响应</span><span class="sxs-lookup"><span data-stu-id="3b08d-171">Response</span></span>
<span data-ttu-id="3b08d-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b08d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1216

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
  "isBuiltIn": true
}
```





