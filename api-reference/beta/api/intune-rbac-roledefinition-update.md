---
title: 更新 roleDefinition
description: 更新 roleDefinition 对象的属性。
ms.openlocfilehash: debf63b5d0b7116a1e8d1f9274868d97c3cb8931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042108"
---
# <a name="update-roledefinition"></a><span data-ttu-id="8732b-103">更新 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8732b-103">Update roleDefinition</span></span>

> <span data-ttu-id="8732b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8732b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8732b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8732b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8732b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8732b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8732b-107">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8732b-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8732b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8732b-108">Prerequisites</span></span>
<span data-ttu-id="8732b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8732b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8732b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8732b-111">Permission type</span></span>|<span data-ttu-id="8732b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8732b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8732b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8732b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8732b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8732b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8732b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8732b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8732b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8732b-116">Not supported.</span></span>|
|<span data-ttu-id="8732b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8732b-117">Application</span></span>|<span data-ttu-id="8732b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8732b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8732b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8732b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="8732b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8732b-120">Request headers</span></span>
|<span data-ttu-id="8732b-121">标头</span><span class="sxs-lookup"><span data-stu-id="8732b-121">Header</span></span>|<span data-ttu-id="8732b-122">值</span><span class="sxs-lookup"><span data-stu-id="8732b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8732b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8732b-123">Authorization</span></span>|<span data-ttu-id="8732b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8732b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8732b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8732b-125">Accept</span></span>|<span data-ttu-id="8732b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8732b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8732b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8732b-127">Request body</span></span>
<span data-ttu-id="8732b-128">在请求正文中，提供 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8732b-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="8732b-129">下表显示创建 [roleDefinition](../resources/intune-rbac-roledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8732b-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="8732b-130">属性</span><span class="sxs-lookup"><span data-stu-id="8732b-130">Property</span></span>|<span data-ttu-id="8732b-131">类型</span><span class="sxs-lookup"><span data-stu-id="8732b-131">Type</span></span>|<span data-ttu-id="8732b-132">说明</span><span class="sxs-lookup"><span data-stu-id="8732b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8732b-133">id</span><span class="sxs-lookup"><span data-stu-id="8732b-133">id</span></span>|<span data-ttu-id="8732b-134">String</span><span class="sxs-lookup"><span data-stu-id="8732b-134">String</span></span>|<span data-ttu-id="8732b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8732b-135">Key of the entity.</span></span> <span data-ttu-id="8732b-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="8732b-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="8732b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8732b-137">displayName</span></span>|<span data-ttu-id="8732b-138">String</span><span class="sxs-lookup"><span data-stu-id="8732b-138">String</span></span>|<span data-ttu-id="8732b-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8732b-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="8732b-140">说明</span><span class="sxs-lookup"><span data-stu-id="8732b-140">description</span></span>|<span data-ttu-id="8732b-141">String</span><span class="sxs-lookup"><span data-stu-id="8732b-141">String</span></span>|<span data-ttu-id="8732b-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="8732b-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="8732b-143">permissions</span><span class="sxs-lookup"><span data-stu-id="8732b-143">permissions</span></span>|<span data-ttu-id="8732b-144">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8732b-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8732b-145">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="8732b-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8732b-146">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="8732b-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="8732b-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8732b-147">rolePermissions</span></span>|<span data-ttu-id="8732b-148">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8732b-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8732b-149">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="8732b-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8732b-150">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="8732b-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="8732b-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8732b-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="8732b-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="8732b-152">Boolean</span></span>|<span data-ttu-id="8732b-153">角色类型。</span><span class="sxs-lookup"><span data-stu-id="8732b-153">Type of Role.</span></span> <span data-ttu-id="8732b-154">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="8732b-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="8732b-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8732b-155">isBuiltIn</span></span>|<span data-ttu-id="8732b-156">布尔值</span><span class="sxs-lookup"><span data-stu-id="8732b-156">Boolean</span></span>|<span data-ttu-id="8732b-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="8732b-157">Type of Role.</span></span> <span data-ttu-id="8732b-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="8732b-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="8732b-159">响应</span><span class="sxs-lookup"><span data-stu-id="8732b-159">Response</span></span>
<span data-ttu-id="8732b-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8732b-160">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8732b-161">示例</span><span class="sxs-lookup"><span data-stu-id="8732b-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="8732b-162">请求</span><span class="sxs-lookup"><span data-stu-id="8732b-162">Request</span></span>
<span data-ttu-id="8732b-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8732b-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1092

{
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

### <a name="response"></a><span data-ttu-id="8732b-164">响应</span><span class="sxs-lookup"><span data-stu-id="8732b-164">Response</span></span>
<span data-ttu-id="8732b-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8732b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1194

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
  "isBuiltIn": true
}
```





