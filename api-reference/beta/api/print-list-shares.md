---
title: 获取共享
description: 检索打印机共享的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f67ba775906e9b21287d48fe1e1cc8bbfbacd89d
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080644"
---
# <a name="list-shares"></a><span data-ttu-id="35177-103">列出共享</span><span class="sxs-lookup"><span data-stu-id="35177-103">List shares</span></span>

<span data-ttu-id="35177-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35177-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35177-105">检索**printerShares**的列表。</span><span class="sxs-lookup"><span data-stu-id="35177-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="35177-106">权限</span><span class="sxs-lookup"><span data-stu-id="35177-106">Permissions</span></span>
<span data-ttu-id="35177-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="35177-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="35177-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="35177-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35177-110">Permission type</span></span> | <span data-ttu-id="35177-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35177-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="35177-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35177-112">Delegated (work or school account)</span></span>| <span data-ttu-id="35177-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="35177-113">Users.Read.All</span></span> |
|<span data-ttu-id="35177-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35177-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35177-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35177-115">Not Supported.</span></span>|
|<span data-ttu-id="35177-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="35177-116">Application</span></span>|<span data-ttu-id="35177-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="35177-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35177-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35177-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35177-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35177-119">Optional query parameters</span></span>
<span data-ttu-id="35177-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35177-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="35177-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="35177-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="35177-122">若要查看每个打印机共享的功能的列表，请包含可选的 `$select=capabilities` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="35177-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="35177-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="35177-123">Exceptions</span></span>
<span data-ttu-id="35177-124">某些运算符不受支持： `$count` 、 `$orderby` 、 `$search` 。</span><span class="sxs-lookup"><span data-stu-id="35177-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35177-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="35177-125">Request headers</span></span>
| <span data-ttu-id="35177-126">名称</span><span class="sxs-lookup"><span data-stu-id="35177-126">Name</span></span>      |<span data-ttu-id="35177-127">说明</span><span class="sxs-lookup"><span data-stu-id="35177-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35177-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="35177-128">Authorization</span></span> | <span data-ttu-id="35177-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35177-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35177-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="35177-131">Request body</span></span>
<span data-ttu-id="35177-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35177-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="35177-133">响应</span><span class="sxs-lookup"><span data-stu-id="35177-133">Response</span></span>
<span data-ttu-id="35177-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printerShare](../resources/printershare.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="35177-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35177-135">示例</span><span class="sxs-lookup"><span data-stu-id="35177-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35177-136">请求</span><span class="sxs-lookup"><span data-stu-id="35177-136">Request</span></span>
<span data-ttu-id="35177-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="35177-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35177-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="35177-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="35177-139">C#</span><span class="sxs-lookup"><span data-stu-id="35177-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35177-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35177-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35177-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35177-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35177-142">响应</span><span class="sxs-lookup"><span data-stu-id="35177-142">Response</span></span>
<span data-ttu-id="35177-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="35177-143">The following is an example of the response.</span></span>
><span data-ttu-id="35177-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35177-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
