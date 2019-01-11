---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3f669ac0c3758f2b96e4732fbbdd46966dd87b4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838302"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="6a653-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="6a653-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a653-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a653-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a653-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a653-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a653-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a653-107">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a653-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a653-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a653-108">Prerequisites</span></span>
<span data-ttu-id="6a653-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6a653-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a653-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a653-111">Permission type</span></span>|<span data-ttu-id="6a653-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a653-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a653-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a653-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a653-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a653-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6a653-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a653-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a653-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a653-116">Not supported.</span></span>|
|<span data-ttu-id="6a653-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a653-117">Application</span></span>|<span data-ttu-id="6a653-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a653-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a653-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a653-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6a653-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a653-120">Request headers</span></span>
|<span data-ttu-id="6a653-121">标头</span><span class="sxs-lookup"><span data-stu-id="6a653-121">Header</span></span>|<span data-ttu-id="6a653-122">值</span><span class="sxs-lookup"><span data-stu-id="6a653-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a653-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a653-123">Authorization</span></span>|<span data-ttu-id="6a653-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a653-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a653-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a653-125">Accept</span></span>|<span data-ttu-id="6a653-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a653-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a653-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a653-127">Request body</span></span>
<span data-ttu-id="6a653-128">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a653-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="6a653-129">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a653-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="6a653-130">属性</span><span class="sxs-lookup"><span data-stu-id="6a653-130">Property</span></span>|<span data-ttu-id="6a653-131">类型</span><span class="sxs-lookup"><span data-stu-id="6a653-131">Type</span></span>|<span data-ttu-id="6a653-132">说明</span><span class="sxs-lookup"><span data-stu-id="6a653-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a653-133">id</span><span class="sxs-lookup"><span data-stu-id="6a653-133">id</span></span>|<span data-ttu-id="6a653-134">String</span><span class="sxs-lookup"><span data-stu-id="6a653-134">String</span></span>|<span data-ttu-id="6a653-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6a653-135">Key of the entity.</span></span> <span data-ttu-id="6a653-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="6a653-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="6a653-137">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6a653-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6a653-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6a653-138">displayName</span></span>|<span data-ttu-id="6a653-139">String</span><span class="sxs-lookup"><span data-stu-id="6a653-139">String</span></span>|<span data-ttu-id="6a653-140">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="6a653-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="6a653-141">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6a653-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6a653-142">description</span><span class="sxs-lookup"><span data-stu-id="6a653-142">description</span></span>|<span data-ttu-id="6a653-143">String</span><span class="sxs-lookup"><span data-stu-id="6a653-143">String</span></span>|<span data-ttu-id="6a653-144">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="6a653-144">Description of the Role Assignment.</span></span> <span data-ttu-id="6a653-145">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6a653-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6a653-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="6a653-146">scopeMembers</span></span>|<span data-ttu-id="6a653-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="6a653-147">String collection</span></span>|<span data-ttu-id="6a653-148">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="6a653-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6a653-149">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="6a653-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="6a653-150">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6a653-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6a653-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="6a653-151">scopeType</span></span>|[<span data-ttu-id="6a653-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="6a653-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="6a653-153">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="6a653-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="6a653-154">默认类型 ResourceScope 允许 ResourceScopes 工作的分配。</span><span class="sxs-lookup"><span data-stu-id="6a653-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="6a653-155">AllDevices、 AllLicensedUsers' 和 'AllDevicesAndLicensedUsers'，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="6a653-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="6a653-156">继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="6a653-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="6a653-157">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="6a653-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="6a653-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="6a653-158">resourceScopes</span></span>|<span data-ttu-id="6a653-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="6a653-159">String collection</span></span>|<span data-ttu-id="6a653-160">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="6a653-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6a653-161">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="6a653-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="6a653-162">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6a653-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6a653-163">members</span><span class="sxs-lookup"><span data-stu-id="6a653-163">members</span></span>|<span data-ttu-id="6a653-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="6a653-164">String collection</span></span>|<span data-ttu-id="6a653-165">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="6a653-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="6a653-166">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="6a653-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="6a653-167">响应</span><span class="sxs-lookup"><span data-stu-id="6a653-167">Response</span></span>
<span data-ttu-id="6a653-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a653-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a653-169">示例</span><span class="sxs-lookup"><span data-stu-id="6a653-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a653-170">请求</span><span class="sxs-lookup"><span data-stu-id="6a653-170">Request</span></span>
<span data-ttu-id="6a653-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a653-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 267

{
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

### <a name="response"></a><span data-ttu-id="6a653-172">响应</span><span class="sxs-lookup"><span data-stu-id="6a653-172">Response</span></span>
<span data-ttu-id="6a653-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a653-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





