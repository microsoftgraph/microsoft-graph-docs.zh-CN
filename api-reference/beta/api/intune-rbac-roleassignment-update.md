---
title: 更新 roleAssignment
description: 更新 roleAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dbb23619e6f44c9630d13808bb9263f21420d5b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414863"
---
# <a name="update-roleassignment"></a><span data-ttu-id="b5366-103">更新 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b5366-103">Update roleAssignment</span></span>

> <span data-ttu-id="b5366-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b5366-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5366-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5366-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5366-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5366-107">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5366-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5366-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5366-108">Prerequisites</span></span>
<span data-ttu-id="b5366-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b5366-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b5366-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5366-111">Permission type</span></span>|<span data-ttu-id="b5366-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5366-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5366-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5366-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5366-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5366-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b5366-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5366-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5366-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5366-116">Not supported.</span></span>|
|<span data-ttu-id="b5366-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5366-117">Application</span></span>|<span data-ttu-id="b5366-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5366-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5366-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5366-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b5366-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5366-120">Request headers</span></span>
|<span data-ttu-id="b5366-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5366-121">Header</span></span>|<span data-ttu-id="b5366-122">值</span><span class="sxs-lookup"><span data-stu-id="b5366-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5366-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5366-123">Authorization</span></span>|<span data-ttu-id="b5366-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5366-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5366-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b5366-125">Accept</span></span>|<span data-ttu-id="b5366-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5366-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5366-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5366-127">Request body</span></span>
<span data-ttu-id="b5366-128">在请求正文中，提供 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5366-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="b5366-129">下表显示创建 [roleAssignment](../resources/intune-rbac-roleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5366-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="b5366-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5366-130">Property</span></span>|<span data-ttu-id="b5366-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5366-131">Type</span></span>|<span data-ttu-id="b5366-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5366-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5366-133">id</span><span class="sxs-lookup"><span data-stu-id="b5366-133">id</span></span>|<span data-ttu-id="b5366-134">String</span><span class="sxs-lookup"><span data-stu-id="b5366-134">String</span></span>|<span data-ttu-id="b5366-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5366-135">Key of the entity.</span></span> <span data-ttu-id="b5366-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="b5366-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b5366-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b5366-137">displayName</span></span>|<span data-ttu-id="b5366-138">String</span><span class="sxs-lookup"><span data-stu-id="b5366-138">String</span></span>|<span data-ttu-id="b5366-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="b5366-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b5366-140">description</span><span class="sxs-lookup"><span data-stu-id="b5366-140">description</span></span>|<span data-ttu-id="b5366-141">String</span><span class="sxs-lookup"><span data-stu-id="b5366-141">String</span></span>|<span data-ttu-id="b5366-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="b5366-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b5366-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="b5366-143">scopeMembers</span></span>|<span data-ttu-id="b5366-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="b5366-144">String collection</span></span>|<span data-ttu-id="b5366-145">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b5366-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b5366-146">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="b5366-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="b5366-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="b5366-147">scopeType</span></span>|[<span data-ttu-id="b5366-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="b5366-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="b5366-149">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="b5366-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="b5366-150">默认类型 ResourceScope 允许 ResourceScopes 工作的分配。</span><span class="sxs-lookup"><span data-stu-id="b5366-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="b5366-151">AllDevices、 AllLicensedUsers' 和 'AllDevicesAndLicensedUsers'，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="b5366-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="b5366-152">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="b5366-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="b5366-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b5366-153">resourceScopes</span></span>|<span data-ttu-id="b5366-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="b5366-154">String collection</span></span>|<span data-ttu-id="b5366-155">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b5366-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b5366-156">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="b5366-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b5366-157">响应</span><span class="sxs-lookup"><span data-stu-id="b5366-157">Response</span></span>
<span data-ttu-id="b5366-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5366-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5366-159">示例</span><span class="sxs-lookup"><span data-stu-id="b5366-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5366-160">请求</span><span class="sxs-lookup"><span data-stu-id="b5366-160">Request</span></span>
<span data-ttu-id="b5366-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5366-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="b5366-162">响应</span><span class="sxs-lookup"><span data-stu-id="b5366-162">Response</span></span>
<span data-ttu-id="b5366-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5366-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




