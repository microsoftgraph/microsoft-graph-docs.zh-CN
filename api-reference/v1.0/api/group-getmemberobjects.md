---
title: 'group: getMemberObjects'
description: 返回此组所属的全部组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c1da59fa3644b8ca1ab3d06f71cfba3f61f5abcf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094692"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="fef30-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fef30-103">group: getMemberObjects</span></span>

<span data-ttu-id="fef30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fef30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fef30-p101">返回此组所属的全部组。检查是可传递的。注意：组不能是目录角色的成员，因此不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="fef30-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="fef30-108">权限</span><span class="sxs-lookup"><span data-stu-id="fef30-108">Permissions</span></span>
<span data-ttu-id="fef30-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fef30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef30-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fef30-111">Permission type</span></span>      | <span data-ttu-id="fef30-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fef30-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fef30-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fef30-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fef30-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fef30-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fef30-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fef30-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fef30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fef30-116">Not supported.</span></span>    |
|<span data-ttu-id="fef30-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fef30-117">Application</span></span> | <span data-ttu-id="fef30-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef30-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fef30-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fef30-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="fef30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fef30-120">Request headers</span></span>
| <span data-ttu-id="fef30-121">名称</span><span class="sxs-lookup"><span data-stu-id="fef30-121">Name</span></span>       | <span data-ttu-id="fef30-122">类型</span><span class="sxs-lookup"><span data-stu-id="fef30-122">Type</span></span> | <span data-ttu-id="fef30-123">说明</span><span class="sxs-lookup"><span data-stu-id="fef30-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fef30-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fef30-124">Authorization</span></span>  | <span data-ttu-id="fef30-125">string</span><span class="sxs-lookup"><span data-stu-id="fef30-125">string</span></span>  | <span data-ttu-id="fef30-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fef30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fef30-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fef30-128">Request body</span></span>
<span data-ttu-id="fef30-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fef30-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fef30-130">参数</span><span class="sxs-lookup"><span data-stu-id="fef30-130">Parameter</span></span>    | <span data-ttu-id="fef30-131">类型</span><span class="sxs-lookup"><span data-stu-id="fef30-131">Type</span></span>   |<span data-ttu-id="fef30-132">说明</span><span class="sxs-lookup"><span data-stu-id="fef30-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fef30-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fef30-133">securityEnabledOnly</span></span>|<span data-ttu-id="fef30-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef30-134">Boolean</span></span>| <span data-ttu-id="fef30-p104">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="fef30-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="fef30-137">响应</span><span class="sxs-lookup"><span data-stu-id="fef30-137">Response</span></span>
<span data-ttu-id="fef30-138">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="fef30-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="fef30-139">示例</span><span class="sxs-lookup"><span data-stu-id="fef30-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fef30-140">请求</span><span class="sxs-lookup"><span data-stu-id="fef30-140">Request</span></span>
<span data-ttu-id="fef30-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fef30-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fef30-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="fef30-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="fef30-143">C#</span><span class="sxs-lookup"><span data-stu-id="fef30-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fef30-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fef30-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fef30-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fef30-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fef30-146">Java</span><span class="sxs-lookup"><span data-stu-id="fef30-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fef30-147">响应</span><span class="sxs-lookup"><span data-stu-id="fef30-147">Response</span></span>
<span data-ttu-id="fef30-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fef30-148">The following is an example of the response.</span></span>
><span data-ttu-id="fef30-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fef30-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fef30-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fef30-150">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

