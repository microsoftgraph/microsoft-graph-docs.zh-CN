---
title: 列出作业
description: 检索与打印机关联的打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5b8c16df2985e03e8b2aacc4e9463618102d93b4
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947852"
---
# <a name="list-jobs"></a><span data-ttu-id="09283-103">列出作业</span><span class="sxs-lookup"><span data-stu-id="09283-103">List jobs</span></span>

<span data-ttu-id="09283-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09283-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09283-105">检索与[打印机](../resources/printer.md)关联的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="09283-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09283-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="09283-106">Permissions</span></span>
<span data-ttu-id="09283-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="09283-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="09283-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="09283-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="09283-110">Permission type</span></span> | <span data-ttu-id="09283-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09283-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="09283-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09283-112">Delegated (work or school account)</span></span>| <span data-ttu-id="09283-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="09283-113">Users.Read.All</span></span> |
|<span data-ttu-id="09283-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09283-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09283-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="09283-115">Not Supported.</span></span>|
|<span data-ttu-id="09283-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="09283-116">Application</span></span>|<span data-ttu-id="09283-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="09283-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09283-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09283-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="09283-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="09283-119">Request headers</span></span>
| <span data-ttu-id="09283-120">名称</span><span class="sxs-lookup"><span data-stu-id="09283-120">Name</span></span>      |<span data-ttu-id="09283-121">说明</span><span class="sxs-lookup"><span data-stu-id="09283-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09283-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09283-122">Authorization</span></span> | <span data-ttu-id="09283-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09283-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09283-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="09283-125">Request body</span></span>
<span data-ttu-id="09283-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09283-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="09283-127">响应</span><span class="sxs-lookup"><span data-stu-id="09283-127">Response</span></span>
<span data-ttu-id="09283-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printJob](../resources/printjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="09283-128">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09283-129">示例</span><span class="sxs-lookup"><span data-stu-id="09283-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09283-130">请求</span><span class="sxs-lookup"><span data-stu-id="09283-130">Request</span></span>
<span data-ttu-id="09283-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09283-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09283-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="09283-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="09283-133">C#</span><span class="sxs-lookup"><span data-stu-id="09283-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09283-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09283-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09283-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09283-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="09283-136">响应</span><span class="sxs-lookup"><span data-stu-id="09283-136">Response</span></span>
<span data-ttu-id="09283-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09283-137">The following is an example of the response.</span></span>
><span data-ttu-id="09283-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09283-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
