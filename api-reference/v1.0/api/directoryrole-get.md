---
title: 获取 directoryRole
description: 检索 directoryRole 对象的属性。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 368503c10b809571dcef4cef5265a86a37044031
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522721"
---
# <a name="get-directoryrole"></a><span data-ttu-id="6a46f-103">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="6a46f-103">Get directoryRole</span></span>

<span data-ttu-id="6a46f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a46f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a46f-105">检索 [directoryRole](../resources/directoryrole.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a46f-105">Retrieve the properties of a [directoryRole](../resources/directoryrole.md) object.</span></span> <span data-ttu-id="6a46f-106">若要成功进行响应，必须在租户中激活角色。</span><span class="sxs-lookup"><span data-stu-id="6a46f-106">The role must be activated in tenant for a successful response.</span></span>

> [!Note]
> <span data-ttu-id="6a46f-107">您可以将 **directoryRole** 的对象 id 和模板 ID 与此 API 一起使用。</span><span class="sxs-lookup"><span data-stu-id="6a46f-107">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="6a46f-108">内置角色的模板 ID 是不可变的，可在 Azure 门户上的角色说明中查看。</span><span class="sxs-lookup"><span data-stu-id="6a46f-108">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="6a46f-109">有关详细信息，请参阅 [角色模板 id](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)。</span><span class="sxs-lookup"><span data-stu-id="6a46f-109">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a46f-110">权限</span><span class="sxs-lookup"><span data-stu-id="6a46f-110">Permissions</span></span>
<span data-ttu-id="6a46f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a46f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a46f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a46f-113">Permission type</span></span>      | <span data-ttu-id="6a46f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a46f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a46f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a46f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6a46f-116">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="6a46f-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a46f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a46f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a46f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a46f-118">Not supported.</span></span>    |
|<span data-ttu-id="6a46f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a46f-119">Application</span></span> | <span data-ttu-id="6a46f-120">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="6a46f-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a46f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a46f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a46f-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6a46f-122">Optional query parameters</span></span>
<span data-ttu-id="6a46f-123">此方法 **不** 支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="6a46f-123">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a46f-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a46f-124">Request headers</span></span>
| <span data-ttu-id="6a46f-125">名称</span><span class="sxs-lookup"><span data-stu-id="6a46f-125">Name</span></span>       | <span data-ttu-id="6a46f-126">类型</span><span class="sxs-lookup"><span data-stu-id="6a46f-126">Type</span></span> | <span data-ttu-id="6a46f-127">说明</span><span class="sxs-lookup"><span data-stu-id="6a46f-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a46f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a46f-128">Authorization</span></span>  | <span data-ttu-id="6a46f-129">string</span><span class="sxs-lookup"><span data-stu-id="6a46f-129">string</span></span>  | <span data-ttu-id="6a46f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a46f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a46f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a46f-132">Request body</span></span>
<span data-ttu-id="6a46f-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a46f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a46f-134">响应</span><span class="sxs-lookup"><span data-stu-id="6a46f-134">Response</span></span>

<span data-ttu-id="6a46f-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a46f-135">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6a46f-136">示例</span><span class="sxs-lookup"><span data-stu-id="6a46f-136">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-objectid"></a><span data-ttu-id="6a46f-137">示例1：使用 objectId 获取目录角色的定义</span><span class="sxs-lookup"><span data-stu-id="6a46f-137">Example 1: Get the definition of a directory role using objectId</span></span>
##### <a name="request"></a><span data-ttu-id="6a46f-138">请求</span><span class="sxs-lookup"><span data-stu-id="6a46f-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a46f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a46f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_objectId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda
```
# <a name="c"></a>[<span data-ttu-id="6a46f-140">C#</span><span class="sxs-lookup"><span data-stu-id="6a46f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a46f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a46f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a46f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a46f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a46f-143">Java</span><span class="sxs-lookup"><span data-stu-id="6a46f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a46f-144">响应</span><span class="sxs-lookup"><span data-stu-id="6a46f-144">Response</span></span>
><span data-ttu-id="6a46f-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a46f-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-directory-role-using-templateid"></a><span data-ttu-id="6a46f-146">示例2：使用 templateId 获取目录角色的定义</span><span class="sxs-lookup"><span data-stu-id="6a46f-146">Example 2: Get the definition of a directory role using templateId</span></span>
##### <a name="request"></a><span data-ttu-id="6a46f-147">请求</span><span class="sxs-lookup"><span data-stu-id="6a46f-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a46f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a46f-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf
```
# <a name="c"></a>[<span data-ttu-id="6a46f-149">C#</span><span class="sxs-lookup"><span data-stu-id="6a46f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a46f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a46f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a46f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a46f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a46f-152">Java</span><span class="sxs-lookup"><span data-stu-id="6a46f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6a46f-153">响应</span><span class="sxs-lookup"><span data-stu-id="6a46f-153">Response</span></span>
><span data-ttu-id="6a46f-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a46f-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
