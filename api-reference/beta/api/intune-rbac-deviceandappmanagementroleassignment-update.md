---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0de5546e35e9fb850dfef7932ec24f3a821fecb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044961"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="7c087-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7c087-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="7c087-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c087-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c087-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c087-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c087-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c087-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c087-107">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c087-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c087-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7c087-108">Prerequisites</span></span>
<span data-ttu-id="7c087-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c087-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c087-111">Permission type</span></span>|<span data-ttu-id="7c087-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7c087-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c087-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c087-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c087-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c087-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7c087-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c087-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c087-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c087-116">Not supported.</span></span>|
|<span data-ttu-id="7c087-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c087-117">Application</span></span>|<span data-ttu-id="7c087-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c087-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c087-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c087-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7c087-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c087-120">Request headers</span></span>
|<span data-ttu-id="7c087-121">标头</span><span class="sxs-lookup"><span data-stu-id="7c087-121">Header</span></span>|<span data-ttu-id="7c087-122">值</span><span class="sxs-lookup"><span data-stu-id="7c087-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c087-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c087-123">Authorization</span></span>|<span data-ttu-id="7c087-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7c087-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c087-125">接受</span><span class="sxs-lookup"><span data-stu-id="7c087-125">Accept</span></span>|<span data-ttu-id="7c087-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c087-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c087-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c087-127">Request body</span></span>
<span data-ttu-id="7c087-128">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c087-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="7c087-129">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7c087-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="7c087-130">属性</span><span class="sxs-lookup"><span data-stu-id="7c087-130">Property</span></span>|<span data-ttu-id="7c087-131">类型</span><span class="sxs-lookup"><span data-stu-id="7c087-131">Type</span></span>|<span data-ttu-id="7c087-132">说明</span><span class="sxs-lookup"><span data-stu-id="7c087-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c087-133">id</span><span class="sxs-lookup"><span data-stu-id="7c087-133">id</span></span>|<span data-ttu-id="7c087-134">String</span><span class="sxs-lookup"><span data-stu-id="7c087-134">String</span></span>|<span data-ttu-id="7c087-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7c087-135">Key of the entity.</span></span> <span data-ttu-id="7c087-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="7c087-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="7c087-137">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c087-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7c087-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7c087-138">displayName</span></span>|<span data-ttu-id="7c087-139">String</span><span class="sxs-lookup"><span data-stu-id="7c087-139">String</span></span>|<span data-ttu-id="7c087-140">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="7c087-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="7c087-141">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c087-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7c087-142">description</span><span class="sxs-lookup"><span data-stu-id="7c087-142">description</span></span>|<span data-ttu-id="7c087-143">String</span><span class="sxs-lookup"><span data-stu-id="7c087-143">String</span></span>|<span data-ttu-id="7c087-144">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="7c087-144">Description of the Role Assignment.</span></span> <span data-ttu-id="7c087-145">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c087-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7c087-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="7c087-146">scopeMembers</span></span>|<span data-ttu-id="7c087-147">String collection</span><span class="sxs-lookup"><span data-stu-id="7c087-147">String collection</span></span>|<span data-ttu-id="7c087-148">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="7c087-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7c087-149">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c087-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="7c087-150">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c087-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7c087-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="7c087-151">scopeType</span></span>|[<span data-ttu-id="7c087-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="7c087-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="7c087-153">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="7c087-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="7c087-154">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="7c087-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="7c087-155">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers"，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="7c087-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="7c087-156">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7c087-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="7c087-157">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="7c087-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="7c087-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7c087-158">resourceScopes</span></span>|<span data-ttu-id="7c087-159">String collection</span><span class="sxs-lookup"><span data-stu-id="7c087-159">String collection</span></span>|<span data-ttu-id="7c087-160">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="7c087-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7c087-161">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c087-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="7c087-162">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c087-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7c087-163">members</span><span class="sxs-lookup"><span data-stu-id="7c087-163">members</span></span>|<span data-ttu-id="7c087-164">String collection</span><span class="sxs-lookup"><span data-stu-id="7c087-164">String collection</span></span>|<span data-ttu-id="7c087-165">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="7c087-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="7c087-166">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c087-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="7c087-167">响应</span><span class="sxs-lookup"><span data-stu-id="7c087-167">Response</span></span>
<span data-ttu-id="7c087-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c087-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c087-169">示例</span><span class="sxs-lookup"><span data-stu-id="7c087-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c087-170">请求</span><span class="sxs-lookup"><span data-stu-id="7c087-170">Request</span></span>
<span data-ttu-id="7c087-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c087-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c087-172">响应</span><span class="sxs-lookup"><span data-stu-id="7c087-172">Response</span></span>
<span data-ttu-id="7c087-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c087-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






