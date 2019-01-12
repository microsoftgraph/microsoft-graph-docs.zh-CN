---
title: 更新 roleAssignment
description: 更新 roleAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f35f7ee957250a546d721a615036f18648d28ff7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913873"
---
# <a name="update-roleassignment"></a><span data-ttu-id="1e72f-103">更新 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="1e72f-103">Update roleAssignment</span></span>

> <span data-ttu-id="1e72f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1e72f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e72f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e72f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e72f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e72f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e72f-107">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e72f-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e72f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e72f-108">Prerequisites</span></span>
<span data-ttu-id="1e72f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1e72f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e72f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e72f-111">Permission type</span></span>|<span data-ttu-id="1e72f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e72f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e72f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e72f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e72f-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e72f-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1e72f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e72f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e72f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e72f-116">Not supported.</span></span>|
|<span data-ttu-id="1e72f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e72f-117">Application</span></span>|<span data-ttu-id="1e72f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e72f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e72f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e72f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1e72f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e72f-120">Request headers</span></span>
|<span data-ttu-id="1e72f-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e72f-121">Header</span></span>|<span data-ttu-id="1e72f-122">值</span><span class="sxs-lookup"><span data-stu-id="1e72f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e72f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e72f-123">Authorization</span></span>|<span data-ttu-id="1e72f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e72f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e72f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e72f-125">Accept</span></span>|<span data-ttu-id="1e72f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e72f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e72f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e72f-127">Request body</span></span>
<span data-ttu-id="1e72f-128">在请求正文中，提供 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e72f-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="1e72f-129">下表显示创建 [roleAssignment](../resources/intune-rbac-roleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e72f-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="1e72f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1e72f-130">Property</span></span>|<span data-ttu-id="1e72f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1e72f-131">Type</span></span>|<span data-ttu-id="1e72f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1e72f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e72f-133">id</span><span class="sxs-lookup"><span data-stu-id="1e72f-133">id</span></span>|<span data-ttu-id="1e72f-134">String</span><span class="sxs-lookup"><span data-stu-id="1e72f-134">String</span></span>|<span data-ttu-id="1e72f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e72f-135">Key of the entity.</span></span> <span data-ttu-id="1e72f-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="1e72f-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="1e72f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1e72f-137">displayName</span></span>|<span data-ttu-id="1e72f-138">String</span><span class="sxs-lookup"><span data-stu-id="1e72f-138">String</span></span>|<span data-ttu-id="1e72f-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="1e72f-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="1e72f-140">description</span><span class="sxs-lookup"><span data-stu-id="1e72f-140">description</span></span>|<span data-ttu-id="1e72f-141">String</span><span class="sxs-lookup"><span data-stu-id="1e72f-141">String</span></span>|<span data-ttu-id="1e72f-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="1e72f-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="1e72f-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="1e72f-143">scopeMembers</span></span>|<span data-ttu-id="1e72f-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="1e72f-144">String collection</span></span>|<span data-ttu-id="1e72f-145">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1e72f-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1e72f-146">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e72f-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="1e72f-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="1e72f-147">scopeType</span></span>|[<span data-ttu-id="1e72f-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="1e72f-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="1e72f-149">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="1e72f-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="1e72f-150">默认类型 ResourceScope 允许 ResourceScopes 工作的分配。</span><span class="sxs-lookup"><span data-stu-id="1e72f-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="1e72f-151">AllDevices、 AllLicensedUsers' 和 'AllDevicesAndLicensedUsers'，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="1e72f-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="1e72f-152">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="1e72f-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="1e72f-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1e72f-153">resourceScopes</span></span>|<span data-ttu-id="1e72f-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="1e72f-154">String collection</span></span>|<span data-ttu-id="1e72f-155">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1e72f-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1e72f-156">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e72f-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="1e72f-157">响应</span><span class="sxs-lookup"><span data-stu-id="1e72f-157">Response</span></span>
<span data-ttu-id="1e72f-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e72f-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e72f-159">示例</span><span class="sxs-lookup"><span data-stu-id="1e72f-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e72f-160">请求</span><span class="sxs-lookup"><span data-stu-id="1e72f-160">Request</span></span>
<span data-ttu-id="1e72f-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e72f-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 224

{
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

### <a name="response"></a><span data-ttu-id="1e72f-162">响应</span><span class="sxs-lookup"><span data-stu-id="1e72f-162">Response</span></span>
<span data-ttu-id="1e72f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e72f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





