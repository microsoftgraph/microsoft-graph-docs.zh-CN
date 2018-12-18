---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
author: tfitzmac
ms.openlocfilehash: bf255b0d2c077cbba2e34e81d9730e51c4f5d813
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359743"
---
# <a name="create-roleassignment"></a><span data-ttu-id="fb5c0-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb5c0-103">Create roleAssignment</span></span>

> <span data-ttu-id="fb5c0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb5c0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb5c0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb5c0-107">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb5c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb5c0-108">Prerequisites</span></span>
<span data-ttu-id="fb5c0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fb5c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb5c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb5c0-111">Permission type</span></span>|<span data-ttu-id="fb5c0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb5c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb5c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb5c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb5c0-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb5c0-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fb5c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb5c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb5c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-116">Not supported.</span></span>|
|<span data-ttu-id="fb5c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb5c0-117">Application</span></span>|<span data-ttu-id="fb5c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb5c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb5c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="fb5c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb5c0-120">Request headers</span></span>
|<span data-ttu-id="fb5c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb5c0-121">Header</span></span>|<span data-ttu-id="fb5c0-122">值</span><span class="sxs-lookup"><span data-stu-id="fb5c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb5c0-123">授权</span><span class="sxs-lookup"><span data-stu-id="fb5c0-123">Authorization</span></span>|<span data-ttu-id="fb5c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb5c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb5c0-125">Accept</span></span>|<span data-ttu-id="fb5c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb5c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb5c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb5c0-127">Request body</span></span>
<span data-ttu-id="fb5c0-128">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="fb5c0-129">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="fb5c0-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb5c0-130">Property</span></span>|<span data-ttu-id="fb5c0-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb5c0-131">Type</span></span>|<span data-ttu-id="fb5c0-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb5c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb5c0-133">id</span><span class="sxs-lookup"><span data-stu-id="fb5c0-133">id</span></span>|<span data-ttu-id="fb5c0-134">String</span><span class="sxs-lookup"><span data-stu-id="fb5c0-134">String</span></span>|<span data-ttu-id="fb5c0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-135">Key of the entity.</span></span> <span data-ttu-id="fb5c0-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fb5c0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fb5c0-137">displayName</span></span>|<span data-ttu-id="fb5c0-138">String</span><span class="sxs-lookup"><span data-stu-id="fb5c0-138">String</span></span>|<span data-ttu-id="fb5c0-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="fb5c0-140">description</span><span class="sxs-lookup"><span data-stu-id="fb5c0-140">description</span></span>|<span data-ttu-id="fb5c0-141">String</span><span class="sxs-lookup"><span data-stu-id="fb5c0-141">String</span></span>|<span data-ttu-id="fb5c0-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="fb5c0-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="fb5c0-143">scopeMembers</span></span>|<span data-ttu-id="fb5c0-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="fb5c0-144">String collection</span></span>|<span data-ttu-id="fb5c0-145">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fb5c0-146">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="fb5c0-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="fb5c0-147">scopeType</span></span>|[<span data-ttu-id="fb5c0-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="fb5c0-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="fb5c0-149">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="fb5c0-150">默认类型 ResourceScope 允许 ResourceScopes 工作的分配。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="fb5c0-151">AllDevices、 AllLicensedUsers' 和 'AllDevicesAndLicensedUsers'，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="fb5c0-152">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="fb5c0-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fb5c0-153">resourceScopes</span></span>|<span data-ttu-id="fb5c0-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="fb5c0-154">String collection</span></span>|<span data-ttu-id="fb5c0-155">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fb5c0-156">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="fb5c0-157">响应</span><span class="sxs-lookup"><span data-stu-id="fb5c0-157">Response</span></span>
<span data-ttu-id="fb5c0-158">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb5c0-159">示例</span><span class="sxs-lookup"><span data-stu-id="fb5c0-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb5c0-160">请求</span><span class="sxs-lookup"><span data-stu-id="fb5c0-160">Request</span></span>
<span data-ttu-id="fb5c0-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb5c0-162">响应</span><span class="sxs-lookup"><span data-stu-id="fb5c0-162">Response</span></span>
<span data-ttu-id="fb5c0-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb5c0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





