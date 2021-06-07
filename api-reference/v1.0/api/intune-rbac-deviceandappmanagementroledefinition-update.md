---
title: 更新 deviceAndAppManagementRoleDefinition
description: 更新 deviceAndAppManagementRoleDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e7ad1fd0ad74df9e81ceeafc599e795a91f7f68c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756882"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="daecd-103">更新 deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="daecd-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="daecd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daecd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daecd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="daecd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daecd-106">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="daecd-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daecd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="daecd-107">Prerequisites</span></span>
<span data-ttu-id="daecd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="daecd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daecd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="daecd-110">Permission type</span></span>|<span data-ttu-id="daecd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="daecd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daecd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="daecd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="daecd-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daecd-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="daecd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="daecd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daecd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="daecd-115">Not supported.</span></span>|
|<span data-ttu-id="daecd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="daecd-116">Application</span></span>|<span data-ttu-id="daecd-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daecd-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daecd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="daecd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="daecd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="daecd-119">Request headers</span></span>
|<span data-ttu-id="daecd-120">标头</span><span class="sxs-lookup"><span data-stu-id="daecd-120">Header</span></span>|<span data-ttu-id="daecd-121">值</span><span class="sxs-lookup"><span data-stu-id="daecd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daecd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="daecd-122">Authorization</span></span>|<span data-ttu-id="daecd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="daecd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daecd-124">接受</span><span class="sxs-lookup"><span data-stu-id="daecd-124">Accept</span></span>|<span data-ttu-id="daecd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="daecd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daecd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="daecd-126">Request body</span></span>
<span data-ttu-id="daecd-127">在请求正文中，提供 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daecd-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="daecd-128">下表显示创建 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="daecd-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="daecd-129">属性</span><span class="sxs-lookup"><span data-stu-id="daecd-129">Property</span></span>|<span data-ttu-id="daecd-130">类型</span><span class="sxs-lookup"><span data-stu-id="daecd-130">Type</span></span>|<span data-ttu-id="daecd-131">说明</span><span class="sxs-lookup"><span data-stu-id="daecd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daecd-132">id</span><span class="sxs-lookup"><span data-stu-id="daecd-132">id</span></span>|<span data-ttu-id="daecd-133">String</span><span class="sxs-lookup"><span data-stu-id="daecd-133">String</span></span>|<span data-ttu-id="daecd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="daecd-134">Key of the entity.</span></span> <span data-ttu-id="daecd-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="daecd-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="daecd-136">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="daecd-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="daecd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="daecd-137">displayName</span></span>|<span data-ttu-id="daecd-138">String</span><span class="sxs-lookup"><span data-stu-id="daecd-138">String</span></span>|<span data-ttu-id="daecd-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="daecd-139">Display Name of the Role definition.</span></span> <span data-ttu-id="daecd-140">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="daecd-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="daecd-141">说明</span><span class="sxs-lookup"><span data-stu-id="daecd-141">description</span></span>|<span data-ttu-id="daecd-142">String</span><span class="sxs-lookup"><span data-stu-id="daecd-142">String</span></span>|<span data-ttu-id="daecd-143">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="daecd-143">Description of the Role definition.</span></span> <span data-ttu-id="daecd-144">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="daecd-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="daecd-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="daecd-145">rolePermissions</span></span>|<span data-ttu-id="daecd-146">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="daecd-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="daecd-147">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="daecd-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="daecd-148">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="daecd-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="daecd-149">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="daecd-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="daecd-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="daecd-150">isBuiltIn</span></span>|<span data-ttu-id="daecd-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="daecd-151">Boolean</span></span>|<span data-ttu-id="daecd-152">角色类型。</span><span class="sxs-lookup"><span data-stu-id="daecd-152">Type of Role.</span></span> <span data-ttu-id="daecd-153">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="daecd-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="daecd-154">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="daecd-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="daecd-155">响应</span><span class="sxs-lookup"><span data-stu-id="daecd-155">Response</span></span>
<span data-ttu-id="daecd-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="daecd-156">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daecd-157">示例</span><span class="sxs-lookup"><span data-stu-id="daecd-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="daecd-158">请求</span><span class="sxs-lookup"><span data-stu-id="daecd-158">Request</span></span>
<span data-ttu-id="daecd-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="daecd-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="daecd-160">响应</span><span class="sxs-lookup"><span data-stu-id="daecd-160">Response</span></span>
<span data-ttu-id="daecd-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="daecd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




