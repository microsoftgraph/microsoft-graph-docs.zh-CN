---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 363e3a5d5ca3d20c26ed6aeef9ad576bf318929f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953669"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="44950-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="44950-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="44950-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44950-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44950-105">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="44950-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="44950-106">权限</span><span class="sxs-lookup"><span data-stu-id="44950-106">Permissions</span></span>

<span data-ttu-id="44950-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="44950-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44950-109">Permission type</span></span>      | <span data-ttu-id="44950-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44950-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44950-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44950-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44950-112">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44950-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="44950-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44950-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44950-114">不支持</span><span class="sxs-lookup"><span data-stu-id="44950-114">Not supported</span></span> |
|<span data-ttu-id="44950-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44950-115">Application</span></span> | <span data-ttu-id="44950-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44950-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44950-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44950-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="44950-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="44950-118">Optional query parameters</span></span>
<span data-ttu-id="44950-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="44950-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44950-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44950-120">Request headers</span></span>
| <span data-ttu-id="44950-121">名称</span><span class="sxs-lookup"><span data-stu-id="44950-121">Name</span></span> | <span data-ttu-id="44950-122">说明</span><span class="sxs-lookup"><span data-stu-id="44950-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="44950-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44950-123">Authorization</span></span> | <span data-ttu-id="44950-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44950-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44950-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="44950-126">Request body</span></span>
<span data-ttu-id="44950-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44950-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44950-128">响应</span><span class="sxs-lookup"><span data-stu-id="44950-128">Response</span></span>

<span data-ttu-id="44950-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="44950-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44950-130">示例</span><span class="sxs-lookup"><span data-stu-id="44950-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="44950-131">请求</span><span class="sxs-lookup"><span data-stu-id="44950-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="44950-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="44950-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="44950-133">C#</span><span class="sxs-lookup"><span data-stu-id="44950-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44950-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44950-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44950-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44950-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44950-136">Java</span><span class="sxs-lookup"><span data-stu-id="44950-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44950-137">响应</span><span class="sxs-lookup"><span data-stu-id="44950-137">Response</span></span>

<span data-ttu-id="44950-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44950-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
