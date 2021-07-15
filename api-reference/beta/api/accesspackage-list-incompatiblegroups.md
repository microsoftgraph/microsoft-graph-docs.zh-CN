---
title: 列出 incompatibleGroups
description: 检索其访问权限与特定访问包不兼容的组列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c5af81b8995b0fc0662a35157ab4579631b5f189
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439910"
---
# <a name="list-incompatiblegroups"></a><span data-ttu-id="ec214-103">列出 incompatibleGroups</span><span class="sxs-lookup"><span data-stu-id="ec214-103">List incompatibleGroups</span></span>

<span data-ttu-id="ec214-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec214-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec214-105">检索在 accessPackage [上标记为](../resources/group.md) 不兼容的 [组对象的列表](../resources/accesspackage.md)。</span><span class="sxs-lookup"><span data-stu-id="ec214-105">Retrieve a list of the [group](../resources/group.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="ec214-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec214-106">Permissions</span></span>

<span data-ttu-id="ec214-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec214-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec214-109">Permission type</span></span>                        | <span data-ttu-id="ec214-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec214-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec214-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec214-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec214-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec214-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ec214-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec214-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec214-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec214-114">Not supported.</span></span> |
| <span data-ttu-id="ec214-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec214-115">Application</span></span>                            | <span data-ttu-id="ec214-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec214-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec214-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec214-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec214-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec214-118">Optional query parameters</span></span>

<span data-ttu-id="ec214-119">此方法支持通过大型响应对服务器端分页使用 OData 查询参数。</span><span class="sxs-lookup"><span data-stu-id="ec214-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="ec214-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ec214-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec214-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec214-121">Request headers</span></span>

| <span data-ttu-id="ec214-122">名称</span><span class="sxs-lookup"><span data-stu-id="ec214-122">Name</span></span>      |<span data-ttu-id="ec214-123">说明</span><span class="sxs-lookup"><span data-stu-id="ec214-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec214-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec214-124">Authorization</span></span> | <span data-ttu-id="ec214-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec214-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec214-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec214-127">Request body</span></span>

<span data-ttu-id="ec214-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec214-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec214-129">响应</span><span class="sxs-lookup"><span data-stu-id="ec214-129">Response</span></span>

<span data-ttu-id="ec214-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec214-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec214-131">示例</span><span class="sxs-lookup"><span data-stu-id="ec214-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec214-132">请求</span><span class="sxs-lookup"><span data-stu-id="ec214-132">Request</span></span>

<span data-ttu-id="ec214-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ec214-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ec214-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec214-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_incompatiblegroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups
```
# <a name="c"></a>[<span data-ttu-id="ec214-135">C#</span><span class="sxs-lookup"><span data-stu-id="ec214-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-incompatiblegroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec214-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec214-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-incompatiblegroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec214-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec214-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-incompatiblegroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec214-138">Java</span><span class="sxs-lookup"><span data-stu-id="ec214-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-incompatiblegroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec214-139">响应</span><span class="sxs-lookup"><span data-stu-id="ec214-139">Response</span></span>

<span data-ttu-id="ec214-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ec214-140">The following is an example of the response.</span></span>

> <span data-ttu-id="ec214-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ec214-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "a743348f-5667-41a4-89a3-5ad8a94da5d2",
      "displayName": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List incompatibleGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

