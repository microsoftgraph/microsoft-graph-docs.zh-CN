---
title: 列出成员
description: 获取组的直接成员列表。 组可将用户、组织联系人、设备、服务主体和其他组作为成员。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6eebc7a1f9a33b1cebf5d935b4ff5af0a4b3a790
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057631"
---
# <a name="list-members"></a><span data-ttu-id="d1260-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="d1260-104">List members</span></span>

<span data-ttu-id="d1260-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1260-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1260-106">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="d1260-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="d1260-107">组可将用户、组织联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="d1260-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="d1260-108">当前，由于在 Graph V1.0 终结点上分阶段部署服务主体，因此未将服务主体列为组成员。</span><span class="sxs-lookup"><span data-stu-id="d1260-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="d1260-109">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="d1260-109">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1260-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1260-110">Permissions</span></span>
<span data-ttu-id="d1260-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1260-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1260-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1260-113">Permission type</span></span>      | <span data-ttu-id="d1260-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1260-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1260-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1260-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d1260-116">User.ReadBasic.All、User.Read.All、GroupMember.Read.All、Group.Read.All、 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1260-116">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="d1260-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1260-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1260-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1260-118">Not supported.</span></span>    |
|<span data-ttu-id="d1260-119">Application</span><span class="sxs-lookup"><span data-stu-id="d1260-119">Application</span></span> | <span data-ttu-id="d1260-120">User.Read.All、GroupMember.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1260-120">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d1260-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1260-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1260-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1260-122">Optional query parameters</span></span>
<span data-ttu-id="d1260-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d1260-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1260-124">请求头</span><span class="sxs-lookup"><span data-stu-id="d1260-124">Request headers</span></span>
| <span data-ttu-id="d1260-125">标头</span><span class="sxs-lookup"><span data-stu-id="d1260-125">Header</span></span>       | <span data-ttu-id="d1260-126">值</span><span class="sxs-lookup"><span data-stu-id="d1260-126">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d1260-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1260-127">Authorization</span></span>  | <span data-ttu-id="d1260-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1260-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1260-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1260-130">Request body</span></span>
<span data-ttu-id="d1260-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1260-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1260-132">响应</span><span class="sxs-lookup"><span data-stu-id="d1260-132">Response</span></span>
<span data-ttu-id="d1260-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d1260-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1260-134">示例</span><span class="sxs-lookup"><span data-stu-id="d1260-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d1260-135">请求</span><span class="sxs-lookup"><span data-stu-id="d1260-135">Request</span></span>
<span data-ttu-id="d1260-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1260-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1260-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1260-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="d1260-138">C#</span><span class="sxs-lookup"><span data-stu-id="d1260-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1260-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1260-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1260-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1260-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1260-141">Java</span><span class="sxs-lookup"><span data-stu-id="d1260-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d1260-142">响应</span><span class="sxs-lookup"><span data-stu-id="d1260-142">Response</span></span>
<span data-ttu-id="d1260-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d1260-143">The following is an example of the response.</span></span>
><span data-ttu-id="d1260-144">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d1260-144">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

