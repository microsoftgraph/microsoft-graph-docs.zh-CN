---
title: 创建 deviceAndAppManagementRoleDefinition
description: 创建新的 deviceAndAppManagementRoleDefinition 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bc5438b9d0d4db833949cc4ee84d9d43785b6e2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926104"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="912ad-103">创建 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="912ad-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="912ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="912ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="912ad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="912ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="912ad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="912ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="912ad-107">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="912ad-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="912ad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="912ad-108">Prerequisites</span></span>
<span data-ttu-id="912ad-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="912ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="912ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="912ad-111">Permission type</span></span>|<span data-ttu-id="912ad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="912ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="912ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="912ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="912ad-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912ad-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="912ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="912ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="912ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="912ad-116">Not supported.</span></span>|
|<span data-ttu-id="912ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="912ad-117">Application</span></span>|<span data-ttu-id="912ad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="912ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="912ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="912ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="912ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="912ad-120">Request headers</span></span>
|<span data-ttu-id="912ad-121">标头</span><span class="sxs-lookup"><span data-stu-id="912ad-121">Header</span></span>|<span data-ttu-id="912ad-122">值</span><span class="sxs-lookup"><span data-stu-id="912ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="912ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="912ad-123">Authorization</span></span>|<span data-ttu-id="912ad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="912ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="912ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="912ad-125">Accept</span></span>|<span data-ttu-id="912ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="912ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="912ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="912ad-127">Request body</span></span>
<span data-ttu-id="912ad-128">在请求正文中，提供 deviceAndAppManagementRoleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="912ad-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="912ad-129">下表显示创建 deviceAndAppManagementRoleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="912ad-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="912ad-130">属性</span><span class="sxs-lookup"><span data-stu-id="912ad-130">Property</span></span>|<span data-ttu-id="912ad-131">类型</span><span class="sxs-lookup"><span data-stu-id="912ad-131">Type</span></span>|<span data-ttu-id="912ad-132">说明</span><span class="sxs-lookup"><span data-stu-id="912ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="912ad-133">id</span><span class="sxs-lookup"><span data-stu-id="912ad-133">id</span></span>|<span data-ttu-id="912ad-134">String</span><span class="sxs-lookup"><span data-stu-id="912ad-134">String</span></span>|<span data-ttu-id="912ad-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="912ad-135">Key of the entity.</span></span> <span data-ttu-id="912ad-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="912ad-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="912ad-137">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="912ad-138">displayName</span><span class="sxs-lookup"><span data-stu-id="912ad-138">displayName</span></span>|<span data-ttu-id="912ad-139">String</span><span class="sxs-lookup"><span data-stu-id="912ad-139">String</span></span>|<span data-ttu-id="912ad-140">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="912ad-140">Display Name of the Role definition.</span></span> <span data-ttu-id="912ad-141">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="912ad-142">description</span><span class="sxs-lookup"><span data-stu-id="912ad-142">description</span></span>|<span data-ttu-id="912ad-143">String</span><span class="sxs-lookup"><span data-stu-id="912ad-143">String</span></span>|<span data-ttu-id="912ad-144">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="912ad-144">Description of the Role definition.</span></span> <span data-ttu-id="912ad-145">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="912ad-146">permissions</span><span class="sxs-lookup"><span data-stu-id="912ad-146">permissions</span></span>|<span data-ttu-id="912ad-147">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="912ad-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="912ad-148">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="912ad-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="912ad-149">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="912ad-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="912ad-150">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="912ad-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="912ad-151">rolePermissions</span></span>|<span data-ttu-id="912ad-152">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="912ad-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="912ad-153">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="912ad-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="912ad-154">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="912ad-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="912ad-155">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="912ad-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="912ad-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="912ad-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="912ad-157">Boolean</span></span>|<span data-ttu-id="912ad-158">角色类型。</span><span class="sxs-lookup"><span data-stu-id="912ad-158">Type of Role.</span></span> <span data-ttu-id="912ad-159">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="912ad-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="912ad-160">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="912ad-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="912ad-161">isBuiltIn</span></span>|<span data-ttu-id="912ad-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="912ad-162">Boolean</span></span>|<span data-ttu-id="912ad-163">角色类型。</span><span class="sxs-lookup"><span data-stu-id="912ad-163">Type of Role.</span></span> <span data-ttu-id="912ad-164">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="912ad-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="912ad-165">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="912ad-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="912ad-166">响应</span><span class="sxs-lookup"><span data-stu-id="912ad-166">Response</span></span>
<span data-ttu-id="912ad-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="912ad-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="912ad-168">示例</span><span class="sxs-lookup"><span data-stu-id="912ad-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="912ad-169">请求</span><span class="sxs-lookup"><span data-stu-id="912ad-169">Request</span></span>
<span data-ttu-id="912ad-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="912ad-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="912ad-171">响应</span><span class="sxs-lookup"><span data-stu-id="912ad-171">Response</span></span>
<span data-ttu-id="912ad-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="912ad-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





