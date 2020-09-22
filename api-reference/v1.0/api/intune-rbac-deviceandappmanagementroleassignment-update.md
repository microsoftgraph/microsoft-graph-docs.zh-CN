---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4bc446f2a59244fcd6b02f157d25e260480524a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025674"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="51ece-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51ece-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="51ece-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51ece-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51ece-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51ece-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ece-106">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51ece-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51ece-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="51ece-107">Prerequisites</span></span>
<span data-ttu-id="51ece-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51ece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ece-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51ece-110">Permission type</span></span>|<span data-ttu-id="51ece-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51ece-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ece-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51ece-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51ece-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ece-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="51ece-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51ece-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ece-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51ece-115">Not supported.</span></span>|
|<span data-ttu-id="51ece-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="51ece-116">Application</span></span>|<span data-ttu-id="51ece-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51ece-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ece-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51ece-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="51ece-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51ece-119">Request headers</span></span>
|<span data-ttu-id="51ece-120">标头</span><span class="sxs-lookup"><span data-stu-id="51ece-120">Header</span></span>|<span data-ttu-id="51ece-121">值</span><span class="sxs-lookup"><span data-stu-id="51ece-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51ece-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51ece-122">Authorization</span></span>|<span data-ttu-id="51ece-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51ece-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51ece-124">接受</span><span class="sxs-lookup"><span data-stu-id="51ece-124">Accept</span></span>|<span data-ttu-id="51ece-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51ece-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ece-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="51ece-126">Request body</span></span>
<span data-ttu-id="51ece-127">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51ece-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="51ece-128">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51ece-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="51ece-129">属性</span><span class="sxs-lookup"><span data-stu-id="51ece-129">Property</span></span>|<span data-ttu-id="51ece-130">类型</span><span class="sxs-lookup"><span data-stu-id="51ece-130">Type</span></span>|<span data-ttu-id="51ece-131">说明</span><span class="sxs-lookup"><span data-stu-id="51ece-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ece-132">id</span><span class="sxs-lookup"><span data-stu-id="51ece-132">id</span></span>|<span data-ttu-id="51ece-133">String</span><span class="sxs-lookup"><span data-stu-id="51ece-133">String</span></span>|<span data-ttu-id="51ece-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51ece-134">Key of the entity.</span></span> <span data-ttu-id="51ece-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="51ece-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="51ece-136">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51ece-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="51ece-137">displayName</span><span class="sxs-lookup"><span data-stu-id="51ece-137">displayName</span></span>|<span data-ttu-id="51ece-138">String</span><span class="sxs-lookup"><span data-stu-id="51ece-138">String</span></span>|<span data-ttu-id="51ece-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="51ece-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="51ece-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51ece-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="51ece-141">description</span><span class="sxs-lookup"><span data-stu-id="51ece-141">description</span></span>|<span data-ttu-id="51ece-142">String</span><span class="sxs-lookup"><span data-stu-id="51ece-142">String</span></span>|<span data-ttu-id="51ece-143">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="51ece-143">Description of the Role Assignment.</span></span> <span data-ttu-id="51ece-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51ece-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="51ece-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="51ece-145">resourceScopes</span></span>|<span data-ttu-id="51ece-146">String collection</span><span class="sxs-lookup"><span data-stu-id="51ece-146">String collection</span></span>|<span data-ttu-id="51ece-147">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="51ece-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="51ece-148">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="51ece-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="51ece-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51ece-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="51ece-150">members</span><span class="sxs-lookup"><span data-stu-id="51ece-150">members</span></span>|<span data-ttu-id="51ece-151">String collection</span><span class="sxs-lookup"><span data-stu-id="51ece-151">String collection</span></span>|<span data-ttu-id="51ece-152">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="51ece-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="51ece-153">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="51ece-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="51ece-154">响应</span><span class="sxs-lookup"><span data-stu-id="51ece-154">Response</span></span>
<span data-ttu-id="51ece-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51ece-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51ece-156">示例</span><span class="sxs-lookup"><span data-stu-id="51ece-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="51ece-157">请求</span><span class="sxs-lookup"><span data-stu-id="51ece-157">Request</span></span>
<span data-ttu-id="51ece-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51ece-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="51ece-159">响应</span><span class="sxs-lookup"><span data-stu-id="51ece-159">Response</span></span>
<span data-ttu-id="51ece-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51ece-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```









