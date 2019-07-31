---
title: 'group: getMemberObjects'
description: 返回组所属的所有组和管理单元。 检查是可传递的。 注意：组不能是目录角色的成员，因此不会返回任何目录角色。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b0379ab01d0c5fc2677801e6fa6eb08c9bf47521
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953876"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="0aac0-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="0aac0-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aac0-106">返回组所属的所有组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="0aac0-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="0aac0-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="0aac0-107">The check is transitive.</span></span> <span data-ttu-id="0aac0-108">注意：组不能是目录角色的成员，因此不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="0aac0-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="0aac0-109">权限</span><span class="sxs-lookup"><span data-stu-id="0aac0-109">Permissions</span></span>
<span data-ttu-id="0aac0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0aac0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aac0-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0aac0-112">Permission type</span></span>      | <span data-ttu-id="0aac0-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0aac0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aac0-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0aac0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0aac0-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0aac0-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0aac0-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0aac0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aac0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0aac0-117">Not supported.</span></span>    |
|<span data-ttu-id="0aac0-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0aac0-118">Application</span></span> | <span data-ttu-id="0aac0-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aac0-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aac0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0aac0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="0aac0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0aac0-121">Request headers</span></span>
| <span data-ttu-id="0aac0-122">名称</span><span class="sxs-lookup"><span data-stu-id="0aac0-122">Name</span></span>       | <span data-ttu-id="0aac0-123">类型</span><span class="sxs-lookup"><span data-stu-id="0aac0-123">Type</span></span> | <span data-ttu-id="0aac0-124">说明</span><span class="sxs-lookup"><span data-stu-id="0aac0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0aac0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aac0-125">Authorization</span></span>  | <span data-ttu-id="0aac0-126">string</span><span class="sxs-lookup"><span data-stu-id="0aac0-126">string</span></span>  | <span data-ttu-id="0aac0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0aac0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aac0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0aac0-129">Request body</span></span>
<span data-ttu-id="0aac0-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0aac0-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0aac0-131">参数</span><span class="sxs-lookup"><span data-stu-id="0aac0-131">Parameter</span></span>    | <span data-ttu-id="0aac0-132">类型</span><span class="sxs-lookup"><span data-stu-id="0aac0-132">Type</span></span>   |<span data-ttu-id="0aac0-133">说明</span><span class="sxs-lookup"><span data-stu-id="0aac0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0aac0-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0aac0-134">securityEnabledOnly</span></span>|<span data-ttu-id="0aac0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="0aac0-135">Boolean</span></span>|<span data-ttu-id="0aac0-p105">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="0aac0-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="0aac0-138">响应</span><span class="sxs-lookup"><span data-stu-id="0aac0-138">Response</span></span>
<span data-ttu-id="0aac0-139">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="0aac0-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="0aac0-140">示例</span><span class="sxs-lookup"><span data-stu-id="0aac0-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0aac0-141">请求</span><span class="sxs-lookup"><span data-stu-id="0aac0-141">Request</span></span>
<span data-ttu-id="0aac0-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0aac0-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0aac0-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0aac0-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0aac0-144">C#</span><span class="sxs-lookup"><span data-stu-id="0aac0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0aac0-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="0aac0-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0aac0-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="0aac0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0aac0-147">Java</span><span class="sxs-lookup"><span data-stu-id="0aac0-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0aac0-148">响应</span><span class="sxs-lookup"><span data-stu-id="0aac0-148">Response</span></span>
<span data-ttu-id="0aac0-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0aac0-149">The following is an example of the response.</span></span>
><span data-ttu-id="0aac0-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0aac0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
