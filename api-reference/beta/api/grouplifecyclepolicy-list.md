---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d4e4b693144b0714822a877952e16e1f5696f866
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681135"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="0ed9e-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0ed9e-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="0ed9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ed9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed9e-105">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ed9e-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ed9e-106">Permissions</span></span>

<span data-ttu-id="0ed9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0ed9e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ed9e-109">Permission type</span></span>      | <span data-ttu-id="0ed9e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ed9e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ed9e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ed9e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ed9e-112">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed9e-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0ed9e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ed9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ed9e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0ed9e-114">Not supported</span></span> |
|<span data-ttu-id="0ed9e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ed9e-115">Application</span></span> | <span data-ttu-id="0ed9e-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed9e-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ed9e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ed9e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ed9e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ed9e-118">Optional query parameters</span></span>
<span data-ttu-id="0ed9e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ed9e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ed9e-120">Request headers</span></span>
| <span data-ttu-id="0ed9e-121">名称</span><span class="sxs-lookup"><span data-stu-id="0ed9e-121">Name</span></span> | <span data-ttu-id="0ed9e-122">说明</span><span class="sxs-lookup"><span data-stu-id="0ed9e-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0ed9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ed9e-123">Authorization</span></span> | <span data-ttu-id="0ed9e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ed9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ed9e-126">Request body</span></span>
<span data-ttu-id="0ed9e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ed9e-128">响应</span><span class="sxs-lookup"><span data-stu-id="0ed9e-128">Response</span></span>

<span data-ttu-id="0ed9e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ed9e-130">示例</span><span class="sxs-lookup"><span data-stu-id="0ed9e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ed9e-131">请求</span><span class="sxs-lookup"><span data-stu-id="0ed9e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0ed9e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ed9e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="0ed9e-133">C#</span><span class="sxs-lookup"><span data-stu-id="0ed9e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ed9e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ed9e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ed9e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ed9e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ed9e-136">Java</span><span class="sxs-lookup"><span data-stu-id="0ed9e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ed9e-137">响应</span><span class="sxs-lookup"><span data-stu-id="0ed9e-137">Response</span></span>

<span data-ttu-id="0ed9e-138">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ed9e-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
