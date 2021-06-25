---
title: 获取 directoryRole
description: 检索 directoryRole 对象的属性。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e3a64d75b1501f5c88154d483cc10342b6b5c551
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118684"
---
# <a name="get-directoryrole"></a><span data-ttu-id="7ade5-103">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="7ade5-103">Get directoryRole</span></span>

<span data-ttu-id="7ade5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ade5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ade5-105">检索 [directoryRole 对象](../resources/directoryrole.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="7ade5-105">Retrieve the properties of a [directoryRole](../resources/directoryrole.md) object.</span></span> <span data-ttu-id="7ade5-106">角色必须在租户中激活，以成功响应。</span><span class="sxs-lookup"><span data-stu-id="7ade5-106">The role must be activated in tenant for a successful response.</span></span>

<span data-ttu-id="7ade5-107">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="7ade5-107">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="7ade5-108">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="7ade5-108">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="7ade5-109">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="7ade5-109">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ade5-110">权限</span><span class="sxs-lookup"><span data-stu-id="7ade5-110">Permissions</span></span>
<span data-ttu-id="7ade5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ade5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ade5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ade5-113">Permission type</span></span>      | <span data-ttu-id="7ade5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ade5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ade5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ade5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7ade5-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ade5-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ade5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ade5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ade5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ade5-118">Not supported.</span></span>    |
|<span data-ttu-id="7ade5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ade5-119">Application</span></span> | <span data-ttu-id="7ade5-120">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ade5-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ade5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ade5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}
GET /directoryRoles/roleTemplateId={roleTemplateId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ade5-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7ade5-122">Optional query parameters</span></span>
<span data-ttu-id="7ade5-123">例如， **此方法不支持** 任何 [OData](/graph/query-parameters) 查询参数来帮助自定义响应 (，例如，本文不支持 `$filter`) 。</span><span class="sxs-lookup"><span data-stu-id="7ade5-123">This method does **not** support any [OData query parameters](/graph/query-parameters) to help customize the response (for example, `$filter` is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ade5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ade5-124">Request headers</span></span>
| <span data-ttu-id="7ade5-125">名称</span><span class="sxs-lookup"><span data-stu-id="7ade5-125">Name</span></span>       | <span data-ttu-id="7ade5-126">类型</span><span class="sxs-lookup"><span data-stu-id="7ade5-126">Type</span></span> | <span data-ttu-id="7ade5-127">说明</span><span class="sxs-lookup"><span data-stu-id="7ade5-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7ade5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ade5-128">Authorization</span></span>  | <span data-ttu-id="7ade5-129">string</span><span class="sxs-lookup"><span data-stu-id="7ade5-129">string</span></span>  | <span data-ttu-id="7ade5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ade5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ade5-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ade5-132">Request body</span></span>
<span data-ttu-id="7ade5-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ade5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ade5-134">响应</span><span class="sxs-lookup"><span data-stu-id="7ade5-134">Response</span></span>

<span data-ttu-id="7ade5-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ade5-135">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7ade5-136">示例</span><span class="sxs-lookup"><span data-stu-id="7ade5-136">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-role-id"></a><span data-ttu-id="7ade5-137">示例 1：使用角色 ID 获取目录角色的定义</span><span class="sxs-lookup"><span data-stu-id="7ade5-137">Example 1: Get the definition of a directory role using role id</span></span>
#### <a name="request"></a><span data-ttu-id="7ade5-138">请求</span><span class="sxs-lookup"><span data-stu-id="7ade5-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7ade5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ade5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_objectId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda
```
# <a name="c"></a>[<span data-ttu-id="7ade5-140">C#</span><span class="sxs-lookup"><span data-stu-id="7ade5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ade5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ade5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ade5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ade5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ade5-143">Java</span><span class="sxs-lookup"><span data-stu-id="7ade5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7ade5-144">响应</span><span class="sxs-lookup"><span data-stu-id="7ade5-144">Response</span></span>
><span data-ttu-id="7ade5-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7ade5-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
    "id": "23f3b4b4-8a29-4420-8052-e4950273bbda",
    "deletedDateTime": null,
    "description": "Can read sign-in and audit reports.",
    "displayName": "Reports Reader",
    "roleTemplateId": "4a5d8f65-41da-4de4-8968-e035b65339cf"
}
```

### <a name="example-2-get-the-definition-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="7ade5-146">示例 2：使用 roleTemplateId 获取目录角色的定义</span><span class="sxs-lookup"><span data-stu-id="7ade5-146">Example 2: Get the definition of a directory role using roleTemplateId</span></span>
#### <a name="request"></a><span data-ttu-id="7ade5-147">请求</span><span class="sxs-lookup"><span data-stu-id="7ade5-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7ade5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ade5-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf
```
# <a name="c"></a>[<span data-ttu-id="7ade5-149">C#</span><span class="sxs-lookup"><span data-stu-id="7ade5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ade5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ade5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ade5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ade5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ade5-152">Java</span><span class="sxs-lookup"><span data-stu-id="7ade5-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ade5-153">响应</span><span class="sxs-lookup"><span data-stu-id="7ade5-153">Response</span></span>
><span data-ttu-id="7ade5-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7ade5-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
    "id": "23f3b4b4-8a29-4420-8052-e4950273bbda",
    "deletedDateTime": null,
    "description": "Allows ability to read usage reports.",
    "displayName": "Reports Reader",
    "roleTemplateId": "4a5d8f65-41da-4de4-8968-e035b65339cf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
