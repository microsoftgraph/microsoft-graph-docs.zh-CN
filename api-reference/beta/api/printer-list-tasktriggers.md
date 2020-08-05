---
title: List taskTriggers
description: 检索与打印机关联的任务触发器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 189830fb76de676163a24a8166cff6017cceffc5
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565893"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="31c64-103">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="31c64-103">List taskTriggers</span></span>

<span data-ttu-id="31c64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31c64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31c64-105">检索与[打印机](../resources/printer.md)关联的[任务触发器](../resources/printtasktrigger.md)列表。</span><span class="sxs-lookup"><span data-stu-id="31c64-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="31c64-106">任务触发器列表定义由于打印过程中发生的事件而将触发的任务。</span><span class="sxs-lookup"><span data-stu-id="31c64-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="31c64-107">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="31c64-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="31c64-108">权限</span><span class="sxs-lookup"><span data-stu-id="31c64-108">Permissions</span></span>
<span data-ttu-id="31c64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31c64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="31c64-111">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="31c64-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="31c64-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="31c64-112">Permission type</span></span> | <span data-ttu-id="31c64-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31c64-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="31c64-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31c64-114">Delegated (work or school account)</span></span>| <span data-ttu-id="31c64-115">Printer。 all，完全控制，All，All</span><span class="sxs-lookup"><span data-stu-id="31c64-115">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="31c64-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31c64-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31c64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="31c64-117">Not Supported.</span></span>|
|<span data-ttu-id="31c64-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="31c64-118">Application</span></span>| <span data-ttu-id="31c64-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="31c64-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31c64-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31c64-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31c64-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31c64-121">Optional query parameters</span></span>
<span data-ttu-id="31c64-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31c64-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="31c64-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="31c64-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="31c64-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="31c64-124">Exceptions</span></span>
<span data-ttu-id="31c64-125">某些运算符不受支持：、、、、 `$count` `$format` `$search` `$select` `$skip` 、 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="31c64-125">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31c64-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="31c64-126">Request headers</span></span>
| <span data-ttu-id="31c64-127">名称</span><span class="sxs-lookup"><span data-stu-id="31c64-127">Name</span></span>      |<span data-ttu-id="31c64-128">说明</span><span class="sxs-lookup"><span data-stu-id="31c64-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31c64-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="31c64-129">Authorization</span></span> | <span data-ttu-id="31c64-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31c64-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31c64-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="31c64-132">Request body</span></span>
<span data-ttu-id="31c64-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31c64-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31c64-134">响应</span><span class="sxs-lookup"><span data-stu-id="31c64-134">Response</span></span>
<span data-ttu-id="31c64-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printTaskTrigger](../resources/printtasktrigger.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="31c64-135">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31c64-136">示例</span><span class="sxs-lookup"><span data-stu-id="31c64-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="31c64-137">请求</span><span class="sxs-lookup"><span data-stu-id="31c64-137">Request</span></span>
<span data-ttu-id="31c64-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31c64-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31c64-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="31c64-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="31c64-140">C#</span><span class="sxs-lookup"><span data-stu-id="31c64-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31c64-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31c64-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31c64-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31c64-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="31c64-143">响应</span><span class="sxs-lookup"><span data-stu-id="31c64-143">Response</span></span>
<span data-ttu-id="31c64-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31c64-144">The following is an example of the response.</span></span>
><span data-ttu-id="31c64-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="31c64-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskTriggers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
