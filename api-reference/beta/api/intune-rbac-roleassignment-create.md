---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f38b990b37191cec8f0dc1a74ecbd757d4b2b8ee
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189464"
---
# <a name="create-roleassignment"></a><span data-ttu-id="cf581-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf581-103">Create roleAssignment</span></span>

> <span data-ttu-id="cf581-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf581-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf581-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf581-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf581-106">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf581-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf581-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf581-107">Prerequisites</span></span>
<span data-ttu-id="cf581-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf581-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf581-110">Permission type</span></span>|<span data-ttu-id="cf581-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf581-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf581-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf581-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf581-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf581-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cf581-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf581-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf581-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf581-115">Not supported.</span></span>|
|<span data-ttu-id="cf581-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf581-116">Application</span></span>|<span data-ttu-id="cf581-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf581-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf581-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf581-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="cf581-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf581-119">Request headers</span></span>
|<span data-ttu-id="cf581-120">标头</span><span class="sxs-lookup"><span data-stu-id="cf581-120">Header</span></span>|<span data-ttu-id="cf581-121">值</span><span class="sxs-lookup"><span data-stu-id="cf581-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf581-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf581-122">Authorization</span></span>|<span data-ttu-id="cf581-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf581-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf581-124">接受</span><span class="sxs-lookup"><span data-stu-id="cf581-124">Accept</span></span>|<span data-ttu-id="cf581-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf581-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf581-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf581-126">Request body</span></span>
<span data-ttu-id="cf581-127">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf581-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="cf581-128">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cf581-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="cf581-129">属性</span><span class="sxs-lookup"><span data-stu-id="cf581-129">Property</span></span>|<span data-ttu-id="cf581-130">类型</span><span class="sxs-lookup"><span data-stu-id="cf581-130">Type</span></span>|<span data-ttu-id="cf581-131">说明</span><span class="sxs-lookup"><span data-stu-id="cf581-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf581-132">id</span><span class="sxs-lookup"><span data-stu-id="cf581-132">id</span></span>|<span data-ttu-id="cf581-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cf581-133">String</span></span>|<span data-ttu-id="cf581-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cf581-134">Key of the entity.</span></span> <span data-ttu-id="cf581-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="cf581-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cf581-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cf581-136">displayName</span></span>|<span data-ttu-id="cf581-137">String</span><span class="sxs-lookup"><span data-stu-id="cf581-137">String</span></span>|<span data-ttu-id="cf581-138">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="cf581-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="cf581-139">说明</span><span class="sxs-lookup"><span data-stu-id="cf581-139">description</span></span>|<span data-ttu-id="cf581-140">String</span><span class="sxs-lookup"><span data-stu-id="cf581-140">String</span></span>|<span data-ttu-id="cf581-141">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="cf581-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="cf581-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="cf581-142">scopeMembers</span></span>|<span data-ttu-id="cf581-143">String collection</span><span class="sxs-lookup"><span data-stu-id="cf581-143">String collection</span></span>|<span data-ttu-id="cf581-144">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="cf581-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="cf581-145">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="cf581-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="cf581-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="cf581-146">scopeType</span></span>|[<span data-ttu-id="cf581-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="cf581-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="cf581-148">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="cf581-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="cf581-149">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="cf581-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="cf581-150">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers"，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="cf581-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="cf581-151">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="cf581-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="cf581-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="cf581-152">resourceScopes</span></span>|<span data-ttu-id="cf581-153">String collection</span><span class="sxs-lookup"><span data-stu-id="cf581-153">String collection</span></span>|<span data-ttu-id="cf581-154">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="cf581-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="cf581-155">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="cf581-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="cf581-156">响应</span><span class="sxs-lookup"><span data-stu-id="cf581-156">Response</span></span>
<span data-ttu-id="cf581-157">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf581-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf581-158">示例</span><span class="sxs-lookup"><span data-stu-id="cf581-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf581-159">请求</span><span class="sxs-lookup"><span data-stu-id="cf581-159">Request</span></span>
<span data-ttu-id="cf581-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf581-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cf581-161">响应</span><span class="sxs-lookup"><span data-stu-id="cf581-161">Response</span></span>
<span data-ttu-id="cf581-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf581-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```




