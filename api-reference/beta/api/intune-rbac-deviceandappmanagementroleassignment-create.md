---
title: 创建 deviceAndAppManagementRoleAssignment
description: 创建新的 deviceAndAppManagementRoleAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffb7f192f7dc044ddd6e31ced38d978083f4c09b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157825"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="db222-103">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="db222-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="db222-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db222-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db222-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db222-106">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db222-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db222-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db222-107">Prerequisites</span></span>
<span data-ttu-id="db222-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db222-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db222-110">Permission type</span></span>|<span data-ttu-id="db222-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db222-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db222-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db222-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db222-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="db222-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db222-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db222-115">Not supported.</span></span>|
|<span data-ttu-id="db222-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db222-116">Application</span></span>|<span data-ttu-id="db222-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db222-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db222-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db222-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="db222-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db222-119">Request headers</span></span>
|<span data-ttu-id="db222-120">标头</span><span class="sxs-lookup"><span data-stu-id="db222-120">Header</span></span>|<span data-ttu-id="db222-121">值</span><span class="sxs-lookup"><span data-stu-id="db222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db222-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db222-122">Authorization</span></span>|<span data-ttu-id="db222-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db222-124">Accept</span><span class="sxs-lookup"><span data-stu-id="db222-124">Accept</span></span>|<span data-ttu-id="db222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db222-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db222-126">Request body</span></span>
<span data-ttu-id="db222-127">在请求正文中，提供 deviceAndAppManagementRoleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db222-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="db222-128">下表显示创建 deviceAndAppManagementRoleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db222-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="db222-129">属性</span><span class="sxs-lookup"><span data-stu-id="db222-129">Property</span></span>|<span data-ttu-id="db222-130">类型</span><span class="sxs-lookup"><span data-stu-id="db222-130">Type</span></span>|<span data-ttu-id="db222-131">说明</span><span class="sxs-lookup"><span data-stu-id="db222-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db222-132">id</span><span class="sxs-lookup"><span data-stu-id="db222-132">id</span></span>|<span data-ttu-id="db222-133">String</span><span class="sxs-lookup"><span data-stu-id="db222-133">String</span></span>|<span data-ttu-id="db222-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db222-134">Key of the entity.</span></span> <span data-ttu-id="db222-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="db222-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="db222-136">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db222-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="db222-137">displayName</span><span class="sxs-lookup"><span data-stu-id="db222-137">displayName</span></span>|<span data-ttu-id="db222-138">String</span><span class="sxs-lookup"><span data-stu-id="db222-138">String</span></span>|<span data-ttu-id="db222-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="db222-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="db222-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db222-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="db222-141">description</span><span class="sxs-lookup"><span data-stu-id="db222-141">description</span></span>|<span data-ttu-id="db222-142">String</span><span class="sxs-lookup"><span data-stu-id="db222-142">String</span></span>|<span data-ttu-id="db222-143">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="db222-143">Description of the Role Assignment.</span></span> <span data-ttu-id="db222-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db222-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="db222-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="db222-145">scopeMembers</span></span>|<span data-ttu-id="db222-146">String collection</span><span class="sxs-lookup"><span data-stu-id="db222-146">String collection</span></span>|<span data-ttu-id="db222-147">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="db222-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="db222-148">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="db222-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="db222-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db222-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="db222-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="db222-150">scopeType</span></span>|[<span data-ttu-id="db222-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="db222-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="db222-152">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="db222-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="db222-153">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="db222-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="db222-154">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="db222-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="db222-155">继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="db222-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="db222-156">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="db222-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="db222-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="db222-157">resourceScopes</span></span>|<span data-ttu-id="db222-158">String collection</span><span class="sxs-lookup"><span data-stu-id="db222-158">String collection</span></span>|<span data-ttu-id="db222-159">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="db222-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="db222-160">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="db222-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="db222-161">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db222-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="db222-162">members</span><span class="sxs-lookup"><span data-stu-id="db222-162">members</span></span>|<span data-ttu-id="db222-163">String collection</span><span class="sxs-lookup"><span data-stu-id="db222-163">String collection</span></span>|<span data-ttu-id="db222-164">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="db222-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="db222-165">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="db222-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="db222-166">响应</span><span class="sxs-lookup"><span data-stu-id="db222-166">Response</span></span>
<span data-ttu-id="db222-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db222-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db222-168">示例</span><span class="sxs-lookup"><span data-stu-id="db222-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="db222-169">请求</span><span class="sxs-lookup"><span data-stu-id="db222-169">Request</span></span>
<span data-ttu-id="db222-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db222-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="db222-171">响应</span><span class="sxs-lookup"><span data-stu-id="db222-171">Response</span></span>
<span data-ttu-id="db222-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db222-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```




