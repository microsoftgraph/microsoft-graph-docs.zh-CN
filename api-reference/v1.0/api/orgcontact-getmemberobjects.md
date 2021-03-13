---
title: orgContact： getMemberObjects
description: 返回此组织联系人是成员的所有组。 检查是可传递的。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a51cd565b363e1fe080f5a1d48de9f51b38d78f7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761637"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="a1e29-104">orgContact： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a1e29-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="a1e29-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1e29-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1e29-106">返回此组织联系人 [是](../resources/orgcontact.md) 成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="a1e29-106">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="a1e29-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a1e29-107">The check is transitive.</span></span> <span data-ttu-id="a1e29-108">组织联系人不能是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="a1e29-108">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="a1e29-109">不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="a1e29-109">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1e29-110">权限</span><span class="sxs-lookup"><span data-stu-id="a1e29-110">Permissions</span></span>
<span data-ttu-id="a1e29-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1e29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e29-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1e29-113">Permission type</span></span>      | <span data-ttu-id="a1e29-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1e29-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1e29-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e29-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a1e29-116">OrgContact.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1e29-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="a1e29-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e29-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1e29-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1e29-118">Not supported.</span></span>    |
|<span data-ttu-id="a1e29-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1e29-119">Application</span></span> | <span data-ttu-id="a1e29-120">OrgContact.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1e29-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1e29-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1e29-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="a1e29-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1e29-122">Request headers</span></span>
| <span data-ttu-id="a1e29-123">标头</span><span class="sxs-lookup"><span data-stu-id="a1e29-123">Header</span></span>       | <span data-ttu-id="a1e29-124">值</span><span class="sxs-lookup"><span data-stu-id="a1e29-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a1e29-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1e29-125">Authorization</span></span>  | <span data-ttu-id="a1e29-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1e29-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1e29-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="a1e29-128">Content-type</span></span>   | <span data-ttu-id="a1e29-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a1e29-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e29-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1e29-131">Request body</span></span>
<span data-ttu-id="a1e29-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a1e29-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a1e29-133">参数</span><span class="sxs-lookup"><span data-stu-id="a1e29-133">Parameter</span></span>    | <span data-ttu-id="a1e29-134">类型</span><span class="sxs-lookup"><span data-stu-id="a1e29-134">Type</span></span>   |<span data-ttu-id="a1e29-135">说明</span><span class="sxs-lookup"><span data-stu-id="a1e29-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1e29-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a1e29-136">securityEnabledOnly</span></span>|<span data-ttu-id="a1e29-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1e29-137">Boolean</span></span>|<span data-ttu-id="a1e29-138">设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="a1e29-138">Set to `false`.</span></span> <span data-ttu-id="a1e29-139">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="a1e29-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="a1e29-140">响应</span><span class="sxs-lookup"><span data-stu-id="a1e29-140">Response</span></span>

<span data-ttu-id="a1e29-141">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="a1e29-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1e29-142">示例</span><span class="sxs-lookup"><span data-stu-id="a1e29-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a1e29-143">请求</span><span class="sxs-lookup"><span data-stu-id="a1e29-143">Request</span></span>
<span data-ttu-id="a1e29-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1e29-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a1e29-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e29-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="a1e29-146">C#</span><span class="sxs-lookup"><span data-stu-id="a1e29-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1e29-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1e29-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1e29-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1e29-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1e29-149">Java</span><span class="sxs-lookup"><span data-stu-id="a1e29-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a1e29-150">响应</span><span class="sxs-lookup"><span data-stu-id="a1e29-150">Response</span></span>
<span data-ttu-id="a1e29-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1e29-151">The following is an example of the response.</span></span>
><span data-ttu-id="a1e29-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a1e29-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

