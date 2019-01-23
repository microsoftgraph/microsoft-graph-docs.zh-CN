---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a8c889e401664fb0fea66030ff3bcabd0631503
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399911"
---
# <a name="create-roleassignment"></a><span data-ttu-id="60606-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="60606-103">Create roleAssignment</span></span>

> <span data-ttu-id="60606-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="60606-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60606-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60606-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60606-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60606-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60606-107">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60606-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60606-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60606-108">Prerequisites</span></span>
<span data-ttu-id="60606-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="60606-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="60606-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60606-111">Permission type</span></span>|<span data-ttu-id="60606-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60606-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60606-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60606-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60606-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60606-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="60606-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60606-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60606-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60606-116">Not supported.</span></span>|
|<span data-ttu-id="60606-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60606-117">Application</span></span>|<span data-ttu-id="60606-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60606-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60606-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60606-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="60606-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60606-120">Request headers</span></span>
|<span data-ttu-id="60606-121">标头</span><span class="sxs-lookup"><span data-stu-id="60606-121">Header</span></span>|<span data-ttu-id="60606-122">值</span><span class="sxs-lookup"><span data-stu-id="60606-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60606-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60606-123">Authorization</span></span>|<span data-ttu-id="60606-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60606-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60606-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60606-125">Accept</span></span>|<span data-ttu-id="60606-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60606-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60606-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60606-127">Request body</span></span>
<span data-ttu-id="60606-128">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60606-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="60606-129">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60606-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="60606-130">属性</span><span class="sxs-lookup"><span data-stu-id="60606-130">Property</span></span>|<span data-ttu-id="60606-131">类型</span><span class="sxs-lookup"><span data-stu-id="60606-131">Type</span></span>|<span data-ttu-id="60606-132">说明</span><span class="sxs-lookup"><span data-stu-id="60606-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60606-133">id</span><span class="sxs-lookup"><span data-stu-id="60606-133">id</span></span>|<span data-ttu-id="60606-134">String</span><span class="sxs-lookup"><span data-stu-id="60606-134">String</span></span>|<span data-ttu-id="60606-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60606-135">Key of the entity.</span></span> <span data-ttu-id="60606-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="60606-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="60606-137">displayName</span><span class="sxs-lookup"><span data-stu-id="60606-137">displayName</span></span>|<span data-ttu-id="60606-138">String</span><span class="sxs-lookup"><span data-stu-id="60606-138">String</span></span>|<span data-ttu-id="60606-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="60606-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="60606-140">description</span><span class="sxs-lookup"><span data-stu-id="60606-140">description</span></span>|<span data-ttu-id="60606-141">String</span><span class="sxs-lookup"><span data-stu-id="60606-141">String</span></span>|<span data-ttu-id="60606-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="60606-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="60606-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="60606-143">scopeMembers</span></span>|<span data-ttu-id="60606-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="60606-144">String collection</span></span>|<span data-ttu-id="60606-145">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="60606-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="60606-146">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="60606-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="60606-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="60606-147">scopeType</span></span>|[<span data-ttu-id="60606-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="60606-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="60606-149">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="60606-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="60606-150">默认类型 ResourceScope 允许 ResourceScopes 工作的分配。</span><span class="sxs-lookup"><span data-stu-id="60606-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="60606-151">AllDevices、 AllLicensedUsers' 和 'AllDevicesAndLicensedUsers'，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="60606-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="60606-152">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="60606-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="60606-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="60606-153">resourceScopes</span></span>|<span data-ttu-id="60606-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="60606-154">String collection</span></span>|<span data-ttu-id="60606-155">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="60606-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="60606-156">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="60606-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="60606-157">响应</span><span class="sxs-lookup"><span data-stu-id="60606-157">Response</span></span>
<span data-ttu-id="60606-158">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60606-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60606-159">示例</span><span class="sxs-lookup"><span data-stu-id="60606-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="60606-160">请求</span><span class="sxs-lookup"><span data-stu-id="60606-160">Request</span></span>
<span data-ttu-id="60606-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60606-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60606-162">响应</span><span class="sxs-lookup"><span data-stu-id="60606-162">Response</span></span>
<span data-ttu-id="60606-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60606-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




