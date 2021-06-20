---
title: 'group: getMemberObjects'
description: 返回此组所属的全部组。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a5f71a53fba79da14674328760081a51fbdcea34
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030787"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="19c48-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="19c48-103">group: getMemberObjects</span></span>

<span data-ttu-id="19c48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19c48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19c48-105">返回此组所属的全部组。</span><span class="sxs-lookup"><span data-stu-id="19c48-105">Return all of the groups that this group is a member of.</span></span> <span data-ttu-id="19c48-106">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="19c48-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="19c48-107">权限</span><span class="sxs-lookup"><span data-stu-id="19c48-107">Permissions</span></span>
<span data-ttu-id="19c48-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19c48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19c48-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19c48-110">Permission type</span></span>      | <span data-ttu-id="19c48-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19c48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19c48-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19c48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19c48-113">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19c48-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="19c48-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19c48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19c48-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19c48-115">Not supported.</span></span>    |
|<span data-ttu-id="19c48-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19c48-116">Application</span></span> | <span data-ttu-id="19c48-117">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c48-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19c48-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19c48-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="19c48-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19c48-119">Request headers</span></span>
| <span data-ttu-id="19c48-120">名称</span><span class="sxs-lookup"><span data-stu-id="19c48-120">Name</span></span>       | <span data-ttu-id="19c48-121">类型</span><span class="sxs-lookup"><span data-stu-id="19c48-121">Type</span></span> | <span data-ttu-id="19c48-122">说明</span><span class="sxs-lookup"><span data-stu-id="19c48-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19c48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19c48-123">Authorization</span></span>  | <span data-ttu-id="19c48-124">string</span><span class="sxs-lookup"><span data-stu-id="19c48-124">string</span></span>  | <span data-ttu-id="19c48-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19c48-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19c48-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19c48-127">Request body</span></span>
<span data-ttu-id="19c48-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19c48-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19c48-129">参数</span><span class="sxs-lookup"><span data-stu-id="19c48-129">Parameter</span></span>    | <span data-ttu-id="19c48-130">类型</span><span class="sxs-lookup"><span data-stu-id="19c48-130">Type</span></span>   |<span data-ttu-id="19c48-131">说明</span><span class="sxs-lookup"><span data-stu-id="19c48-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19c48-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="19c48-132">securityEnabledOnly</span></span>|<span data-ttu-id="19c48-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="19c48-133">Boolean</span></span>| <span data-ttu-id="19c48-p104">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="19c48-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="19c48-136">响应</span><span class="sxs-lookup"><span data-stu-id="19c48-136">Response</span></span>
<span data-ttu-id="19c48-137">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="19c48-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="19c48-138">示例</span><span class="sxs-lookup"><span data-stu-id="19c48-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="19c48-139">请求</span><span class="sxs-lookup"><span data-stu-id="19c48-139">Request</span></span>
<span data-ttu-id="19c48-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19c48-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19c48-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="19c48-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19c48-142">C#</span><span class="sxs-lookup"><span data-stu-id="19c48-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19c48-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19c48-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19c48-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19c48-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19c48-145">Java</span><span class="sxs-lookup"><span data-stu-id="19c48-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19c48-146">响应</span><span class="sxs-lookup"><span data-stu-id="19c48-146">Response</span></span>
<span data-ttu-id="19c48-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19c48-147">The following is an example of the response.</span></span>
><span data-ttu-id="19c48-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="19c48-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

