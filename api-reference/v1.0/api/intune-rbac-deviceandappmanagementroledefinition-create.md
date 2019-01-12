---
title: 创建 deviceAndAppManagementRoleDefinition
description: 创建新的 deviceAndAppManagementRoleDefinition 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 712d8a84cd70bda889aaae83fa9138a635e10acb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938298"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="130a6-103">创建 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="130a6-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="130a6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="130a6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="130a6-105">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="130a6-105">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="130a6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="130a6-106">Prerequisites</span></span>
<span data-ttu-id="130a6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="130a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130a6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="130a6-109">Permission type</span></span>|<span data-ttu-id="130a6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="130a6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="130a6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="130a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="130a6-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="130a6-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="130a6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="130a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="130a6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="130a6-114">Not supported.</span></span>|
|<span data-ttu-id="130a6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="130a6-115">Application</span></span>|<span data-ttu-id="130a6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="130a6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="130a6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="130a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="130a6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="130a6-118">Request headers</span></span>
|<span data-ttu-id="130a6-119">标头</span><span class="sxs-lookup"><span data-stu-id="130a6-119">Header</span></span>|<span data-ttu-id="130a6-120">值</span><span class="sxs-lookup"><span data-stu-id="130a6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="130a6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="130a6-121">Authorization</span></span>|<span data-ttu-id="130a6-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="130a6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="130a6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="130a6-123">Accept</span></span>|<span data-ttu-id="130a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="130a6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="130a6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="130a6-125">Request body</span></span>
<span data-ttu-id="130a6-126">在请求正文中，提供 deviceAndAppManagementRoleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="130a6-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="130a6-127">下表显示创建 deviceAndAppManagementRoleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="130a6-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="130a6-128">属性</span><span class="sxs-lookup"><span data-stu-id="130a6-128">Property</span></span>|<span data-ttu-id="130a6-129">类型</span><span class="sxs-lookup"><span data-stu-id="130a6-129">Type</span></span>|<span data-ttu-id="130a6-130">说明</span><span class="sxs-lookup"><span data-stu-id="130a6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="130a6-131">id</span><span class="sxs-lookup"><span data-stu-id="130a6-131">id</span></span>|<span data-ttu-id="130a6-132">String</span><span class="sxs-lookup"><span data-stu-id="130a6-132">String</span></span>|<span data-ttu-id="130a6-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="130a6-133">Key of the entity.</span></span> <span data-ttu-id="130a6-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="130a6-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="130a6-135">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="130a6-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="130a6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="130a6-136">displayName</span></span>|<span data-ttu-id="130a6-137">String</span><span class="sxs-lookup"><span data-stu-id="130a6-137">String</span></span>|<span data-ttu-id="130a6-138">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="130a6-138">Display Name of the Role definition.</span></span> <span data-ttu-id="130a6-139">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="130a6-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="130a6-140">description</span><span class="sxs-lookup"><span data-stu-id="130a6-140">description</span></span>|<span data-ttu-id="130a6-141">String</span><span class="sxs-lookup"><span data-stu-id="130a6-141">String</span></span>|<span data-ttu-id="130a6-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="130a6-142">Description of the Role definition.</span></span> <span data-ttu-id="130a6-143">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="130a6-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="130a6-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="130a6-144">rolePermissions</span></span>|<span data-ttu-id="130a6-145">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="130a6-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="130a6-146">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="130a6-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="130a6-147">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="130a6-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="130a6-148">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="130a6-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="130a6-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="130a6-149">isBuiltIn</span></span>|<span data-ttu-id="130a6-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="130a6-150">Boolean</span></span>|<span data-ttu-id="130a6-151">角色类型。</span><span class="sxs-lookup"><span data-stu-id="130a6-151">Type of Role.</span></span> <span data-ttu-id="130a6-152">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="130a6-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="130a6-153">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="130a6-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="130a6-154">响应</span><span class="sxs-lookup"><span data-stu-id="130a6-154">Response</span></span>
<span data-ttu-id="130a6-155">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="130a6-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130a6-156">示例</span><span class="sxs-lookup"><span data-stu-id="130a6-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="130a6-157">请求</span><span class="sxs-lookup"><span data-stu-id="130a6-157">Request</span></span>
<span data-ttu-id="130a6-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="130a6-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="130a6-159">响应</span><span class="sxs-lookup"><span data-stu-id="130a6-159">Response</span></span>
<span data-ttu-id="130a6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="130a6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```



