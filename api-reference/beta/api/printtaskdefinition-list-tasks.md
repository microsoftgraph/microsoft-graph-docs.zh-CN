---
title: 列出任务
description: 检索与任务定义关联的任务列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e489a7a1c34a60d1f1da45d151a50e46511e6ca0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053578"
---
# <a name="list-tasks"></a><span data-ttu-id="ab643-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="ab643-103">List tasks</span></span>

<span data-ttu-id="ab643-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab643-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab643-105">检索与 [任务定义](../resources/printtask.md) 相关联的任务 [列表](../resources/printtaskdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="ab643-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="ab643-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="ab643-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab643-107">权限</span><span class="sxs-lookup"><span data-stu-id="ab643-107">Permissions</span></span>
<span data-ttu-id="ab643-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ab643-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ab643-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ab643-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab643-111">Permission type</span></span> | <span data-ttu-id="ab643-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab643-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ab643-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab643-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ab643-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab643-114">Not supported.</span></span> |
|<span data-ttu-id="ab643-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab643-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab643-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab643-116">Not Supported.</span></span>|
|<span data-ttu-id="ab643-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab643-117">Application</span></span>| <span data-ttu-id="ab643-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab643-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab643-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab643-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab643-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab643-120">Optional query parameters</span></span>
<span data-ttu-id="ab643-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ab643-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab643-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ab643-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="ab643-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ab643-123">Exceptions</span></span>
<span data-ttu-id="ab643-124">不支持某些运算符 `$count` `$format` ：、、、、、。 `$search` `$select` `$skip` `$top`</span><span class="sxs-lookup"><span data-stu-id="ab643-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab643-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab643-125">Request headers</span></span>
| <span data-ttu-id="ab643-126">名称</span><span class="sxs-lookup"><span data-stu-id="ab643-126">Name</span></span>      |<span data-ttu-id="ab643-127">说明</span><span class="sxs-lookup"><span data-stu-id="ab643-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab643-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab643-128">Authorization</span></span> | <span data-ttu-id="ab643-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab643-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab643-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab643-131">Request body</span></span>
<span data-ttu-id="ab643-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab643-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ab643-133">响应</span><span class="sxs-lookup"><span data-stu-id="ab643-133">Response</span></span>
<span data-ttu-id="ab643-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printTask](../resources/printtask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab643-134">If successful, this method returns a `200 OK` response code and collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab643-135">示例</span><span class="sxs-lookup"><span data-stu-id="ab643-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab643-136">请求</span><span class="sxs-lookup"><span data-stu-id="ab643-136">Request</span></span>
<span data-ttu-id="ab643-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab643-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ab643-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab643-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks
```
# <a name="c"></a>[<span data-ttu-id="ab643-139">C#</span><span class="sxs-lookup"><span data-stu-id="ab643-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtaskdefinition-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab643-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab643-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtaskdefinition-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab643-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab643-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtaskdefinition-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab643-142">Java</span><span class="sxs-lookup"><span data-stu-id="ab643-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtaskdefinition-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="ab643-143">响应</span><span class="sxs-lookup"><span data-stu-id="ab643-143">Response</span></span>
<span data-ttu-id="ab643-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab643-144">The following is an example of the response.</span></span>
><span data-ttu-id="ab643-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ab643-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 429

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printTask)",
  "value": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


