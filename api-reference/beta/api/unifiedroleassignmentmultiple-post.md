---
title: 创建 unifiedRoleAssignmentMultiple
description: 创建新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cabca41e1935f4a17073e512ea5835d56c982643
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054740"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="244d6-103">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="244d6-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="244d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="244d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="244d6-105">创建新的 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="244d6-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="244d6-106">使用此对象在角色分配Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="244d6-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="244d6-107">For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="244d6-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="244d6-108">权限</span><span class="sxs-lookup"><span data-stu-id="244d6-108">Permissions</span></span>

<span data-ttu-id="244d6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="244d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="244d6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="244d6-111">Permission type</span></span> | <span data-ttu-id="244d6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="244d6-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="244d6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="244d6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="244d6-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="244d6-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="244d6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="244d6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="244d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="244d6-116">Not supported.</span></span> |
| <span data-ttu-id="244d6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="244d6-117">Application</span></span> | <span data-ttu-id="244d6-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="244d6-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="244d6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="244d6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="244d6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="244d6-120">Request headers</span></span>

| <span data-ttu-id="244d6-121">名称</span><span class="sxs-lookup"><span data-stu-id="244d6-121">Name</span></span> | <span data-ttu-id="244d6-122">说明</span><span class="sxs-lookup"><span data-stu-id="244d6-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="244d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="244d6-123">Authorization</span></span> | <span data-ttu-id="244d6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="244d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="244d6-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="244d6-126">Content-type</span></span> | <span data-ttu-id="244d6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="244d6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="244d6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="244d6-129">Request body</span></span>

<span data-ttu-id="244d6-130">在请求正文中，提供 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="244d6-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="244d6-131">请求必须具有在 Azure AD 中定义的作用域（如 ）或特定于应用程序的范围（ `directoryScopeIds` 如 `appScopeId` ）。</span><span class="sxs-lookup"><span data-stu-id="244d6-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="244d6-132">Azure AD 范围的示例包括租户 (/") 、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="244d6-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="244d6-133">响应</span><span class="sxs-lookup"><span data-stu-id="244d6-133">Response</span></span>

<span data-ttu-id="244d6-134">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="244d6-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="244d6-135">示例</span><span class="sxs-lookup"><span data-stu-id="244d6-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="244d6-136">示例 1：在 Intune 角色分配两个作用域组上创建一个 (组，即 Azure AD 对象) </span><span class="sxs-lookup"><span data-stu-id="244d6-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="244d6-137">请求</span><span class="sxs-lookup"><span data-stu-id="244d6-137">Request</span></span>

<span data-ttu-id="244d6-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="244d6-138">The following is an example of the request.</span></span>
> <span data-ttu-id="244d6-139">**注意\*\*\*\*：roleDefinitionId** 的 **roleTemplateId 的使用**。</span><span class="sxs-lookup"><span data-stu-id="244d6-139">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="244d6-140">**roleDefinitionId** 可以是服务范围的模板 ID 或特定于目录 **的 roleDefinitionId**。</span><span class="sxs-lookup"><span data-stu-id="244d6-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="244d6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="244d6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="244d6-142">C#</span><span class="sxs-lookup"><span data-stu-id="244d6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="244d6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="244d6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="244d6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="244d6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="244d6-145">Java</span><span class="sxs-lookup"><span data-stu-id="244d6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="244d6-146">响应</span><span class="sxs-lookup"><span data-stu-id="244d6-146">Response</span></span>

<span data-ttu-id="244d6-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="244d6-147">The following is an example of the response.</span></span>
> <span data-ttu-id="244d6-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="244d6-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="244d6-149">示例 2：在 Intune 角色分配"所有设备"的 Intune 中创建一个应用</span><span class="sxs-lookup"><span data-stu-id="244d6-149">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="244d6-150">使用以下信息创建 Intune 角色分配：</span><span class="sxs-lookup"><span data-stu-id="244d6-150">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="244d6-151">若要允许在所有 Intune 设备上进行分配，请使用 `AllDevices` **appScopeIds 中的值**。</span><span class="sxs-lookup"><span data-stu-id="244d6-151">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="244d6-152">若要允许分配所有 Intune 许可用户，请使用 `AllLicensedUsers` **appScopeIds 中的值**。</span><span class="sxs-lookup"><span data-stu-id="244d6-152">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="244d6-153">若要允许分配所有 Intune 设备和许可用户，请使用 `/` **directoryScopeIds 中的值**。</span><span class="sxs-lookup"><span data-stu-id="244d6-153">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="244d6-154">请求</span><span class="sxs-lookup"><span data-stu-id="244d6-154">Request</span></span>

<span data-ttu-id="244d6-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="244d6-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="244d6-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="244d6-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="244d6-157">C#</span><span class="sxs-lookup"><span data-stu-id="244d6-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="244d6-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="244d6-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="244d6-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="244d6-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="244d6-160">Java</span><span class="sxs-lookup"><span data-stu-id="244d6-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="244d6-161">响应</span><span class="sxs-lookup"><span data-stu-id="244d6-161">Response</span></span>

<span data-ttu-id="244d6-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="244d6-162">The following is an example of the response.</span></span>
> <span data-ttu-id="244d6-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="244d6-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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


