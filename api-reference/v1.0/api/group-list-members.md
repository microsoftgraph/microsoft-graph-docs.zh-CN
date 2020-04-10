---
title: 列出成员
description: 获取组的直接成员列表。 组可将用户、组织联系人和其他组作为成员。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fdb70c70f066c459b2188e90fce40ed73adc0050
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181713"
---
# <a name="list-members"></a><span data-ttu-id="3804e-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="3804e-104">List members</span></span>

<span data-ttu-id="3804e-p102">命名空间：microsoft.graph 获取组的直接成员列表。组可将用户、组织联系人和其他组作为成员。此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="3804e-p102">Namespace: microsoft.graph Get a list of the group's direct members. A group can have users, organizational contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3804e-108">权限</span><span class="sxs-lookup"><span data-stu-id="3804e-108">Permissions</span></span>
<span data-ttu-id="3804e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3804e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3804e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3804e-111">Permission type</span></span>      | <span data-ttu-id="3804e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3804e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3804e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3804e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3804e-114">User.ReadBasic.All、User.Read.All、GroupMember.Read.All、Group.Read.All、 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3804e-114">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="3804e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3804e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3804e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3804e-116">Not supported.</span></span>    |
|<span data-ttu-id="3804e-117">Application</span><span class="sxs-lookup"><span data-stu-id="3804e-117">Application</span></span> | <span data-ttu-id="3804e-118">User.Read.All、GroupMember.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3804e-118">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3804e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3804e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3804e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3804e-120">Optional query parameters</span></span>
<span data-ttu-id="3804e-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3804e-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3804e-122">请求头</span><span class="sxs-lookup"><span data-stu-id="3804e-122">Request headers</span></span>
| <span data-ttu-id="3804e-123">标头</span><span class="sxs-lookup"><span data-stu-id="3804e-123">Header</span></span>       | <span data-ttu-id="3804e-124">值</span><span class="sxs-lookup"><span data-stu-id="3804e-124">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3804e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3804e-125">Authorization</span></span>  | <span data-ttu-id="3804e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3804e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3804e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3804e-128">Request body</span></span>
<span data-ttu-id="3804e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3804e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3804e-130">响应</span><span class="sxs-lookup"><span data-stu-id="3804e-130">Response</span></span>
<span data-ttu-id="3804e-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3804e-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3804e-132">示例</span><span class="sxs-lookup"><span data-stu-id="3804e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3804e-133">请求</span><span class="sxs-lookup"><span data-stu-id="3804e-133">Request</span></span>
<span data-ttu-id="3804e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3804e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3804e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3804e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="3804e-136">C#</span><span class="sxs-lookup"><span data-stu-id="3804e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3804e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3804e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3804e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3804e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3804e-139">Java</span><span class="sxs-lookup"><span data-stu-id="3804e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3804e-140">响应</span><span class="sxs-lookup"><span data-stu-id="3804e-140">Response</span></span>
<span data-ttu-id="3804e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3804e-141">The following is an example of the response.</span></span>
><span data-ttu-id="3804e-142">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3804e-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
