---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
ms.openlocfilehash: 887e802371c8545baf44bca81da9b79455eb262d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008715"
---
# <a name="create-roleassignment"></a><span data-ttu-id="df4a8-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="df4a8-103">Create roleAssignment</span></span>

> <span data-ttu-id="df4a8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df4a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df4a8-105">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df4a8-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df4a8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="df4a8-106">Prerequisites</span></span>
<span data-ttu-id="df4a8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="df4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4a8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df4a8-109">Permission type</span></span>|<span data-ttu-id="df4a8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df4a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df4a8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df4a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df4a8-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4a8-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="df4a8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df4a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df4a8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df4a8-114">Not supported.</span></span>|
|<span data-ttu-id="df4a8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df4a8-115">Application</span></span>|<span data-ttu-id="df4a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df4a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df4a8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df4a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="df4a8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="df4a8-118">Request headers</span></span>
|<span data-ttu-id="df4a8-119">标头</span><span class="sxs-lookup"><span data-stu-id="df4a8-119">Header</span></span>|<span data-ttu-id="df4a8-120">值</span><span class="sxs-lookup"><span data-stu-id="df4a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df4a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="df4a8-121">Authorization</span></span>|<span data-ttu-id="df4a8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df4a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df4a8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="df4a8-123">Accept</span></span>|<span data-ttu-id="df4a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="df4a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df4a8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="df4a8-125">Request body</span></span>
<span data-ttu-id="df4a8-126">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df4a8-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="df4a8-127">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df4a8-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="df4a8-128">属性</span><span class="sxs-lookup"><span data-stu-id="df4a8-128">Property</span></span>|<span data-ttu-id="df4a8-129">类型</span><span class="sxs-lookup"><span data-stu-id="df4a8-129">Type</span></span>|<span data-ttu-id="df4a8-130">说明</span><span class="sxs-lookup"><span data-stu-id="df4a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df4a8-131">id</span><span class="sxs-lookup"><span data-stu-id="df4a8-131">id</span></span>|<span data-ttu-id="df4a8-132">String</span><span class="sxs-lookup"><span data-stu-id="df4a8-132">String</span></span>|<span data-ttu-id="df4a8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df4a8-133">Key of the entity.</span></span> <span data-ttu-id="df4a8-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="df4a8-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="df4a8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="df4a8-135">displayName</span></span>|<span data-ttu-id="df4a8-136">String</span><span class="sxs-lookup"><span data-stu-id="df4a8-136">String</span></span>|<span data-ttu-id="df4a8-137">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="df4a8-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="df4a8-138">description</span><span class="sxs-lookup"><span data-stu-id="df4a8-138">description</span></span>|<span data-ttu-id="df4a8-139">String</span><span class="sxs-lookup"><span data-stu-id="df4a8-139">String</span></span>|<span data-ttu-id="df4a8-140">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="df4a8-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="df4a8-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="df4a8-141">resourceScopes</span></span>|<span data-ttu-id="df4a8-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="df4a8-142">String collection</span></span>|<span data-ttu-id="df4a8-143">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="df4a8-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="df4a8-144">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="df4a8-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="df4a8-145">响应</span><span class="sxs-lookup"><span data-stu-id="df4a8-145">Response</span></span>
<span data-ttu-id="df4a8-146">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df4a8-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df4a8-147">示例</span><span class="sxs-lookup"><span data-stu-id="df4a8-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="df4a8-148">请求</span><span class="sxs-lookup"><span data-stu-id="df4a8-148">Request</span></span>
<span data-ttu-id="df4a8-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df4a8-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="df4a8-150">响应</span><span class="sxs-lookup"><span data-stu-id="df4a8-150">Response</span></span>
<span data-ttu-id="df4a8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df4a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



