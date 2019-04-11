---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711edd13e1a9a7627dccde60c6522dea346a8a93
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795392"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="3ec64-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3ec64-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="3ec64-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ec64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ec64-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ec64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ec64-106">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3ec64-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ec64-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ec64-107">Prerequisites</span></span>
<span data-ttu-id="3ec64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ec64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ec64-110">Permission type</span></span>|<span data-ttu-id="3ec64-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3ec64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ec64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ec64-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec64-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3ec64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ec64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec64-115">Not supported.</span></span>|
|<span data-ttu-id="3ec64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec64-116">Application</span></span>|<span data-ttu-id="3ec64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ec64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ec64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3ec64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec64-119">Request headers</span></span>
|<span data-ttu-id="3ec64-120">标头</span><span class="sxs-lookup"><span data-stu-id="3ec64-120">Header</span></span>|<span data-ttu-id="3ec64-121">值</span><span class="sxs-lookup"><span data-stu-id="3ec64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ec64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec64-122">Authorization</span></span>|<span data-ttu-id="3ec64-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ec64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ec64-124">接受</span><span class="sxs-lookup"><span data-stu-id="3ec64-124">Accept</span></span>|<span data-ttu-id="3ec64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ec64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec64-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec64-126">Request body</span></span>
<span data-ttu-id="3ec64-127">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ec64-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="3ec64-128">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3ec64-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="3ec64-129">属性</span><span class="sxs-lookup"><span data-stu-id="3ec64-129">Property</span></span>|<span data-ttu-id="3ec64-130">类型</span><span class="sxs-lookup"><span data-stu-id="3ec64-130">Type</span></span>|<span data-ttu-id="3ec64-131">说明</span><span class="sxs-lookup"><span data-stu-id="3ec64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ec64-132">id</span><span class="sxs-lookup"><span data-stu-id="3ec64-132">id</span></span>|<span data-ttu-id="3ec64-133">String</span><span class="sxs-lookup"><span data-stu-id="3ec64-133">String</span></span>|<span data-ttu-id="3ec64-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3ec64-134">Key of the entity.</span></span> <span data-ttu-id="3ec64-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="3ec64-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="3ec64-136">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ec64-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="3ec64-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3ec64-137">displayName</span></span>|<span data-ttu-id="3ec64-138">String</span><span class="sxs-lookup"><span data-stu-id="3ec64-138">String</span></span>|<span data-ttu-id="3ec64-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="3ec64-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="3ec64-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ec64-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="3ec64-141">description</span><span class="sxs-lookup"><span data-stu-id="3ec64-141">description</span></span>|<span data-ttu-id="3ec64-142">String</span><span class="sxs-lookup"><span data-stu-id="3ec64-142">String</span></span>|<span data-ttu-id="3ec64-143">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="3ec64-143">Description of the Role Assignment.</span></span> <span data-ttu-id="3ec64-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ec64-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="3ec64-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="3ec64-145">scopeMembers</span></span>|<span data-ttu-id="3ec64-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="3ec64-146">String collection</span></span>|<span data-ttu-id="3ec64-147">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="3ec64-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="3ec64-148">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3ec64-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="3ec64-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ec64-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="3ec64-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="3ec64-150">scopeType</span></span>|[<span data-ttu-id="3ec64-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="3ec64-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="3ec64-152">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="3ec64-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="3ec64-153">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="3ec64-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="3ec64-154">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="3ec64-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="3ec64-155">继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="3ec64-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="3ec64-156">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="3ec64-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="3ec64-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="3ec64-157">resourceScopes</span></span>|<span data-ttu-id="3ec64-158">String 集合</span><span class="sxs-lookup"><span data-stu-id="3ec64-158">String collection</span></span>|<span data-ttu-id="3ec64-159">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="3ec64-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="3ec64-160">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3ec64-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="3ec64-161">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ec64-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="3ec64-162">members</span><span class="sxs-lookup"><span data-stu-id="3ec64-162">members</span></span>|<span data-ttu-id="3ec64-163">String collection</span><span class="sxs-lookup"><span data-stu-id="3ec64-163">String collection</span></span>|<span data-ttu-id="3ec64-164">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="3ec64-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="3ec64-165">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="3ec64-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="3ec64-166">响应</span><span class="sxs-lookup"><span data-stu-id="3ec64-166">Response</span></span>
<span data-ttu-id="3ec64-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec64-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec64-168">示例</span><span class="sxs-lookup"><span data-stu-id="3ec64-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ec64-169">请求</span><span class="sxs-lookup"><span data-stu-id="3ec64-169">Request</span></span>
<span data-ttu-id="3ec64-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec64-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ec64-171">响应</span><span class="sxs-lookup"><span data-stu-id="3ec64-171">Response</span></span>
<span data-ttu-id="3ec64-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ec64-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





