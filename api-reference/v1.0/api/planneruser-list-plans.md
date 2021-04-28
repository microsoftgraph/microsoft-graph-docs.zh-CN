---
title: 列出计划
description: 检索与 user 对象共享的 **plannerplan** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 0fee8525da4a29a4a610ec847cdd8c8776edcdac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055839"
---
# <a name="list-plans"></a><span data-ttu-id="357c5-103">列出计划</span><span class="sxs-lookup"><span data-stu-id="357c5-103">List plans</span></span>

<span data-ttu-id="357c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="357c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="357c5-105">检索与 [user](../resources/user.md) 对象共享的 **plannerplan** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="357c5-105">Retrieve a list of **plannerplan** objects shared with a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="357c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="357c5-106">Permissions</span></span>
<span data-ttu-id="357c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="357c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="357c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="357c5-109">Permission type</span></span>      | <span data-ttu-id="357c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="357c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="357c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="357c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="357c5-112">任务.读取，任务.ReadWrite，Group.Read.All，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="357c5-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="357c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="357c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="357c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="357c5-114">Not supported.</span></span>    |
|<span data-ttu-id="357c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="357c5-115">Application</span></span> | <span data-ttu-id="357c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="357c5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="357c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="357c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/plans
GET /users/{id}/planner/plans
GET /drive/root/createdByUser/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="357c5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="357c5-118">Request headers</span></span>
| <span data-ttu-id="357c5-119">名称</span><span class="sxs-lookup"><span data-stu-id="357c5-119">Name</span></span>      |<span data-ttu-id="357c5-120">说明</span><span class="sxs-lookup"><span data-stu-id="357c5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="357c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="357c5-121">Authorization</span></span>  | <span data-ttu-id="357c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="357c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="357c5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="357c5-124">Request body</span></span>
<span data-ttu-id="357c5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="357c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="357c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="357c5-126">Response</span></span>

<span data-ttu-id="357c5-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="357c5-127">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="357c5-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="357c5-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="357c5-131">示例</span><span class="sxs-lookup"><span data-stu-id="357c5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="357c5-132">请求</span><span class="sxs-lookup"><span data-stu-id="357c5-132">Request</span></span>
<span data-ttu-id="357c5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="357c5-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="357c5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="357c5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="357c5-135">C#</span><span class="sxs-lookup"><span data-stu-id="357c5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="357c5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="357c5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="357c5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="357c5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="357c5-138">Java</span><span class="sxs-lookup"><span data-stu-id="357c5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="357c5-139">响应</span><span class="sxs-lookup"><span data-stu-id="357c5-139">Response</span></span>
<span data-ttu-id="357c5-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="357c5-140">Here is an example of the response.</span></span> <span data-ttu-id="357c5-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="357c5-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 438

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

