---
title: 获取共享
description: 检索打印机共享的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 80da97475b6d8f79107034b441a06e58de9dc806
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022258"
---
# <a name="list-shares"></a><span data-ttu-id="c4cd3-103">列出共享项</span><span class="sxs-lookup"><span data-stu-id="c4cd3-103">List shares</span></span>

<span data-ttu-id="c4cd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4cd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4cd3-105">检索 **printerShares**的列表。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4cd3-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4cd3-106">Permissions</span></span>
<span data-ttu-id="c4cd3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c4cd3-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="c4cd3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4cd3-110">Permission type</span></span> | <span data-ttu-id="c4cd3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4cd3-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c4cd3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4cd3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c4cd3-113">PrinterShare、PrinterShare 和所有</span><span class="sxs-lookup"><span data-stu-id="c4cd3-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c4cd3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4cd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4cd3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-115">Not Supported.</span></span>|
|<span data-ttu-id="c4cd3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4cd3-116">Application</span></span>|<span data-ttu-id="c4cd3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4cd3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4cd3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4cd3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4cd3-119">Optional query parameters</span></span>
<span data-ttu-id="c4cd3-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c4cd3-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="c4cd3-122">若要查看每个打印机共享的功能的列表，请包含可选的 `$select=capabilities` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="c4cd3-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c4cd3-123">Exceptions</span></span>
<span data-ttu-id="c4cd3-124">某些运算符不受支持： `$count` 、 `$orderby` 、 `$search` 。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4cd3-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4cd3-125">Request headers</span></span>
| <span data-ttu-id="c4cd3-126">名称</span><span class="sxs-lookup"><span data-stu-id="c4cd3-126">Name</span></span>      |<span data-ttu-id="c4cd3-127">说明</span><span class="sxs-lookup"><span data-stu-id="c4cd3-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4cd3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4cd3-128">Authorization</span></span> | <span data-ttu-id="c4cd3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4cd3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4cd3-131">Request body</span></span>
<span data-ttu-id="c4cd3-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c4cd3-133">响应</span><span class="sxs-lookup"><span data-stu-id="c4cd3-133">Response</span></span>
<span data-ttu-id="c4cd3-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printerShare](../resources/printershare.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4cd3-135">示例</span><span class="sxs-lookup"><span data-stu-id="c4cd3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4cd3-136">请求</span><span class="sxs-lookup"><span data-stu-id="c4cd3-136">Request</span></span>
<span data-ttu-id="c4cd3-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4cd3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4cd3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="c4cd3-139">C#</span><span class="sxs-lookup"><span data-stu-id="c4cd3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4cd3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4cd3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4cd3-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4cd3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4cd3-142">响应</span><span class="sxs-lookup"><span data-stu-id="c4cd3-142">Response</span></span>
<span data-ttu-id="c4cd3-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-143">The following is an example of the response.</span></span>
><span data-ttu-id="c4cd3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4cd3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterShareName",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List shares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


