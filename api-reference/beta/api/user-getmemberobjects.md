---
title: 'user: getMemberObjects'
description: 返回用户所属的所有组、目录角色和管理单元。检查是可传递的。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 10047d6836b3bbd8a71c3f60596c52f4e7c40010
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017092"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="6667d-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="6667d-104">user: getMemberObjects</span></span>

<span data-ttu-id="6667d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6667d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6667d-p102">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="6667d-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6667d-108">权限</span><span class="sxs-lookup"><span data-stu-id="6667d-108">Permissions</span></span>
<span data-ttu-id="6667d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6667d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6667d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6667d-111">Permission type</span></span>      | <span data-ttu-id="6667d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6667d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6667d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6667d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6667d-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6667d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6667d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6667d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6667d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6667d-116">Not supported.</span></span>    |
|<span data-ttu-id="6667d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6667d-117">Application</span></span> | <span data-ttu-id="6667d-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6667d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6667d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6667d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="6667d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6667d-120">Request headers</span></span>
| <span data-ttu-id="6667d-121">标头</span><span class="sxs-lookup"><span data-stu-id="6667d-121">Header</span></span>       | <span data-ttu-id="6667d-122">值</span><span class="sxs-lookup"><span data-stu-id="6667d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6667d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6667d-123">Authorization</span></span>  | <span data-ttu-id="6667d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6667d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6667d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6667d-126">Content-Type</span></span>  | <span data-ttu-id="6667d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6667d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6667d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6667d-128">Request body</span></span>
<span data-ttu-id="6667d-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6667d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6667d-130">参数</span><span class="sxs-lookup"><span data-stu-id="6667d-130">Parameter</span></span>    | <span data-ttu-id="6667d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6667d-131">Type</span></span>   |<span data-ttu-id="6667d-132">说明</span><span class="sxs-lookup"><span data-stu-id="6667d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6667d-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6667d-133">securityEnabledOnly</span></span>|<span data-ttu-id="6667d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6667d-134">Boolean</span></span>|<span data-ttu-id="6667d-p105">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6667d-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="6667d-137">响应</span><span class="sxs-lookup"><span data-stu-id="6667d-137">Response</span></span>

<span data-ttu-id="6667d-138">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200 OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="6667d-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="6667d-139">示例</span><span class="sxs-lookup"><span data-stu-id="6667d-139">Example</span></span>
<span data-ttu-id="6667d-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6667d-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6667d-141">请求</span><span class="sxs-lookup"><span data-stu-id="6667d-141">Request</span></span>
<span data-ttu-id="6667d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6667d-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6667d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6667d-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6667d-144">C#</span><span class="sxs-lookup"><span data-stu-id="6667d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6667d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6667d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6667d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6667d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6667d-147">响应</span><span class="sxs-lookup"><span data-stu-id="6667d-147">Response</span></span>
<span data-ttu-id="6667d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6667d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


