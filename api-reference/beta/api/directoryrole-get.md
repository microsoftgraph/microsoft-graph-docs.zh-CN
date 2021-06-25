---
title: 获取 directoryRole
description: 检索 directoryRole 对象的属性。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 905afd750bce1976a25cd5e759df4659cbcb5fe0
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118530"
---
# <a name="get-directoryrole"></a><span data-ttu-id="d65d1-103">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="d65d1-103">Get directoryRole</span></span>

<span data-ttu-id="d65d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d65d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d65d1-105">检索 directoryRole 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d65d1-105">Retrieve the properties of a directoryRole object.</span></span>

<span data-ttu-id="d65d1-106">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="d65d1-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="d65d1-107">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="d65d1-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="d65d1-108">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="d65d1-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="d65d1-109">权限</span><span class="sxs-lookup"><span data-stu-id="d65d1-109">Permissions</span></span>
<span data-ttu-id="d65d1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d65d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d65d1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d65d1-112">Permission type</span></span>      | <span data-ttu-id="d65d1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d65d1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d65d1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d65d1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d65d1-115">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d65d1-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d65d1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d65d1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d65d1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d65d1-117">Not supported.</span></span>    |
|<span data-ttu-id="d65d1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d65d1-118">Application</span></span> | <span data-ttu-id="d65d1-119">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d65d1-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d65d1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d65d1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}
GET /directoryRoles/roleTemplateId={roleTemplateId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d65d1-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d65d1-121">Optional query parameters</span></span>
<span data-ttu-id="d65d1-122">例如， **此方法不支持** 任何 [OData](/graph/query-parameters) 查询参数来帮助自定义响应 (，例如，本文不支持 `$filter`) 。</span><span class="sxs-lookup"><span data-stu-id="d65d1-122">This method does **not** support any [OData query parameters](/graph/query-parameters) to help customize the response (for example, `$filter` is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d65d1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d65d1-123">Request headers</span></span>
| <span data-ttu-id="d65d1-124">名称</span><span class="sxs-lookup"><span data-stu-id="d65d1-124">Name</span></span>       | <span data-ttu-id="d65d1-125">类型</span><span class="sxs-lookup"><span data-stu-id="d65d1-125">Type</span></span> | <span data-ttu-id="d65d1-126">说明</span><span class="sxs-lookup"><span data-stu-id="d65d1-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d65d1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d65d1-127">Authorization</span></span>  | <span data-ttu-id="d65d1-128">string</span><span class="sxs-lookup"><span data-stu-id="d65d1-128">string</span></span>  | <span data-ttu-id="d65d1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d65d1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d65d1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d65d1-131">Request body</span></span>
<span data-ttu-id="d65d1-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d65d1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d65d1-133">响应</span><span class="sxs-lookup"><span data-stu-id="d65d1-133">Response</span></span>

<span data-ttu-id="d65d1-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d65d1-134">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="d65d1-135">示例</span><span class="sxs-lookup"><span data-stu-id="d65d1-135">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-role-id"></a><span data-ttu-id="d65d1-136">示例 1：使用角色 ID 获取目录角色的定义</span><span class="sxs-lookup"><span data-stu-id="d65d1-136">Example 1: Get the definition of a directory role using role id</span></span>
#### <a name="request"></a><span data-ttu-id="d65d1-137">请求</span><span class="sxs-lookup"><span data-stu-id="d65d1-137">Request</span></span>
<span data-ttu-id="d65d1-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d65d1-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d65d1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d65d1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830
```
# <a name="c"></a>[<span data-ttu-id="d65d1-140">C#</span><span class="sxs-lookup"><span data-stu-id="d65d1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d65d1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d65d1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d65d1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d65d1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d65d1-143">Java</span><span class="sxs-lookup"><span data-stu-id="d65d1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d65d1-144">响应</span><span class="sxs-lookup"><span data-stu-id="d65d1-144">Response</span></span>
><span data-ttu-id="d65d1-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d65d1-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```


### <a name="example-2-get-the-definition-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="d65d1-146">示例 2：使用 roleTemplateId 获取目录角色的定义</span><span class="sxs-lookup"><span data-stu-id="d65d1-146">Example 2: Get the definition of a directory role using roleTemplateId</span></span>
#### <a name="request"></a><span data-ttu-id="d65d1-147">请求</span><span class="sxs-lookup"><span data-stu-id="d65d1-147">Request</span></span>
<span data-ttu-id="d65d1-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d65d1-148">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="d65d1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d65d1-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b
```
# <a name="c"></a>[<span data-ttu-id="d65d1-150">C#</span><span class="sxs-lookup"><span data-stu-id="d65d1-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d65d1-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d65d1-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d65d1-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d65d1-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d65d1-153">Java</span><span class="sxs-lookup"><span data-stu-id="d65d1-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d65d1-154">响应</span><span class="sxs-lookup"><span data-stu-id="d65d1-154">Response</span></span>
><span data-ttu-id="d65d1-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d65d1-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
