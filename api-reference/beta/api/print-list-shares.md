---
title: 获取共享
description: 检索打印机共享的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 045df17f2d59f7d8f3081fb28b8a39314e9cacf1
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766502"
---
# <a name="list-shares"></a><span data-ttu-id="b356e-103">列出共享项</span><span class="sxs-lookup"><span data-stu-id="b356e-103">List shares</span></span>

<span data-ttu-id="b356e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b356e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b356e-105">检索 **printerShares 列表**。</span><span class="sxs-lookup"><span data-stu-id="b356e-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b356e-106">权限</span><span class="sxs-lookup"><span data-stu-id="b356e-106">Permissions</span></span>
<span data-ttu-id="b356e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b356e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b356e-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="b356e-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="b356e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b356e-110">Permission type</span></span> | <span data-ttu-id="b356e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b356e-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b356e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b356e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b356e-113">PrinterShare.ReadBasic.All、PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b356e-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="b356e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b356e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b356e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b356e-115">Not Supported.</span></span>|
|<span data-ttu-id="b356e-116">Application</span><span class="sxs-lookup"><span data-stu-id="b356e-116">Application</span></span>|<span data-ttu-id="b356e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b356e-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b356e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b356e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b356e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b356e-119">Optional query parameters</span></span>
<span data-ttu-id="b356e-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b356e-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b356e-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b356e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="b356e-122">若要查看每个打印机共享功能的列表，请包含可选的 `$select=capabilities` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="b356e-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="b356e-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b356e-123">Exceptions</span></span>
<span data-ttu-id="b356e-124">不支持某些运算符 `$count` `$orderby` ：、、。 `$search`</span><span class="sxs-lookup"><span data-stu-id="b356e-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b356e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b356e-125">Request headers</span></span>
| <span data-ttu-id="b356e-126">名称</span><span class="sxs-lookup"><span data-stu-id="b356e-126">Name</span></span>      |<span data-ttu-id="b356e-127">说明</span><span class="sxs-lookup"><span data-stu-id="b356e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b356e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b356e-128">Authorization</span></span> | <span data-ttu-id="b356e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b356e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b356e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b356e-131">Request body</span></span>
<span data-ttu-id="b356e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b356e-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b356e-133">响应</span><span class="sxs-lookup"><span data-stu-id="b356e-133">Response</span></span>
<span data-ttu-id="b356e-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printerShare](../resources/printershare.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b356e-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b356e-135">示例</span><span class="sxs-lookup"><span data-stu-id="b356e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b356e-136">请求</span><span class="sxs-lookup"><span data-stu-id="b356e-136">Request</span></span>
<span data-ttu-id="b356e-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b356e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b356e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b356e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="b356e-139">C#</span><span class="sxs-lookup"><span data-stu-id="b356e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b356e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b356e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b356e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b356e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b356e-142">Java</span><span class="sxs-lookup"><span data-stu-id="b356e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shares-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b356e-143">响应</span><span class="sxs-lookup"><span data-stu-id="b356e-143">Response</span></span>
<span data-ttu-id="b356e-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b356e-144">The following is an example of the response.</span></span>
><span data-ttu-id="b356e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b356e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "displayName": "PrinterShareName",
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


