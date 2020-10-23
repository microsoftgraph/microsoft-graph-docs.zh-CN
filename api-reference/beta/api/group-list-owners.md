---
title: 列出所有者
description: 检索组的所有者列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2b8d2a8478d3b6b0c5ffbea13b4a59873cdc9f91
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701424"
---
# <a name="list-owners"></a><span data-ttu-id="8fc91-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="8fc91-103">List owners</span></span>

<span data-ttu-id="8fc91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fc91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fc91-105">检索组的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="8fc91-105">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="8fc91-106">所有者是一组允许修改组对象的用户。</span><span class="sxs-lookup"><span data-stu-id="8fc91-106">The owners are a set of users who are allowed to modify the group object.</span></span> <span data-ttu-id="8fc91-107">对于在 Exchange 或从本地环境同步的组中创建的组而言，Microsoft Graph 中目前不提供所有者。</span><span class="sxs-lookup"><span data-stu-id="8fc91-107">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8fc91-108">权限</span><span class="sxs-lookup"><span data-stu-id="8fc91-108">Permissions</span></span>
<span data-ttu-id="8fc91-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fc91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fc91-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fc91-111">Permission type</span></span>      | <span data-ttu-id="8fc91-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8fc91-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fc91-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fc91-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8fc91-114">Group.Read.All 和 User.ReadBasic.All、Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All、Group.Read.All 和 User.Read.All 以及 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fc91-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>  |
|<span data-ttu-id="8fc91-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fc91-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fc91-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fc91-116">Not supported.</span></span>    |
|<span data-ttu-id="8fc91-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fc91-117">Application</span></span> | <span data-ttu-id="8fc91-118">Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All、Group.Read.All 和 User.Read.All 以及 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fc91-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8fc91-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fc91-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fc91-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8fc91-120">Optional query parameters</span></span>
<span data-ttu-id="8fc91-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8fc91-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fc91-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fc91-122">Request headers</span></span>
| <span data-ttu-id="8fc91-123">名称</span><span class="sxs-lookup"><span data-stu-id="8fc91-123">Name</span></span>       | <span data-ttu-id="8fc91-124">类型</span><span class="sxs-lookup"><span data-stu-id="8fc91-124">Type</span></span> | <span data-ttu-id="8fc91-125">说明</span><span class="sxs-lookup"><span data-stu-id="8fc91-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8fc91-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fc91-126">Authorization</span></span>  | <span data-ttu-id="8fc91-127">string</span><span class="sxs-lookup"><span data-stu-id="8fc91-127">string</span></span>  | <span data-ttu-id="8fc91-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8fc91-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fc91-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fc91-130">Request body</span></span>
<span data-ttu-id="8fc91-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8fc91-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fc91-132">响应</span><span class="sxs-lookup"><span data-stu-id="8fc91-132">Response</span></span>
<span data-ttu-id="8fc91-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8fc91-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fc91-134">示例</span><span class="sxs-lookup"><span data-stu-id="8fc91-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8fc91-135">请求</span><span class="sxs-lookup"><span data-stu-id="8fc91-135">Request</span></span>
<span data-ttu-id="8fc91-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8fc91-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8fc91-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fc91-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="8fc91-138">C#</span><span class="sxs-lookup"><span data-stu-id="8fc91-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fc91-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fc91-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fc91-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fc91-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8fc91-141">响应</span><span class="sxs-lookup"><span data-stu-id="8fc91-141">Response</span></span>
<span data-ttu-id="8fc91-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8fc91-142">The following is an example of the response.</span></span>
><span data-ttu-id="8fc91-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8fc91-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


