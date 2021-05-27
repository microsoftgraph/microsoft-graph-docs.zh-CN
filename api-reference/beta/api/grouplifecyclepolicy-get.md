---
title: 获取 groupLifecyclePolicy
description: 检索 groupLifecyclePolicy 对象的属性和关系。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cb3698fef265028afefea0ee4011f96628c6acc3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681142"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="d2ff1-103">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d2ff1-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="d2ff1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2ff1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2ff1-105">检索 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-105">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2ff1-106">权限</span><span class="sxs-lookup"><span data-stu-id="d2ff1-106">Permissions</span></span>

<span data-ttu-id="d2ff1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d2ff1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2ff1-109">Permission type</span></span>      | <span data-ttu-id="d2ff1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2ff1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2ff1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2ff1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2ff1-112">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ff1-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d2ff1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2ff1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2ff1-114">不支持</span><span class="sxs-lookup"><span data-stu-id="d2ff1-114">Not supported</span></span> |
|<span data-ttu-id="d2ff1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2ff1-115">Application</span></span> | <span data-ttu-id="d2ff1-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ff1-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2ff1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2ff1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2ff1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d2ff1-118">Optional query parameters</span></span>
<span data-ttu-id="d2ff1-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2ff1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2ff1-120">Request headers</span></span>
| <span data-ttu-id="d2ff1-121">名称</span><span class="sxs-lookup"><span data-stu-id="d2ff1-121">Name</span></span> | <span data-ttu-id="d2ff1-122">说明</span><span class="sxs-lookup"><span data-stu-id="d2ff1-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d2ff1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2ff1-123">Authorization</span></span> | <span data-ttu-id="d2ff1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2ff1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2ff1-126">Request body</span></span>
<span data-ttu-id="d2ff1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2ff1-128">响应</span><span class="sxs-lookup"><span data-stu-id="d2ff1-128">Response</span></span>
<span data-ttu-id="d2ff1-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-129">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2ff1-130">示例</span><span class="sxs-lookup"><span data-stu-id="d2ff1-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2ff1-131">请求</span><span class="sxs-lookup"><span data-stu-id="d2ff1-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d2ff1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2ff1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="d2ff1-133">C#</span><span class="sxs-lookup"><span data-stu-id="d2ff1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2ff1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2ff1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2ff1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2ff1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2ff1-136">Java</span><span class="sxs-lookup"><span data-stu-id="d2ff1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2ff1-137">响应</span><span class="sxs-lookup"><span data-stu-id="d2ff1-137">Response</span></span>

<span data-ttu-id="d2ff1-138">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d2ff1-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
