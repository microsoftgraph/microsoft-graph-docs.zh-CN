---
title: 列出 domainNameReferences
description: 使用对域的引用检索 directoryObject 列表。 返回的列表将包含对域具有依赖性的所有目录对象。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 41e205d5e4a58202eca3b47e759f2cf3704ed68e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260492"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="25653-104">列出 domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="25653-104">List domainNameReferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25653-105">使用对域的引用检索[directoryObject](../resources/directoryobject.md)列表。</span><span class="sxs-lookup"><span data-stu-id="25653-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="25653-106">返回的列表将包含对域具有依赖性的所有目录对象。</span><span class="sxs-lookup"><span data-stu-id="25653-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="25653-107">权限</span><span class="sxs-lookup"><span data-stu-id="25653-107">Permissions</span></span>

<span data-ttu-id="25653-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25653-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="25653-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25653-110">Permission type</span></span>      | <span data-ttu-id="25653-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25653-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25653-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25653-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25653-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="25653-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="25653-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25653-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25653-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25653-115">Not supported.</span></span>    |
|<span data-ttu-id="25653-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25653-116">Application</span></span> | <span data-ttu-id="25653-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25653-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25653-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25653-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="25653-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="25653-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="25653-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="25653-120">Optional query parameters</span></span>

<span data-ttu-id="25653-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="25653-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25653-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="25653-122">Request headers</span></span>

| <span data-ttu-id="25653-123">名称</span><span class="sxs-lookup"><span data-stu-id="25653-123">Name</span></span>      |<span data-ttu-id="25653-124">说明</span><span class="sxs-lookup"><span data-stu-id="25653-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25653-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25653-125">Authorization</span></span>  | <span data-ttu-id="25653-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25653-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25653-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="25653-128">Request body</span></span>

<span data-ttu-id="25653-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25653-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25653-130">响应</span><span class="sxs-lookup"><span data-stu-id="25653-130">Response</span></span>

<span data-ttu-id="25653-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="25653-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25653-132">示例</span><span class="sxs-lookup"><span data-stu-id="25653-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25653-133">请求</span><span class="sxs-lookup"><span data-stu-id="25653-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="25653-134">响应</span><span class="sxs-lookup"><span data-stu-id="25653-134">Response</span></span>
<span data-ttu-id="25653-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25653-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="25653-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="25653-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="25653-138">C#</span><span class="sxs-lookup"><span data-stu-id="25653-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25653-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="25653-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="25653-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="25653-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
