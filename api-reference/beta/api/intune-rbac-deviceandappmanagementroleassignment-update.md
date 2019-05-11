---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 022ae5e4efb63e2eea2893de7058e44976b18bd8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899653"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="b2a18-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b2a18-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="b2a18-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2a18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2a18-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2a18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2a18-106">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b2a18-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2a18-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2a18-107">Prerequisites</span></span>
<span data-ttu-id="b2a18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2a18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2a18-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2a18-110">Permission type</span></span>|<span data-ttu-id="b2a18-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2a18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2a18-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2a18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2a18-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2a18-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b2a18-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2a18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2a18-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2a18-115">Not supported.</span></span>|
|<span data-ttu-id="b2a18-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2a18-116">Application</span></span>|<span data-ttu-id="b2a18-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2a18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2a18-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2a18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b2a18-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2a18-119">Request headers</span></span>
|<span data-ttu-id="b2a18-120">标头</span><span class="sxs-lookup"><span data-stu-id="b2a18-120">Header</span></span>|<span data-ttu-id="b2a18-121">值</span><span class="sxs-lookup"><span data-stu-id="b2a18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2a18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2a18-122">Authorization</span></span>|<span data-ttu-id="b2a18-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2a18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2a18-124">接受</span><span class="sxs-lookup"><span data-stu-id="b2a18-124">Accept</span></span>|<span data-ttu-id="b2a18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2a18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2a18-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2a18-126">Request body</span></span>
<span data-ttu-id="b2a18-127">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2a18-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="b2a18-128">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2a18-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="b2a18-129">属性</span><span class="sxs-lookup"><span data-stu-id="b2a18-129">Property</span></span>|<span data-ttu-id="b2a18-130">类型</span><span class="sxs-lookup"><span data-stu-id="b2a18-130">Type</span></span>|<span data-ttu-id="b2a18-131">说明</span><span class="sxs-lookup"><span data-stu-id="b2a18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2a18-132">id</span><span class="sxs-lookup"><span data-stu-id="b2a18-132">id</span></span>|<span data-ttu-id="b2a18-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b2a18-133">String</span></span>|<span data-ttu-id="b2a18-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b2a18-134">Key of the entity.</span></span> <span data-ttu-id="b2a18-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="b2a18-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="b2a18-136">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2a18-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2a18-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b2a18-137">displayName</span></span>|<span data-ttu-id="b2a18-138">String</span><span class="sxs-lookup"><span data-stu-id="b2a18-138">String</span></span>|<span data-ttu-id="b2a18-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="b2a18-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="b2a18-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2a18-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2a18-141">说明</span><span class="sxs-lookup"><span data-stu-id="b2a18-141">description</span></span>|<span data-ttu-id="b2a18-142">String</span><span class="sxs-lookup"><span data-stu-id="b2a18-142">String</span></span>|<span data-ttu-id="b2a18-143">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="b2a18-143">Description of the Role Assignment.</span></span> <span data-ttu-id="b2a18-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2a18-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2a18-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="b2a18-145">scopeMembers</span></span>|<span data-ttu-id="b2a18-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b2a18-146">String collection</span></span>|<span data-ttu-id="b2a18-147">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b2a18-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b2a18-148">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2a18-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b2a18-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2a18-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2a18-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="b2a18-150">scopeType</span></span>|[<span data-ttu-id="b2a18-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="b2a18-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="b2a18-152">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="b2a18-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="b2a18-153">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="b2a18-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="b2a18-154">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="b2a18-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="b2a18-155">继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="b2a18-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="b2a18-156">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="b2a18-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="b2a18-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b2a18-157">resourceScopes</span></span>|<span data-ttu-id="b2a18-158">String collection</span><span class="sxs-lookup"><span data-stu-id="b2a18-158">String collection</span></span>|<span data-ttu-id="b2a18-159">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b2a18-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b2a18-160">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2a18-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b2a18-161">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2a18-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2a18-162">members</span><span class="sxs-lookup"><span data-stu-id="b2a18-162">members</span></span>|<span data-ttu-id="b2a18-163">String collection</span><span class="sxs-lookup"><span data-stu-id="b2a18-163">String collection</span></span>|<span data-ttu-id="b2a18-164">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b2a18-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="b2a18-165">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2a18-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b2a18-166">响应</span><span class="sxs-lookup"><span data-stu-id="b2a18-166">Response</span></span>
<span data-ttu-id="b2a18-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2a18-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2a18-168">示例</span><span class="sxs-lookup"><span data-stu-id="b2a18-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2a18-169">请求</span><span class="sxs-lookup"><span data-stu-id="b2a18-169">Request</span></span>
<span data-ttu-id="b2a18-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2a18-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="b2a18-171">响应</span><span class="sxs-lookup"><span data-stu-id="b2a18-171">Response</span></span>
<span data-ttu-id="b2a18-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2a18-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




