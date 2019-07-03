---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c189ea32cd67b025c0182e6e25a853637f0320aa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445693"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="9cdd9-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9cdd9-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="9cdd9-104">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cdd9-105">权限</span><span class="sxs-lookup"><span data-stu-id="9cdd9-105">Permissions</span></span>

<span data-ttu-id="9cdd9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9cdd9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cdd9-108">Permission type</span></span>      | <span data-ttu-id="9cdd9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cdd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cdd9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cdd9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9cdd9-111">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cdd9-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9cdd9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cdd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cdd9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-113">Not supported.</span></span>    |
|<span data-ttu-id="9cdd9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cdd9-114">Application</span></span> | <span data-ttu-id="9cdd9-115">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cdd9-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cdd9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cdd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9cdd9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9cdd9-117">Optional query parameters</span></span>
<span data-ttu-id="9cdd9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cdd9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cdd9-119">Request headers</span></span>
| <span data-ttu-id="9cdd9-120">名称</span><span class="sxs-lookup"><span data-stu-id="9cdd9-120">Name</span></span> | <span data-ttu-id="9cdd9-121">说明</span><span class="sxs-lookup"><span data-stu-id="9cdd9-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="9cdd9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cdd9-122">Authorization</span></span> | <span data-ttu-id="9cdd9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cdd9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cdd9-125">Request body</span></span>
<span data-ttu-id="9cdd9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cdd9-127">响应</span><span class="sxs-lookup"><span data-stu-id="9cdd9-127">Response</span></span>

<span data-ttu-id="9cdd9-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cdd9-129">示例</span><span class="sxs-lookup"><span data-stu-id="9cdd9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9cdd9-130">请求</span><span class="sxs-lookup"><span data-stu-id="9cdd9-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cdd9-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9cdd9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cdd9-132">C#</span><span class="sxs-lookup"><span data-stu-id="9cdd9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cdd9-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="9cdd9-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cdd9-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="9cdd9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9cdd9-135">响应</span><span class="sxs-lookup"><span data-stu-id="9cdd9-135">Response</span></span>

<span data-ttu-id="9cdd9-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cdd9-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
