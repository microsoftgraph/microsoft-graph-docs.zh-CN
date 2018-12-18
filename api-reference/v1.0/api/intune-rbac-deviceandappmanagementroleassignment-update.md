---
title: 更新 deviceAndAppManagementRoleAssignment
description: 更新 deviceAndAppManagementRoleAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: d701d859798095442b3ba0e0ee0287e8afced8cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331799"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="9e78b-103">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9e78b-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="9e78b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e78b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e78b-105">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e78b-105">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e78b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e78b-106">Prerequisites</span></span>
<span data-ttu-id="9e78b-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9e78b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e78b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e78b-109">Permission type</span></span>|<span data-ttu-id="9e78b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e78b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e78b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e78b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e78b-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e78b-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9e78b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e78b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e78b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e78b-114">Not supported.</span></span>|
|<span data-ttu-id="9e78b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e78b-115">Application</span></span>|<span data-ttu-id="9e78b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e78b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e78b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e78b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9e78b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e78b-118">Request headers</span></span>
|<span data-ttu-id="9e78b-119">标头</span><span class="sxs-lookup"><span data-stu-id="9e78b-119">Header</span></span>|<span data-ttu-id="9e78b-120">值</span><span class="sxs-lookup"><span data-stu-id="9e78b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e78b-121">授权</span><span class="sxs-lookup"><span data-stu-id="9e78b-121">Authorization</span></span>|<span data-ttu-id="9e78b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e78b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e78b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9e78b-123">Accept</span></span>|<span data-ttu-id="9e78b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e78b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e78b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e78b-125">Request body</span></span>
<span data-ttu-id="9e78b-126">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e78b-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="9e78b-127">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e78b-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="9e78b-128">属性</span><span class="sxs-lookup"><span data-stu-id="9e78b-128">Property</span></span>|<span data-ttu-id="9e78b-129">类型</span><span class="sxs-lookup"><span data-stu-id="9e78b-129">Type</span></span>|<span data-ttu-id="9e78b-130">说明</span><span class="sxs-lookup"><span data-stu-id="9e78b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e78b-131">id</span><span class="sxs-lookup"><span data-stu-id="9e78b-131">id</span></span>|<span data-ttu-id="9e78b-132">String</span><span class="sxs-lookup"><span data-stu-id="9e78b-132">String</span></span>|<span data-ttu-id="9e78b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e78b-133">Key of the entity.</span></span> <span data-ttu-id="9e78b-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="9e78b-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="9e78b-135">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9e78b-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9e78b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9e78b-136">displayName</span></span>|<span data-ttu-id="9e78b-137">String</span><span class="sxs-lookup"><span data-stu-id="9e78b-137">String</span></span>|<span data-ttu-id="9e78b-138">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="9e78b-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="9e78b-139">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9e78b-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9e78b-140">description</span><span class="sxs-lookup"><span data-stu-id="9e78b-140">description</span></span>|<span data-ttu-id="9e78b-141">String</span><span class="sxs-lookup"><span data-stu-id="9e78b-141">String</span></span>|<span data-ttu-id="9e78b-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="9e78b-142">Description of the Role Assignment.</span></span> <span data-ttu-id="9e78b-143">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9e78b-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9e78b-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9e78b-144">resourceScopes</span></span>|<span data-ttu-id="9e78b-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e78b-145">String collection</span></span>|<span data-ttu-id="9e78b-146">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9e78b-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9e78b-147">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e78b-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="9e78b-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9e78b-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9e78b-149">members</span><span class="sxs-lookup"><span data-stu-id="9e78b-149">members</span></span>|<span data-ttu-id="9e78b-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e78b-150">String collection</span></span>|<span data-ttu-id="9e78b-151">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9e78b-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="9e78b-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e78b-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="9e78b-153">响应</span><span class="sxs-lookup"><span data-stu-id="9e78b-153">Response</span></span>
<span data-ttu-id="9e78b-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e78b-154">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e78b-155">示例</span><span class="sxs-lookup"><span data-stu-id="9e78b-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e78b-156">请求</span><span class="sxs-lookup"><span data-stu-id="9e78b-156">Request</span></span>
<span data-ttu-id="9e78b-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e78b-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e78b-158">响应</span><span class="sxs-lookup"><span data-stu-id="9e78b-158">Response</span></span>
<span data-ttu-id="9e78b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e78b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



