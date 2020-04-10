---
title: 创建 unifiedRoleAssignmentMultiple
description: 创建新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61cb184bfb08d90fba6fdcaa879d3b6c38d8e58e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218967"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="91bc6-103">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="91bc6-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="91bc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91bc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91bc6-105">创建新的[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91bc6-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="91bc6-106">使用此对象在 Microsoft Intune 中创建角色分配。</span><span class="sxs-lookup"><span data-stu-id="91bc6-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="91bc6-107">对于其他 Micrsoft 365 应用程序（如 Azure AD），请使用[unifiedRoleAssignment](../resources/unifiedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="91bc6-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91bc6-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="91bc6-108">Permissions</span></span>

<span data-ttu-id="91bc6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91bc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91bc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="91bc6-111">Permission type</span></span> | <span data-ttu-id="91bc6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91bc6-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="91bc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91bc6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="91bc6-114">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="91bc6-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="91bc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91bc6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91bc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91bc6-116">Not supported.</span></span> |
| <span data-ttu-id="91bc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="91bc6-117">Application</span></span> | <span data-ttu-id="91bc6-118">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="91bc6-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="91bc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91bc6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="91bc6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="91bc6-120">Request headers</span></span>

| <span data-ttu-id="91bc6-121">名称</span><span class="sxs-lookup"><span data-stu-id="91bc6-121">Name</span></span> | <span data-ttu-id="91bc6-122">说明</span><span class="sxs-lookup"><span data-stu-id="91bc6-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="91bc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91bc6-123">Authorization</span></span> | <span data-ttu-id="91bc6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91bc6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91bc6-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="91bc6-126">Content-type</span></span> | <span data-ttu-id="91bc6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="91bc6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91bc6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="91bc6-129">Request body</span></span>

<span data-ttu-id="91bc6-130">在请求正文中，提供[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91bc6-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="91bc6-131">请求必须具有在 Azure AD 中定义的作用域（例如`directoryScopeIds`）或特定于应用程序的作用域（例如`appScopeId`）。</span><span class="sxs-lookup"><span data-stu-id="91bc6-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="91bc6-132">Azure AD 作用域的示例包括租户（"/"）、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="91bc6-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="91bc6-133">响应</span><span class="sxs-lookup"><span data-stu-id="91bc6-133">Response</span></span>

<span data-ttu-id="91bc6-134">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91bc6-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91bc6-135">示例</span><span class="sxs-lookup"><span data-stu-id="91bc6-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="91bc6-136">示例1：在 Intune 中在两个作用域组（Azure AD 对象）上创建角色分配</span><span class="sxs-lookup"><span data-stu-id="91bc6-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="91bc6-137">请求</span><span class="sxs-lookup"><span data-stu-id="91bc6-137">Request</span></span>

<span data-ttu-id="91bc6-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91bc6-138">The following is an example of the request.</span></span> <span data-ttu-id="91bc6-139">请注意，使用**roleTemplateId**进行**roleDefinitionId**。</span><span class="sxs-lookup"><span data-stu-id="91bc6-139">Note the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="91bc6-140">**roleDefinitionId**可以是服务范围的模板 ID，也可以是特定于目录的**roleDefinitionId**。</span><span class="sxs-lookup"><span data-stu-id="91bc6-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="91bc6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="91bc6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="91bc6-142">C#</span><span class="sxs-lookup"><span data-stu-id="91bc6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91bc6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91bc6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91bc6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91bc6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="91bc6-145">响应</span><span class="sxs-lookup"><span data-stu-id="91bc6-145">Response</span></span>

<span data-ttu-id="91bc6-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91bc6-146">The following is an example of the response.</span></span>
> <span data-ttu-id="91bc6-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91bc6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="91bc6-149">示例2：在 Intune 中的 "所有设备" 作用域上在 Intune 中创建角色分配</span><span class="sxs-lookup"><span data-stu-id="91bc6-149">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="91bc6-150">使用以下信息创建 Intune 角色分配：</span><span class="sxs-lookup"><span data-stu-id="91bc6-150">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="91bc6-151">若要允许在所有 Intune 设备上进行分配`allDevices` ，请使用**appScopeIds**中的值。</span><span class="sxs-lookup"><span data-stu-id="91bc6-151">To allow assignments over all Intune devices, use the `allDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="91bc6-152">若要允许所有 Intune 许可用户的工作分配， `allLicensedUsers`请使用**appScopeIds**中的值。</span><span class="sxs-lookup"><span data-stu-id="91bc6-152">To allow assignments over all Intune licensed users, use the `allLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="91bc6-153">若要允许在所有 Intune 设备和许可的用户上进行`/`分配，请使用**directoryScopeIds**中的值。</span><span class="sxs-lookup"><span data-stu-id="91bc6-153">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="91bc6-154">请求</span><span class="sxs-lookup"><span data-stu-id="91bc6-154">Request</span></span>

<span data-ttu-id="91bc6-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91bc6-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="91bc6-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="91bc6-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="91bc6-157">C#</span><span class="sxs-lookup"><span data-stu-id="91bc6-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91bc6-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91bc6-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91bc6-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91bc6-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="91bc6-160">响应</span><span class="sxs-lookup"><span data-stu-id="91bc6-160">Response</span></span>

<span data-ttu-id="91bc6-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91bc6-161">The following is an example of the response.</span></span>
> <span data-ttu-id="91bc6-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91bc6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
