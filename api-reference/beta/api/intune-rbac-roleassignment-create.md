---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bbd3624649fc576c29afaf07c532fb627d83261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161458"
---
# <a name="create-roleassignment"></a><span data-ttu-id="a5f05-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a5f05-103">Create roleAssignment</span></span>

> <span data-ttu-id="a5f05-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5f05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5f05-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5f05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f05-106">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a5f05-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5f05-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a5f05-107">Prerequisites</span></span>
<span data-ttu-id="a5f05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a5f05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5f05-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5f05-110">Permission type</span></span>|<span data-ttu-id="a5f05-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a5f05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5f05-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5f05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5f05-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f05-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a5f05-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5f05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5f05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5f05-115">Not supported.</span></span>|
|<span data-ttu-id="a5f05-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5f05-116">Application</span></span>|<span data-ttu-id="a5f05-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5f05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5f05-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5f05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a5f05-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5f05-119">Request headers</span></span>
|<span data-ttu-id="a5f05-120">标头</span><span class="sxs-lookup"><span data-stu-id="a5f05-120">Header</span></span>|<span data-ttu-id="a5f05-121">值</span><span class="sxs-lookup"><span data-stu-id="a5f05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5f05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f05-122">Authorization</span></span>|<span data-ttu-id="a5f05-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a5f05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5f05-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5f05-124">Accept</span></span>|<span data-ttu-id="a5f05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5f05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5f05-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5f05-126">Request body</span></span>
<span data-ttu-id="a5f05-127">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5f05-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="a5f05-128">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a5f05-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="a5f05-129">属性</span><span class="sxs-lookup"><span data-stu-id="a5f05-129">Property</span></span>|<span data-ttu-id="a5f05-130">类型</span><span class="sxs-lookup"><span data-stu-id="a5f05-130">Type</span></span>|<span data-ttu-id="a5f05-131">说明</span><span class="sxs-lookup"><span data-stu-id="a5f05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f05-132">id</span><span class="sxs-lookup"><span data-stu-id="a5f05-132">id</span></span>|<span data-ttu-id="a5f05-133">String</span><span class="sxs-lookup"><span data-stu-id="a5f05-133">String</span></span>|<span data-ttu-id="a5f05-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a5f05-134">Key of the entity.</span></span> <span data-ttu-id="a5f05-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a5f05-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a5f05-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a5f05-136">displayName</span></span>|<span data-ttu-id="a5f05-137">String</span><span class="sxs-lookup"><span data-stu-id="a5f05-137">String</span></span>|<span data-ttu-id="a5f05-138">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a5f05-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="a5f05-139">description</span><span class="sxs-lookup"><span data-stu-id="a5f05-139">description</span></span>|<span data-ttu-id="a5f05-140">String</span><span class="sxs-lookup"><span data-stu-id="a5f05-140">String</span></span>|<span data-ttu-id="a5f05-141">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="a5f05-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="a5f05-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="a5f05-142">scopeMembers</span></span>|<span data-ttu-id="a5f05-143">String collection</span><span class="sxs-lookup"><span data-stu-id="a5f05-143">String collection</span></span>|<span data-ttu-id="a5f05-144">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a5f05-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a5f05-145">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a5f05-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="a5f05-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="a5f05-146">scopeType</span></span>|[<span data-ttu-id="a5f05-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="a5f05-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="a5f05-148">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="a5f05-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="a5f05-149">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="a5f05-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="a5f05-150">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="a5f05-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="a5f05-151">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="a5f05-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="a5f05-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a5f05-152">resourceScopes</span></span>|<span data-ttu-id="a5f05-153">String collection</span><span class="sxs-lookup"><span data-stu-id="a5f05-153">String collection</span></span>|<span data-ttu-id="a5f05-154">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a5f05-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a5f05-155">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a5f05-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="a5f05-156">响应</span><span class="sxs-lookup"><span data-stu-id="a5f05-156">Response</span></span>
<span data-ttu-id="a5f05-157">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a5f05-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f05-158">示例</span><span class="sxs-lookup"><span data-stu-id="a5f05-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5f05-159">请求</span><span class="sxs-lookup"><span data-stu-id="a5f05-159">Request</span></span>
<span data-ttu-id="a5f05-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5f05-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5f05-161">响应</span><span class="sxs-lookup"><span data-stu-id="a5f05-161">Response</span></span>
<span data-ttu-id="a5f05-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5f05-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




