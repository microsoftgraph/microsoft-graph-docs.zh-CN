---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 98c0826390d06c172ab73a8eba37585e9db7c3f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944142"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="ae51e-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ae51e-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="ae51e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae51e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae51e-105">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="ae51e-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae51e-106">权限</span><span class="sxs-lookup"><span data-stu-id="ae51e-106">Permissions</span></span>

<span data-ttu-id="ae51e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae51e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae51e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae51e-109">Permission type</span></span>      | <span data-ttu-id="ae51e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae51e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae51e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae51e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae51e-112">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae51e-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ae51e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae51e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae51e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="ae51e-114">Not supported</span></span> |
|<span data-ttu-id="ae51e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae51e-115">Application</span></span> | <span data-ttu-id="ae51e-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae51e-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae51e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae51e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae51e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae51e-118">Optional query parameters</span></span>
<span data-ttu-id="ae51e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae51e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae51e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae51e-120">Request headers</span></span>
| <span data-ttu-id="ae51e-121">名称</span><span class="sxs-lookup"><span data-stu-id="ae51e-121">Name</span></span> | <span data-ttu-id="ae51e-122">说明</span><span class="sxs-lookup"><span data-stu-id="ae51e-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ae51e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae51e-123">Authorization</span></span> | <span data-ttu-id="ae51e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae51e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae51e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae51e-126">Request body</span></span>
<span data-ttu-id="ae51e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae51e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae51e-128">响应</span><span class="sxs-lookup"><span data-stu-id="ae51e-128">Response</span></span>

<span data-ttu-id="ae51e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ae51e-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae51e-130">示例</span><span class="sxs-lookup"><span data-stu-id="ae51e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae51e-131">请求</span><span class="sxs-lookup"><span data-stu-id="ae51e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ae51e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae51e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="ae51e-133">C#</span><span class="sxs-lookup"><span data-stu-id="ae51e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae51e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae51e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae51e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae51e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae51e-136">Java</span><span class="sxs-lookup"><span data-stu-id="ae51e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ae51e-137">响应</span><span class="sxs-lookup"><span data-stu-id="ae51e-137">Response</span></span>

<span data-ttu-id="ae51e-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae51e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
