---
title: 获取 orgContact 的 transitiveReports
description: 获取组织联系人的可传递报告数。
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2ef9be3212ece4478e53dbbedbb0d2531e816dde
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316942"
---
# <a name="get-transitivereports-for-orgcontact"></a><span data-ttu-id="4ac82-103">获取 orgContact 的 transitiveReports</span><span class="sxs-lookup"><span data-stu-id="4ac82-103">Get transitiveReports for orgContact</span></span>

<span data-ttu-id="4ac82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ac82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ac82-105">检索组织联系人的可传递报告计数。</span><span class="sxs-lookup"><span data-stu-id="4ac82-105">Retrieve a count of transitive reports for an organizational contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ac82-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ac82-106">Permissions</span></span>

<span data-ttu-id="4ac82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ac82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="4ac82-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ac82-109">Permission type</span></span> | <span data-ttu-id="4ac82-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ac82-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="4ac82-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ac82-112">OrgContact.Read、OrgContact.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ac82-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="4ac82-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ac82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ac82-114">Not supported.</span></span> |
| <span data-ttu-id="4ac82-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ac82-115">Application</span></span> | <span data-ttu-id="4ac82-116">OrgContact.Read、OrgContact.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ac82-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ac82-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ac82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/transitiveReports/$count
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ac82-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ac82-118">Optional query parameters</span></span>

<span data-ttu-id="4ac82-119">此方法不支持使用查询参数，但需要查询 `$count` 段。</span><span class="sxs-lookup"><span data-stu-id="4ac82-119">This method does not support the use of query parameters, but does require the `$count` query segment.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ac82-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ac82-120">Request headers</span></span>

| <span data-ttu-id="4ac82-121">标头</span><span class="sxs-lookup"><span data-stu-id="4ac82-121">Header</span></span>       | <span data-ttu-id="4ac82-122">值</span><span class="sxs-lookup"><span data-stu-id="4ac82-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ac82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ac82-123">Authorization</span></span>  | <span data-ttu-id="4ac82-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ac82-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ac82-126">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="4ac82-126">ConsistencyLevel</span></span> | <span data-ttu-id="4ac82-127">最终。</span><span class="sxs-lookup"><span data-stu-id="4ac82-127">eventual.</span></span> <span data-ttu-id="4ac82-128">必填。</span><span class="sxs-lookup"><span data-stu-id="4ac82-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ac82-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ac82-129">Request body</span></span>

<span data-ttu-id="4ac82-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ac82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ac82-131">响应</span><span class="sxs-lookup"><span data-stu-id="4ac82-131">Response</span></span>

<span data-ttu-id="4ac82-132">如果成功，此方法在响应正文中返回组织联系人的响应代码和 `200 OK` 可传递报告计数。</span><span class="sxs-lookup"><span data-stu-id="4ac82-132">If successful, this method returns a `200 OK` response code and a count of transitive reports for an organizational contact in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ac82-133">示例</span><span class="sxs-lookup"><span data-stu-id="4ac82-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ac82-134">请求</span><span class="sxs-lookup"><span data-stu-id="4ac82-134">Request</span></span>

<span data-ttu-id="4ac82-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ac82-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4ac82-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ac82-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="4ac82-137">C#</span><span class="sxs-lookup"><span data-stu-id="4ac82-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ac82-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ac82-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ac82-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ac82-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ac82-140">Java</span><span class="sxs-lookup"><span data-stu-id="4ac82-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ac82-141">响应</span><span class="sxs-lookup"><span data-stu-id="4ac82-141">Response</span></span>

<span data-ttu-id="4ac82-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ac82-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="4ac82-143">5 </span><span class="sxs-lookup"><span data-stu-id="4ac82-143">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
