---
title: group： checkMemberObjects
description: 检查指定组对象的组或目录角色列表中的成员身份。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 50761be98dba7871258223c16f5944fbbafe053c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680764"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="11e23-103">group： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="11e23-103">group: checkMemberObjects</span></span>

<span data-ttu-id="11e23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11e23-105">检查指定组的组或目录角色列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="11e23-105">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="11e23-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="11e23-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="11e23-107">权限</span><span class="sxs-lookup"><span data-stu-id="11e23-107">Permissions</span></span>

<span data-ttu-id="11e23-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11e23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11e23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11e23-110">Permission type</span></span>                        | <span data-ttu-id="11e23-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11e23-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11e23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11e23-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="11e23-113">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11e23-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="11e23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11e23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11e23-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11e23-115">Not supported.</span></span> |
| <span data-ttu-id="11e23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11e23-116">Application</span></span>                            | <span data-ttu-id="11e23-117">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11e23-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11e23-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11e23-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="11e23-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="11e23-119">Request headers</span></span>

| <span data-ttu-id="11e23-120">名称</span><span class="sxs-lookup"><span data-stu-id="11e23-120">Name</span></span>          | <span data-ttu-id="11e23-121">说明</span><span class="sxs-lookup"><span data-stu-id="11e23-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="11e23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11e23-122">Authorization</span></span> | <span data-ttu-id="11e23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11e23-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11e23-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11e23-125">Content-Type</span></span>  | <span data-ttu-id="11e23-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="11e23-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11e23-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="11e23-128">Request body</span></span>

<span data-ttu-id="11e23-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="11e23-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11e23-130">参数</span><span class="sxs-lookup"><span data-stu-id="11e23-130">Parameter</span></span>    | <span data-ttu-id="11e23-131">类型</span><span class="sxs-lookup"><span data-stu-id="11e23-131">Type</span></span>        | <span data-ttu-id="11e23-132">说明</span><span class="sxs-lookup"><span data-stu-id="11e23-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11e23-133">ids</span><span class="sxs-lookup"><span data-stu-id="11e23-133">ids</span></span>|<span data-ttu-id="11e23-134">String collection</span><span class="sxs-lookup"><span data-stu-id="11e23-134">String collection</span></span>| <span data-ttu-id="11e23-135">包含要检查成员身份的目录角色的组、目录角色或 roleTemplate ID 的对象 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="11e23-135">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="11e23-136">可以指定最多 20 个对象。</span><span class="sxs-lookup"><span data-stu-id="11e23-136">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="11e23-137">响应</span><span class="sxs-lookup"><span data-stu-id="11e23-137">Response</span></span>

<span data-ttu-id="11e23-138">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="11e23-138">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11e23-139">示例</span><span class="sxs-lookup"><span data-stu-id="11e23-139">Examples</span></span>

<span data-ttu-id="11e23-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="11e23-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="11e23-141">请求</span><span class="sxs-lookup"><span data-stu-id="11e23-141">Request</span></span>

<span data-ttu-id="11e23-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11e23-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11e23-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e23-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="11e23-144">C#</span><span class="sxs-lookup"><span data-stu-id="11e23-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e23-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e23-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e23-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e23-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11e23-147">Java</span><span class="sxs-lookup"><span data-stu-id="11e23-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11e23-148">响应</span><span class="sxs-lookup"><span data-stu-id="11e23-148">Response</span></span>

<span data-ttu-id="11e23-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11e23-149">The following is an example of the response.</span></span> 

> <span data-ttu-id="11e23-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="11e23-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

