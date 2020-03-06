---
title: 创建 deviceAndAppManagementRoleAssignment
description: 创建新的 deviceAndAppManagementRoleAssignment 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: defac24202a66fff7980d4bb383ecdce38e9d823
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512354"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="484b3-103">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="484b3-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="484b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="484b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="484b3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="484b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="484b3-106">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="484b3-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="484b3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="484b3-107">Prerequisites</span></span>
<span data-ttu-id="484b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="484b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="484b3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="484b3-110">Permission type</span></span>|<span data-ttu-id="484b3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="484b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="484b3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="484b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="484b3-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="484b3-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="484b3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="484b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="484b3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="484b3-115">Not supported.</span></span>|
|<span data-ttu-id="484b3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="484b3-116">Application</span></span>|<span data-ttu-id="484b3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="484b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="484b3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="484b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="484b3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="484b3-119">Request headers</span></span>
|<span data-ttu-id="484b3-120">标头</span><span class="sxs-lookup"><span data-stu-id="484b3-120">Header</span></span>|<span data-ttu-id="484b3-121">值</span><span class="sxs-lookup"><span data-stu-id="484b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="484b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="484b3-122">Authorization</span></span>|<span data-ttu-id="484b3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="484b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="484b3-124">接受</span><span class="sxs-lookup"><span data-stu-id="484b3-124">Accept</span></span>|<span data-ttu-id="484b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="484b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="484b3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="484b3-126">Request body</span></span>
<span data-ttu-id="484b3-127">在请求正文中，提供 deviceAndAppManagementRoleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="484b3-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="484b3-128">下表显示创建 deviceAndAppManagementRoleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="484b3-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="484b3-129">属性</span><span class="sxs-lookup"><span data-stu-id="484b3-129">Property</span></span>|<span data-ttu-id="484b3-130">类型</span><span class="sxs-lookup"><span data-stu-id="484b3-130">Type</span></span>|<span data-ttu-id="484b3-131">说明</span><span class="sxs-lookup"><span data-stu-id="484b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="484b3-132">id</span><span class="sxs-lookup"><span data-stu-id="484b3-132">id</span></span>|<span data-ttu-id="484b3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="484b3-133">String</span></span>|<span data-ttu-id="484b3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="484b3-134">Key of the entity.</span></span> <span data-ttu-id="484b3-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="484b3-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="484b3-136">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="484b3-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="484b3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="484b3-137">displayName</span></span>|<span data-ttu-id="484b3-138">String</span><span class="sxs-lookup"><span data-stu-id="484b3-138">String</span></span>|<span data-ttu-id="484b3-139">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="484b3-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="484b3-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="484b3-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="484b3-141">说明</span><span class="sxs-lookup"><span data-stu-id="484b3-141">description</span></span>|<span data-ttu-id="484b3-142">String</span><span class="sxs-lookup"><span data-stu-id="484b3-142">String</span></span>|<span data-ttu-id="484b3-143">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="484b3-143">Description of the Role Assignment.</span></span> <span data-ttu-id="484b3-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="484b3-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="484b3-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="484b3-145">resourceScopes</span></span>|<span data-ttu-id="484b3-146">String collection</span><span class="sxs-lookup"><span data-stu-id="484b3-146">String collection</span></span>|<span data-ttu-id="484b3-147">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="484b3-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="484b3-148">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="484b3-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="484b3-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="484b3-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="484b3-150">members</span><span class="sxs-lookup"><span data-stu-id="484b3-150">members</span></span>|<span data-ttu-id="484b3-151">String collection</span><span class="sxs-lookup"><span data-stu-id="484b3-151">String collection</span></span>|<span data-ttu-id="484b3-152">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="484b3-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="484b3-153">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="484b3-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="484b3-154">响应</span><span class="sxs-lookup"><span data-stu-id="484b3-154">Response</span></span>
<span data-ttu-id="484b3-155">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="484b3-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="484b3-156">示例</span><span class="sxs-lookup"><span data-stu-id="484b3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="484b3-157">请求</span><span class="sxs-lookup"><span data-stu-id="484b3-157">Request</span></span>
<span data-ttu-id="484b3-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="484b3-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="484b3-159">响应</span><span class="sxs-lookup"><span data-stu-id="484b3-159">Response</span></span>
<span data-ttu-id="484b3-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="484b3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




