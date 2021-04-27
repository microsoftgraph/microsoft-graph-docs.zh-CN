---
title: 'user: getMemberObjects'
description: 返回用户所属的所有组、目录角色和管理单元。检查是可传递的。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a681a4edfe244bd835d7fe07d5aac3ceeedff472
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053368"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="fd19c-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fd19c-104">user: getMemberObjects</span></span>

<span data-ttu-id="fd19c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd19c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd19c-p102">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="fd19c-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd19c-108">权限</span><span class="sxs-lookup"><span data-stu-id="fd19c-108">Permissions</span></span>
<span data-ttu-id="fd19c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd19c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fd19c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd19c-111">Permission type</span></span>      | <span data-ttu-id="fd19c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd19c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd19c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd19c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fd19c-114">User.Read、User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd19c-114">User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd19c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd19c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd19c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd19c-116">Not supported.</span></span>    |
|<span data-ttu-id="fd19c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd19c-117">Application</span></span> | <span data-ttu-id="fd19c-118">User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd19c-118">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd19c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd19c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="fd19c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd19c-120">Request headers</span></span>
| <span data-ttu-id="fd19c-121">标头</span><span class="sxs-lookup"><span data-stu-id="fd19c-121">Header</span></span>       | <span data-ttu-id="fd19c-122">值</span><span class="sxs-lookup"><span data-stu-id="fd19c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd19c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd19c-123">Authorization</span></span>  | <span data-ttu-id="fd19c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd19c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd19c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd19c-126">Content-Type</span></span>  | <span data-ttu-id="fd19c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fd19c-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd19c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd19c-128">Request body</span></span>
<span data-ttu-id="fd19c-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fd19c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fd19c-130">参数</span><span class="sxs-lookup"><span data-stu-id="fd19c-130">Parameter</span></span>    | <span data-ttu-id="fd19c-131">类型</span><span class="sxs-lookup"><span data-stu-id="fd19c-131">Type</span></span>   |<span data-ttu-id="fd19c-132">说明</span><span class="sxs-lookup"><span data-stu-id="fd19c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd19c-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fd19c-133">securityEnabledOnly</span></span>|<span data-ttu-id="fd19c-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd19c-134">Boolean</span></span>|<span data-ttu-id="fd19c-p105">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="fd19c-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="fd19c-137">响应</span><span class="sxs-lookup"><span data-stu-id="fd19c-137">Response</span></span>

<span data-ttu-id="fd19c-138">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200 OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="fd19c-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="fd19c-139">示例</span><span class="sxs-lookup"><span data-stu-id="fd19c-139">Example</span></span>
<span data-ttu-id="fd19c-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fd19c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd19c-141">请求</span><span class="sxs-lookup"><span data-stu-id="fd19c-141">Request</span></span>
<span data-ttu-id="fd19c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd19c-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd19c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd19c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="fd19c-144">C#</span><span class="sxs-lookup"><span data-stu-id="fd19c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd19c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd19c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd19c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd19c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd19c-147">Java</span><span class="sxs-lookup"><span data-stu-id="fd19c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fd19c-148">响应</span><span class="sxs-lookup"><span data-stu-id="fd19c-148">Response</span></span>
<span data-ttu-id="fd19c-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fd19c-149">Here is an example of the response.</span></span> <span data-ttu-id="fd19c-150">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fd19c-150">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


