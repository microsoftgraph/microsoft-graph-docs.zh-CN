---
title: 列出任务
description: 检索与任务定义关联的任务列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 38948e3a6844654b11f9af6b7ded7ea86b1afb3a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768652"
---
# <a name="list-tasks"></a><span data-ttu-id="87428-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="87428-103">List tasks</span></span>
<span data-ttu-id="87428-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87428-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="87428-105">检索与 [任务定义](../resources/printtask.md) 相关联的任务 [列表](../resources/printtaskdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="87428-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="87428-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="87428-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="87428-107">权限</span><span class="sxs-lookup"><span data-stu-id="87428-107">Permissions</span></span>
<span data-ttu-id="87428-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87428-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="87428-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="87428-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="87428-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87428-111">Permission type</span></span> | <span data-ttu-id="87428-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87428-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="87428-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87428-113">Delegated (work or school account)</span></span>| <span data-ttu-id="87428-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="87428-114">Not supported.</span></span> |
|<span data-ttu-id="87428-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87428-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87428-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87428-116">Not Supported.</span></span>|
|<span data-ttu-id="87428-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87428-117">Application</span></span>| <span data-ttu-id="87428-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87428-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87428-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87428-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87428-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="87428-120">Optional query parameters</span></span>
<span data-ttu-id="87428-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="87428-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="87428-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="87428-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="87428-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="87428-123">Exceptions</span></span>
<span data-ttu-id="87428-124">不支持某些运算符 `$count` `$format` ：、、、、、。 `$search` `$select` `$skip` `$top`</span><span class="sxs-lookup"><span data-stu-id="87428-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87428-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="87428-125">Request headers</span></span>
|<span data-ttu-id="87428-126">名称</span><span class="sxs-lookup"><span data-stu-id="87428-126">Name</span></span>|<span data-ttu-id="87428-127">说明</span><span class="sxs-lookup"><span data-stu-id="87428-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="87428-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="87428-128">Authorization</span></span>|<span data-ttu-id="87428-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87428-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87428-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="87428-131">Request body</span></span>
<span data-ttu-id="87428-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87428-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87428-133">响应</span><span class="sxs-lookup"><span data-stu-id="87428-133">Response</span></span>

<span data-ttu-id="87428-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printTask](../resources/printtask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="87428-134">If successful, this method returns a `200 OK` response code and a collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87428-135">示例</span><span class="sxs-lookup"><span data-stu-id="87428-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87428-136">请求</span><span class="sxs-lookup"><span data-stu-id="87428-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="87428-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="87428-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks
```
# <a name="c"></a>[<span data-ttu-id="87428-138">C#</span><span class="sxs-lookup"><span data-stu-id="87428-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87428-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87428-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87428-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87428-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87428-141">Java</span><span class="sxs-lookup"><span data-stu-id="87428-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87428-142">响应</span><span class="sxs-lookup"><span data-stu-id="87428-142">Response</span></span>
<span data-ttu-id="87428-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="87428-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printTask)",
  "value": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

