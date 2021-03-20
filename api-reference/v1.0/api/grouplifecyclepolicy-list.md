---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ed1f2098dc67ca65a81671b49073d2fcc0764ff9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949882"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="f95ba-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f95ba-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="f95ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f95ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f95ba-105">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="f95ba-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f95ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="f95ba-106">Permissions</span></span>

<span data-ttu-id="f95ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f95ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f95ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f95ba-109">Permission type</span></span>      | <span data-ttu-id="f95ba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f95ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f95ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f95ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f95ba-112">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95ba-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f95ba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f95ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f95ba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f95ba-114">Not supported.</span></span>    |
|<span data-ttu-id="f95ba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f95ba-115">Application</span></span> | <span data-ttu-id="f95ba-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95ba-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f95ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f95ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f95ba-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f95ba-118">Optional query parameters</span></span>
<span data-ttu-id="f95ba-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f95ba-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f95ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f95ba-120">Request headers</span></span>
| <span data-ttu-id="f95ba-121">名称</span><span class="sxs-lookup"><span data-stu-id="f95ba-121">Name</span></span> | <span data-ttu-id="f95ba-122">说明</span><span class="sxs-lookup"><span data-stu-id="f95ba-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="f95ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f95ba-123">Authorization</span></span> | <span data-ttu-id="f95ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f95ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f95ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f95ba-126">Request body</span></span>
<span data-ttu-id="f95ba-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f95ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f95ba-128">响应</span><span class="sxs-lookup"><span data-stu-id="f95ba-128">Response</span></span>

<span data-ttu-id="f95ba-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f95ba-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95ba-130">示例</span><span class="sxs-lookup"><span data-stu-id="f95ba-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f95ba-131">请求</span><span class="sxs-lookup"><span data-stu-id="f95ba-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f95ba-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f95ba-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="f95ba-133">C#</span><span class="sxs-lookup"><span data-stu-id="f95ba-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f95ba-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f95ba-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f95ba-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f95ba-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f95ba-136">Java</span><span class="sxs-lookup"><span data-stu-id="f95ba-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f95ba-137">响应</span><span class="sxs-lookup"><span data-stu-id="f95ba-137">Response</span></span>

<span data-ttu-id="f95ba-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f95ba-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
