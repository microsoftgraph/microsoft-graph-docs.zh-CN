---
title: 更新 deviceAndAppManagementRoleDefinition
description: 更新 deviceAndAppManagementRoleDefinition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfcc2f315f528588739a780ea7f70b0207cab67d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467300"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="be9a2-103">更新 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="be9a2-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="be9a2-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be9a2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be9a2-105">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be9a2-105">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be9a2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="be9a2-106">Prerequisites</span></span>
<span data-ttu-id="be9a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be9a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be9a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be9a2-109">Permission type</span></span>|<span data-ttu-id="be9a2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be9a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be9a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be9a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be9a2-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9a2-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="be9a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be9a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be9a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be9a2-114">Not supported.</span></span>|
|<span data-ttu-id="be9a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="be9a2-115">Application</span></span>|<span data-ttu-id="be9a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be9a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be9a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be9a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="be9a2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="be9a2-118">Request headers</span></span>
|<span data-ttu-id="be9a2-119">标头</span><span class="sxs-lookup"><span data-stu-id="be9a2-119">Header</span></span>|<span data-ttu-id="be9a2-120">值</span><span class="sxs-lookup"><span data-stu-id="be9a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be9a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be9a2-121">Authorization</span></span>|<span data-ttu-id="be9a2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be9a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be9a2-123">接受</span><span class="sxs-lookup"><span data-stu-id="be9a2-123">Accept</span></span>|<span data-ttu-id="be9a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be9a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be9a2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="be9a2-125">Request body</span></span>
<span data-ttu-id="be9a2-126">在请求正文中，提供 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be9a2-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="be9a2-127">下表显示创建 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be9a2-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="be9a2-128">属性</span><span class="sxs-lookup"><span data-stu-id="be9a2-128">Property</span></span>|<span data-ttu-id="be9a2-129">类型</span><span class="sxs-lookup"><span data-stu-id="be9a2-129">Type</span></span>|<span data-ttu-id="be9a2-130">说明</span><span class="sxs-lookup"><span data-stu-id="be9a2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be9a2-131">id</span><span class="sxs-lookup"><span data-stu-id="be9a2-131">id</span></span>|<span data-ttu-id="be9a2-132">String</span><span class="sxs-lookup"><span data-stu-id="be9a2-132">String</span></span>|<span data-ttu-id="be9a2-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be9a2-133">Key of the entity.</span></span> <span data-ttu-id="be9a2-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="be9a2-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="be9a2-135">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be9a2-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="be9a2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="be9a2-136">displayName</span></span>|<span data-ttu-id="be9a2-137">String</span><span class="sxs-lookup"><span data-stu-id="be9a2-137">String</span></span>|<span data-ttu-id="be9a2-138">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be9a2-138">Display Name of the Role definition.</span></span> <span data-ttu-id="be9a2-139">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be9a2-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="be9a2-140">description</span><span class="sxs-lookup"><span data-stu-id="be9a2-140">description</span></span>|<span data-ttu-id="be9a2-141">字符串</span><span class="sxs-lookup"><span data-stu-id="be9a2-141">String</span></span>|<span data-ttu-id="be9a2-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="be9a2-142">Description of the Role definition.</span></span> <span data-ttu-id="be9a2-143">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be9a2-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="be9a2-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="be9a2-144">rolePermissions</span></span>|<span data-ttu-id="be9a2-145">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be9a2-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="be9a2-146">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="be9a2-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="be9a2-147">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="be9a2-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="be9a2-148">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be9a2-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="be9a2-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="be9a2-149">isBuiltIn</span></span>|<span data-ttu-id="be9a2-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="be9a2-150">Boolean</span></span>|<span data-ttu-id="be9a2-151">角色类型。</span><span class="sxs-lookup"><span data-stu-id="be9a2-151">Type of Role.</span></span> <span data-ttu-id="be9a2-152">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="be9a2-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="be9a2-153">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="be9a2-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="be9a2-154">响应</span><span class="sxs-lookup"><span data-stu-id="be9a2-154">Response</span></span>
<span data-ttu-id="be9a2-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be9a2-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be9a2-156">示例</span><span class="sxs-lookup"><span data-stu-id="be9a2-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="be9a2-157">请求</span><span class="sxs-lookup"><span data-stu-id="be9a2-157">Request</span></span>
<span data-ttu-id="be9a2-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be9a2-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
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

### <a name="response"></a><span data-ttu-id="be9a2-159">响应</span><span class="sxs-lookup"><span data-stu-id="be9a2-159">Response</span></span>
<span data-ttu-id="be9a2-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be9a2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



