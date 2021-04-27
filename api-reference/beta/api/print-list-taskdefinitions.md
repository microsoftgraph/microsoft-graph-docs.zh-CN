---
title: List taskDefinitions
description: 检索请求应用在租户中定义的任务定义列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 68de2409013cff88752f5a26f1ea06e2a25bb755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053634"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="76ad5-103">List taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="76ad5-103">List taskDefinitions</span></span>

<span data-ttu-id="76ad5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76ad5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76ad5-105">检索请求 [应用在](../resources/printtaskdefinition.md) 租户中定义的任务定义列表。</span><span class="sxs-lookup"><span data-stu-id="76ad5-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="76ad5-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="76ad5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="76ad5-107">权限</span><span class="sxs-lookup"><span data-stu-id="76ad5-107">Permissions</span></span>
<span data-ttu-id="76ad5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="76ad5-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="76ad5-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="76ad5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76ad5-111">Permission type</span></span> | <span data-ttu-id="76ad5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76ad5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="76ad5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76ad5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="76ad5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76ad5-114">Not supported.</span></span> |
|<span data-ttu-id="76ad5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76ad5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76ad5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76ad5-116">Not Supported.</span></span>|
|<span data-ttu-id="76ad5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="76ad5-117">Application</span></span>| <span data-ttu-id="76ad5-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76ad5-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76ad5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76ad5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76ad5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76ad5-120">Optional query parameters</span></span>
<span data-ttu-id="76ad5-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76ad5-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="76ad5-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="76ad5-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="76ad5-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="76ad5-123">Exceptions</span></span>
<span data-ttu-id="76ad5-124">不支持某些运算符 `$count` `$format` ：、、、、、。 `$search` `$select` `$skip` `$top`</span><span class="sxs-lookup"><span data-stu-id="76ad5-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76ad5-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="76ad5-125">Request headers</span></span>
| <span data-ttu-id="76ad5-126">名称</span><span class="sxs-lookup"><span data-stu-id="76ad5-126">Name</span></span>      |<span data-ttu-id="76ad5-127">说明</span><span class="sxs-lookup"><span data-stu-id="76ad5-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76ad5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="76ad5-128">Authorization</span></span> | <span data-ttu-id="76ad5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76ad5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76ad5-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="76ad5-131">Request body</span></span>
<span data-ttu-id="76ad5-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76ad5-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="76ad5-133">响应</span><span class="sxs-lookup"><span data-stu-id="76ad5-133">Response</span></span>
<span data-ttu-id="76ad5-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="76ad5-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76ad5-135">示例</span><span class="sxs-lookup"><span data-stu-id="76ad5-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="76ad5-136">请求</span><span class="sxs-lookup"><span data-stu-id="76ad5-136">Request</span></span>
<span data-ttu-id="76ad5-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76ad5-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="76ad5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="76ad5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```
# <a name="c"></a>[<span data-ttu-id="76ad5-139">C#</span><span class="sxs-lookup"><span data-stu-id="76ad5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-list-taskdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76ad5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76ad5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-list-taskdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76ad5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76ad5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-list-taskdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76ad5-142">Java</span><span class="sxs-lookup"><span data-stu-id="76ad5-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-list-taskdefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="76ad5-143">响应</span><span class="sxs-lookup"><span data-stu-id="76ad5-143">Response</span></span>
<span data-ttu-id="76ad5-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76ad5-144">The following is an example of the response.</span></span>
><span data-ttu-id="76ad5-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="76ad5-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


