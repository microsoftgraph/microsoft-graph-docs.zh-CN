---
title: 获取 taskDefinition
description: 获取有关任务定义的详细信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 295aa68b62ce6444248dbed30dd2bbae1c0f1751
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968167"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="0e1d5-103">获取 taskDefinition</span><span class="sxs-lookup"><span data-stu-id="0e1d5-103">Get taskDefinition</span></span>

<span data-ttu-id="0e1d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e1d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e1d5-105">获取有关任务定义的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-105">Get details about a task definition.</span></span>

<span data-ttu-id="0e1d5-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅 [扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e1d5-107">权限</span><span class="sxs-lookup"><span data-stu-id="0e1d5-107">Permissions</span></span>
<span data-ttu-id="0e1d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0e1d5-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0e1d5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e1d5-111">Permission type</span></span> | <span data-ttu-id="0e1d5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e1d5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0e1d5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e1d5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0e1d5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-114">Not supported.</span></span> |
|<span data-ttu-id="0e1d5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e1d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e1d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-116">Not Supported.</span></span>|
|<span data-ttu-id="0e1d5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e1d5-117">Application</span></span>| <span data-ttu-id="0e1d5-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e1d5-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e1d5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e1d5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e1d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e1d5-120">Request headers</span></span>
| <span data-ttu-id="0e1d5-121">名称</span><span class="sxs-lookup"><span data-stu-id="0e1d5-121">Name</span></span>      |<span data-ttu-id="0e1d5-122">说明</span><span class="sxs-lookup"><span data-stu-id="0e1d5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e1d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e1d5-123">Authorization</span></span> | <span data-ttu-id="0e1d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e1d5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e1d5-126">Request body</span></span>
<span data-ttu-id="0e1d5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0e1d5-128">响应</span><span class="sxs-lookup"><span data-stu-id="0e1d5-128">Response</span></span>
<span data-ttu-id="0e1d5-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printTaskDefinition](../resources/printtaskdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e1d5-130">示例</span><span class="sxs-lookup"><span data-stu-id="0e1d5-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e1d5-131">请求</span><span class="sxs-lookup"><span data-stu-id="0e1d5-131">Request</span></span>
<span data-ttu-id="0e1d5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e1d5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e1d5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```
# <a name="c"></a>[<span data-ttu-id="0e1d5-134">C#</span><span class="sxs-lookup"><span data-stu-id="0e1d5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e1d5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e1d5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e1d5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e1d5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e1d5-137">Java</span><span class="sxs-lookup"><span data-stu-id="0e1d5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="0e1d5-138">响应</span><span class="sxs-lookup"><span data-stu-id="0e1d5-138">Response</span></span>
<span data-ttu-id="0e1d5-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-139">The following is an example of the response.</span></span>
><span data-ttu-id="0e1d5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0e1d5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


