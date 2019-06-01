---
title: 列出域
description: 检索域对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2a7976e476b279bf0c09ceba97aaa797d1490072
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655710"
---
# <a name="list-domains"></a><span data-ttu-id="f4d8f-103">列出域</span><span class="sxs-lookup"><span data-stu-id="f4d8f-103">List domains</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4d8f-104">检索域对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4d8f-105">权限</span><span class="sxs-lookup"><span data-stu-id="f4d8f-105">Permissions</span></span>
<span data-ttu-id="f4d8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4d8f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4d8f-108">Permission type</span></span>      | <span data-ttu-id="f4d8f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4d8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4d8f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4d8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f4d8f-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4d8f-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="f4d8f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4d8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4d8f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-113">Not supported.</span></span>    |
|<span data-ttu-id="f4d8f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4d8f-114">Application</span></span> | <span data-ttu-id="f4d8f-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d8f-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4d8f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4d8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f4d8f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4d8f-117">Optional query parameters</span></span>
<span data-ttu-id="f4d8f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4d8f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4d8f-119">Request headers</span></span>
| <span data-ttu-id="f4d8f-120">名称</span><span class="sxs-lookup"><span data-stu-id="f4d8f-120">Name</span></span>      |<span data-ttu-id="f4d8f-121">说明</span><span class="sxs-lookup"><span data-stu-id="f4d8f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4d8f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4d8f-122">Authorization</span></span>  | <span data-ttu-id="f4d8f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f4d8f-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4d8f-125">Accept</span></span>         | <span data-ttu-id="f4d8f-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="f4d8f-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4d8f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4d8f-127">Request body</span></span>
<span data-ttu-id="f4d8f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4d8f-129">响应</span><span class="sxs-lookup"><span data-stu-id="f4d8f-129">Response</span></span>

<span data-ttu-id="f4d8f-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[domain](../resources/domain.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4d8f-131">示例</span><span class="sxs-lookup"><span data-stu-id="f4d8f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4d8f-132">请求</span><span class="sxs-lookup"><span data-stu-id="f4d8f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
##### <a name="response"></a><span data-ttu-id="f4d8f-133">响应</span><span class="sxs-lookup"><span data-stu-id="f4d8f-133">Response</span></span>
<span data-ttu-id="f4d8f-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4d8f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f4d8f-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f4d8f-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f4d8f-137">C#</span><span class="sxs-lookup"><span data-stu-id="f4d8f-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domains-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4d8f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4d8f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domains-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
