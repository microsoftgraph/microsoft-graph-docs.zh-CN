---
title: 创建 deviceAndAppManagementRoleAssignment
description: 创建新的 deviceAndAppManagementRoleAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 070db4890528c62443a66cedff3cf06723c5515e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985044"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="83b15-103">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="83b15-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="83b15-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="83b15-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83b15-105">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83b15-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83b15-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="83b15-106">Prerequisites</span></span>
<span data-ttu-id="83b15-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="83b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b15-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83b15-109">Permission type</span></span>|<span data-ttu-id="83b15-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83b15-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83b15-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83b15-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83b15-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b15-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="83b15-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83b15-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83b15-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83b15-114">Not supported.</span></span>|
|<span data-ttu-id="83b15-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83b15-115">Application</span></span>|<span data-ttu-id="83b15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83b15-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83b15-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83b15-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="83b15-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="83b15-118">Request headers</span></span>
|<span data-ttu-id="83b15-119">标头</span><span class="sxs-lookup"><span data-stu-id="83b15-119">Header</span></span>|<span data-ttu-id="83b15-120">值</span><span class="sxs-lookup"><span data-stu-id="83b15-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83b15-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83b15-121">Authorization</span></span>|<span data-ttu-id="83b15-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83b15-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83b15-123">Accept</span><span class="sxs-lookup"><span data-stu-id="83b15-123">Accept</span></span>|<span data-ttu-id="83b15-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83b15-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83b15-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="83b15-125">Request body</span></span>
<span data-ttu-id="83b15-126">在请求正文中，提供 deviceAndAppManagementRoleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83b15-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="83b15-127">下表显示创建 deviceAndAppManagementRoleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83b15-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="83b15-128">属性</span><span class="sxs-lookup"><span data-stu-id="83b15-128">Property</span></span>|<span data-ttu-id="83b15-129">类型</span><span class="sxs-lookup"><span data-stu-id="83b15-129">Type</span></span>|<span data-ttu-id="83b15-130">说明</span><span class="sxs-lookup"><span data-stu-id="83b15-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b15-131">id</span><span class="sxs-lookup"><span data-stu-id="83b15-131">id</span></span>|<span data-ttu-id="83b15-132">String</span><span class="sxs-lookup"><span data-stu-id="83b15-132">String</span></span>|<span data-ttu-id="83b15-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83b15-133">Key of the entity.</span></span> <span data-ttu-id="83b15-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="83b15-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="83b15-135">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="83b15-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="83b15-136">displayName</span><span class="sxs-lookup"><span data-stu-id="83b15-136">displayName</span></span>|<span data-ttu-id="83b15-137">String</span><span class="sxs-lookup"><span data-stu-id="83b15-137">String</span></span>|<span data-ttu-id="83b15-138">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="83b15-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="83b15-139">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="83b15-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="83b15-140">description</span><span class="sxs-lookup"><span data-stu-id="83b15-140">description</span></span>|<span data-ttu-id="83b15-141">String</span><span class="sxs-lookup"><span data-stu-id="83b15-141">String</span></span>|<span data-ttu-id="83b15-142">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="83b15-142">Description of the Role Assignment.</span></span> <span data-ttu-id="83b15-143">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="83b15-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="83b15-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="83b15-144">resourceScopes</span></span>|<span data-ttu-id="83b15-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="83b15-145">String collection</span></span>|<span data-ttu-id="83b15-146">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="83b15-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="83b15-147">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="83b15-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="83b15-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="83b15-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="83b15-149">members</span><span class="sxs-lookup"><span data-stu-id="83b15-149">members</span></span>|<span data-ttu-id="83b15-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="83b15-150">String collection</span></span>|<span data-ttu-id="83b15-151">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="83b15-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="83b15-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="83b15-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="83b15-153">响应</span><span class="sxs-lookup"><span data-stu-id="83b15-153">Response</span></span>
<span data-ttu-id="83b15-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83b15-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b15-155">示例</span><span class="sxs-lookup"><span data-stu-id="83b15-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="83b15-156">请求</span><span class="sxs-lookup"><span data-stu-id="83b15-156">Request</span></span>
<span data-ttu-id="83b15-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83b15-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
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

### <a name="response"></a><span data-ttu-id="83b15-158">响应</span><span class="sxs-lookup"><span data-stu-id="83b15-158">Response</span></span>
<span data-ttu-id="83b15-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83b15-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



