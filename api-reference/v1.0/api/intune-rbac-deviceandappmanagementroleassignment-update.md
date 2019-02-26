---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02574f1e6d8bc64dbc5f3415d5c102ed011f1c11
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263348"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="a17be-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a17be-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="a17be-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a17be-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a17be-105">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a17be-105">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a17be-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a17be-106">Prerequisites</span></span>
<span data-ttu-id="a17be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a17be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a17be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a17be-109">Permission type</span></span>|<span data-ttu-id="a17be-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a17be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a17be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a17be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a17be-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a17be-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a17be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a17be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a17be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a17be-114">Not supported.</span></span>|
|<span data-ttu-id="a17be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a17be-115">Application</span></span>|<span data-ttu-id="a17be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a17be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a17be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a17be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a17be-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a17be-118">Request headers</span></span>
|<span data-ttu-id="a17be-119">标头</span><span class="sxs-lookup"><span data-stu-id="a17be-119">Header</span></span>|<span data-ttu-id="a17be-120">值</span><span class="sxs-lookup"><span data-stu-id="a17be-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a17be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a17be-121">Authorization</span></span>|<span data-ttu-id="a17be-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a17be-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a17be-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a17be-123">Accept</span></span>|<span data-ttu-id="a17be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a17be-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a17be-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a17be-125">Request body</span></span>
<span data-ttu-id="a17be-126">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a17be-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="a17be-127">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a17be-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="a17be-128">属性</span><span class="sxs-lookup"><span data-stu-id="a17be-128">Property</span></span>|<span data-ttu-id="a17be-129">类型</span><span class="sxs-lookup"><span data-stu-id="a17be-129">Type</span></span>|<span data-ttu-id="a17be-130">说明</span><span class="sxs-lookup"><span data-stu-id="a17be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a17be-131">id</span><span class="sxs-lookup"><span data-stu-id="a17be-131">id</span></span>|<span data-ttu-id="a17be-132">String</span><span class="sxs-lookup"><span data-stu-id="a17be-132">String</span></span>|<span data-ttu-id="a17be-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a17be-133">Key of the entity.</span></span> <span data-ttu-id="a17be-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a17be-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="a17be-135">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a17be-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a17be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a17be-136">displayName</span></span>|<span data-ttu-id="a17be-137">String</span><span class="sxs-lookup"><span data-stu-id="a17be-137">String</span></span>|<span data-ttu-id="a17be-138">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a17be-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="a17be-139">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a17be-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a17be-140">description</span><span class="sxs-lookup"><span data-stu-id="a17be-140">description</span></span>|<span data-ttu-id="a17be-141">String</span><span class="sxs-lookup"><span data-stu-id="a17be-141">String</span></span>|<span data-ttu-id="a17be-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="a17be-142">Description of the Role Assignment.</span></span> <span data-ttu-id="a17be-143">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a17be-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a17be-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a17be-144">resourceScopes</span></span>|<span data-ttu-id="a17be-145">String collection</span><span class="sxs-lookup"><span data-stu-id="a17be-145">String collection</span></span>|<span data-ttu-id="a17be-146">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a17be-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a17be-147">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a17be-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="a17be-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a17be-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a17be-149">members</span><span class="sxs-lookup"><span data-stu-id="a17be-149">members</span></span>|<span data-ttu-id="a17be-150">String collection</span><span class="sxs-lookup"><span data-stu-id="a17be-150">String collection</span></span>|<span data-ttu-id="a17be-151">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a17be-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="a17be-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a17be-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="a17be-153">响应</span><span class="sxs-lookup"><span data-stu-id="a17be-153">Response</span></span>
<span data-ttu-id="a17be-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a17be-154">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a17be-155">示例</span><span class="sxs-lookup"><span data-stu-id="a17be-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="a17be-156">请求</span><span class="sxs-lookup"><span data-stu-id="a17be-156">Request</span></span>
<span data-ttu-id="a17be-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a17be-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a17be-158">响应</span><span class="sxs-lookup"><span data-stu-id="a17be-158">Response</span></span>
<span data-ttu-id="a17be-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a17be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



