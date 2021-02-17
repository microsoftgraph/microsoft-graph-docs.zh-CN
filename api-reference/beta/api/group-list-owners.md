---
title: 列出所有者
description: 检索组的所有者列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 29352a52e6e50c788bd1457f3038c6389356303f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271968"
---
# <a name="list-owners"></a><span data-ttu-id="0893f-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="0893f-103">List owners</span></span>

<span data-ttu-id="0893f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0893f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0893f-105">检索组的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="0893f-105">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="0893f-106">所有者是允许修改组对象的一组用户。</span><span class="sxs-lookup"><span data-stu-id="0893f-106">The owners are a set of users who are allowed to modify the group object.</span></span> <span data-ttu-id="0893f-107">所有者当前在 Microsoft Graph 中对在 Exchange 中创建的组或从本地环境同步的组不可用。</span><span class="sxs-lookup"><span data-stu-id="0893f-107">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0893f-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0893f-108">Permissions</span></span>
<span data-ttu-id="0893f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0893f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0893f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0893f-111">Permission type</span></span>      | <span data-ttu-id="0893f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0893f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0893f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0893f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0893f-114">GroupMember.Read.All、Group.Read.All、GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0893f-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="0893f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0893f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0893f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0893f-116">Not supported.</span></span>    |
|<span data-ttu-id="0893f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0893f-117">Application</span></span> | <span data-ttu-id="0893f-118">GroupMember.Read.All、Group.Read.All、GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0893f-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0893f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0893f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0893f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0893f-120">Optional query parameters</span></span>
<span data-ttu-id="0893f-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0893f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0893f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0893f-122">Request headers</span></span>
| <span data-ttu-id="0893f-123">名称</span><span class="sxs-lookup"><span data-stu-id="0893f-123">Name</span></span>       | <span data-ttu-id="0893f-124">类型</span><span class="sxs-lookup"><span data-stu-id="0893f-124">Type</span></span> | <span data-ttu-id="0893f-125">说明</span><span class="sxs-lookup"><span data-stu-id="0893f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0893f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0893f-126">Authorization</span></span>  | <span data-ttu-id="0893f-127">string</span><span class="sxs-lookup"><span data-stu-id="0893f-127">string</span></span>  | <span data-ttu-id="0893f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0893f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0893f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0893f-130">Request body</span></span>
<span data-ttu-id="0893f-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0893f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0893f-132">响应</span><span class="sxs-lookup"><span data-stu-id="0893f-132">Response</span></span>
<span data-ttu-id="0893f-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0893f-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0893f-134">示例</span><span class="sxs-lookup"><span data-stu-id="0893f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0893f-135">请求</span><span class="sxs-lookup"><span data-stu-id="0893f-135">Request</span></span>
<span data-ttu-id="0893f-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0893f-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0893f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0893f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="0893f-138">C#</span><span class="sxs-lookup"><span data-stu-id="0893f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0893f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0893f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0893f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0893f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0893f-141">Java</span><span class="sxs-lookup"><span data-stu-id="0893f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0893f-142">响应</span><span class="sxs-lookup"><span data-stu-id="0893f-142">Response</span></span>
<span data-ttu-id="0893f-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0893f-143">The following is an example of the response.</span></span>
><span data-ttu-id="0893f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0893f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


