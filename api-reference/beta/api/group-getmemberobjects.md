---
title: 'group: getMemberObjects'
description: 返回组的成员的所有组和管理单元。 检查是可传递的。 注意：组不能是目录角色的成员，因此不会返回任何目录角色。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 78d240211f38f25a1e59c76634c4dde3b147393b
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869748"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="a2f34-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a2f34-105">group: getMemberObjects</span></span>

<span data-ttu-id="a2f34-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2f34-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f34-107">返回组的成员的所有组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="a2f34-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="a2f34-108">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a2f34-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2f34-109">权限</span><span class="sxs-lookup"><span data-stu-id="a2f34-109">Permissions</span></span>
<span data-ttu-id="a2f34-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2f34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2f34-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2f34-112">Permission type</span></span>      | <span data-ttu-id="a2f34-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2f34-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2f34-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2f34-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a2f34-115">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2f34-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2f34-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2f34-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f34-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2f34-117">Not supported.</span></span>    |
|<span data-ttu-id="a2f34-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2f34-118">Application</span></span> | <span data-ttu-id="a2f34-119">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f34-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2f34-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2f34-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="a2f34-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2f34-121">Request headers</span></span>
| <span data-ttu-id="a2f34-122">名称</span><span class="sxs-lookup"><span data-stu-id="a2f34-122">Name</span></span>       | <span data-ttu-id="a2f34-123">类型</span><span class="sxs-lookup"><span data-stu-id="a2f34-123">Type</span></span> | <span data-ttu-id="a2f34-124">说明</span><span class="sxs-lookup"><span data-stu-id="a2f34-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2f34-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2f34-125">Authorization</span></span>  | <span data-ttu-id="a2f34-126">string</span><span class="sxs-lookup"><span data-stu-id="a2f34-126">string</span></span>  | <span data-ttu-id="a2f34-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2f34-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2f34-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2f34-129">Request body</span></span>
<span data-ttu-id="a2f34-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a2f34-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a2f34-131">参数</span><span class="sxs-lookup"><span data-stu-id="a2f34-131">Parameter</span></span>    | <span data-ttu-id="a2f34-132">类型</span><span class="sxs-lookup"><span data-stu-id="a2f34-132">Type</span></span>   |<span data-ttu-id="a2f34-133">说明</span><span class="sxs-lookup"><span data-stu-id="a2f34-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2f34-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a2f34-134">securityEnabledOnly</span></span>|<span data-ttu-id="a2f34-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f34-135">Boolean</span></span>|<span data-ttu-id="a2f34-p105">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="a2f34-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="a2f34-138">响应</span><span class="sxs-lookup"><span data-stu-id="a2f34-138">Response</span></span>
<span data-ttu-id="a2f34-139">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="a2f34-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a2f34-140">示例</span><span class="sxs-lookup"><span data-stu-id="a2f34-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a2f34-141">请求</span><span class="sxs-lookup"><span data-stu-id="a2f34-141">Request</span></span>
<span data-ttu-id="a2f34-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2f34-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2f34-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2f34-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="a2f34-144">C#</span><span class="sxs-lookup"><span data-stu-id="a2f34-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2f34-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2f34-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2f34-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2f34-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2f34-147">Java</span><span class="sxs-lookup"><span data-stu-id="a2f34-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a2f34-148">响应</span><span class="sxs-lookup"><span data-stu-id="a2f34-148">Response</span></span>
<span data-ttu-id="a2f34-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2f34-149">The following is an example of the response.</span></span>
><span data-ttu-id="a2f34-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a2f34-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


