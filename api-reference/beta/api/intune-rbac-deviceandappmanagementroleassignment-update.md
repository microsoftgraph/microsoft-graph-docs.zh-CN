---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cbdc5b74b0143189872f9117e619a827741d7eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416494"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="5566a-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5566a-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="5566a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5566a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5566a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5566a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5566a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5566a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5566a-107">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5566a-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5566a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5566a-108">Prerequisites</span></span>
<span data-ttu-id="5566a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5566a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5566a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5566a-111">Permission type</span></span>|<span data-ttu-id="5566a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5566a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5566a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5566a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5566a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5566a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5566a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5566a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5566a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5566a-116">Not supported.</span></span>|
|<span data-ttu-id="5566a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5566a-117">Application</span></span>|<span data-ttu-id="5566a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5566a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5566a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5566a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5566a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5566a-120">Request headers</span></span>
|<span data-ttu-id="5566a-121">标头</span><span class="sxs-lookup"><span data-stu-id="5566a-121">Header</span></span>|<span data-ttu-id="5566a-122">值</span><span class="sxs-lookup"><span data-stu-id="5566a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5566a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5566a-123">Authorization</span></span>|<span data-ttu-id="5566a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5566a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5566a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5566a-125">Accept</span></span>|<span data-ttu-id="5566a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5566a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5566a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5566a-127">Request body</span></span>
<span data-ttu-id="5566a-128">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5566a-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="5566a-129">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5566a-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="5566a-130">属性</span><span class="sxs-lookup"><span data-stu-id="5566a-130">Property</span></span>|<span data-ttu-id="5566a-131">类型</span><span class="sxs-lookup"><span data-stu-id="5566a-131">Type</span></span>|<span data-ttu-id="5566a-132">说明</span><span class="sxs-lookup"><span data-stu-id="5566a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5566a-133">id</span><span class="sxs-lookup"><span data-stu-id="5566a-133">id</span></span>|<span data-ttu-id="5566a-134">String</span><span class="sxs-lookup"><span data-stu-id="5566a-134">String</span></span>|<span data-ttu-id="5566a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5566a-135">Key of the entity.</span></span> <span data-ttu-id="5566a-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="5566a-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="5566a-137">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5566a-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5566a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5566a-138">displayName</span></span>|<span data-ttu-id="5566a-139">String</span><span class="sxs-lookup"><span data-stu-id="5566a-139">String</span></span>|<span data-ttu-id="5566a-140">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="5566a-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="5566a-141">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5566a-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5566a-142">description</span><span class="sxs-lookup"><span data-stu-id="5566a-142">description</span></span>|<span data-ttu-id="5566a-143">String</span><span class="sxs-lookup"><span data-stu-id="5566a-143">String</span></span>|<span data-ttu-id="5566a-144">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="5566a-144">Description of the Role Assignment.</span></span> <span data-ttu-id="5566a-145">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5566a-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5566a-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="5566a-146">scopeMembers</span></span>|<span data-ttu-id="5566a-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="5566a-147">String collection</span></span>|<span data-ttu-id="5566a-148">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5566a-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5566a-149">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="5566a-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5566a-150">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5566a-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5566a-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="5566a-151">scopeType</span></span>|[<span data-ttu-id="5566a-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="5566a-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="5566a-153">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="5566a-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="5566a-154">默认类型 ResourceScope 允许 ResourceScopes 工作的分配。</span><span class="sxs-lookup"><span data-stu-id="5566a-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="5566a-155">AllDevices、 AllLicensedUsers' 和 'AllDevicesAndLicensedUsers'，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="5566a-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="5566a-156">继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5566a-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="5566a-157">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="5566a-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="5566a-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="5566a-158">resourceScopes</span></span>|<span data-ttu-id="5566a-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="5566a-159">String collection</span></span>|<span data-ttu-id="5566a-160">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5566a-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5566a-161">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="5566a-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5566a-162">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5566a-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5566a-163">members</span><span class="sxs-lookup"><span data-stu-id="5566a-163">members</span></span>|<span data-ttu-id="5566a-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="5566a-164">String collection</span></span>|<span data-ttu-id="5566a-165">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5566a-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="5566a-166">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="5566a-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="5566a-167">响应</span><span class="sxs-lookup"><span data-stu-id="5566a-167">Response</span></span>
<span data-ttu-id="5566a-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5566a-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5566a-169">示例</span><span class="sxs-lookup"><span data-stu-id="5566a-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="5566a-170">请求</span><span class="sxs-lookup"><span data-stu-id="5566a-170">Request</span></span>
<span data-ttu-id="5566a-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5566a-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5566a-172">响应</span><span class="sxs-lookup"><span data-stu-id="5566a-172">Response</span></span>
<span data-ttu-id="5566a-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5566a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




