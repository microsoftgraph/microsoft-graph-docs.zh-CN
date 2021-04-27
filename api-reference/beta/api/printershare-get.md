---
title: 获取 printerShare
description: 检索打印机共享的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 046d5a107ea2b92adf17bb24f585138764757b50
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037485"
---
# <a name="get-printershare"></a><span data-ttu-id="9bd0b-103">获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="9bd0b-103">Get printerShare</span></span>

<span data-ttu-id="9bd0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd0b-105">检索打印机共享的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bd0b-106">权限</span><span class="sxs-lookup"><span data-stu-id="9bd0b-106">Permissions</span></span>
<span data-ttu-id="9bd0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9bd0b-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9bd0b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bd0b-110">Permission type</span></span> | <span data-ttu-id="9bd0b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bd0b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9bd0b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd0b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9bd0b-113">PrinterShare.ReadBasic.All、PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd0b-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="9bd0b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bd0b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-115">Not Supported.</span></span>|
|<span data-ttu-id="9bd0b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bd0b-116">Application</span></span>|<span data-ttu-id="9bd0b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bd0b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bd0b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bd0b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9bd0b-119">Optional query parameters</span></span>
<span data-ttu-id="9bd0b-120">此方法支持一些 OData 查询参数，$select、$expand自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-120">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="9bd0b-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="9bd0b-122">例如</span><span class="sxs-lookup"><span data-stu-id="9bd0b-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```

### <a name="exceptions"></a><span data-ttu-id="9bd0b-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="9bd0b-123">Exceptions</span></span>
* <span data-ttu-id="9bd0b-124">`$count`运算符不受支持。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-124">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bd0b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bd0b-125">Request headers</span></span>
| <span data-ttu-id="9bd0b-126">名称</span><span class="sxs-lookup"><span data-stu-id="9bd0b-126">Name</span></span>      |<span data-ttu-id="9bd0b-127">说明</span><span class="sxs-lookup"><span data-stu-id="9bd0b-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9bd0b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd0b-128">Authorization</span></span> | <span data-ttu-id="9bd0b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bd0b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bd0b-131">Request body</span></span>
<span data-ttu-id="9bd0b-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9bd0b-133">响应</span><span class="sxs-lookup"><span data-stu-id="9bd0b-133">Response</span></span>
<span data-ttu-id="9bd0b-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-134">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="9bd0b-135">默认情况下，该响应将不包含 [printerCapabilities](../resources/printerCapabilities.md)。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-135">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="9bd0b-136">若要获取 **printerCapabilities，** 请使用 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-136">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="9bd0b-137">示例</span><span class="sxs-lookup"><span data-stu-id="9bd0b-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bd0b-138">请求</span><span class="sxs-lookup"><span data-stu-id="9bd0b-138">Request</span></span>
<span data-ttu-id="9bd0b-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bd0b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bd0b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="9bd0b-141">C#</span><span class="sxs-lookup"><span data-stu-id="9bd0b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bd0b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bd0b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bd0b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bd0b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bd0b-144">Java</span><span class="sxs-lookup"><span data-stu-id="9bd0b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9bd0b-145">响应</span><span class="sxs-lookup"><span data-stu-id="9bd0b-145">Response</span></span>
<span data-ttu-id="9bd0b-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-146">The following is an example of the response.</span></span>
><span data-ttu-id="9bd0b-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<span data-ttu-id="9bd0b-148">下面是使用 $select=id，displayName，capabilities 时的响应示例</span><span class="sxs-lookup"><span data-stu-id="9bd0b-148">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="9bd0b-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9bd0b-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "capabilities": {
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "contentTypes": [
      "application/pdf",
      "image/pwg-raster",
      "application/PCLm"
    ],
    "isPageRangeSupported": false,
    "qualities": [
      "medium"
    ],
    "dpis": [
      600
    ],
    "duplexModes": [
      "oneSided",
      "flipOnLongEdge",
      "flipOnShortEdge"
    ],
    "finishings": [
      "none"
    ],
    "mediaTypes": [
      "stationery"
    ],
    "mediaSizes": [
      "North America Letter"
    ],
    "outputBins": [
      "tray-1"
    ],
    "colorModes": [
      "grayscale",
      "color"
    ],
    "inputBins": [
      "tray-1"
    ],
    "collation": true,
    "scalings": [
      "fill"
    ],
    "copiesPerJob": {
      "start": 1,
      "end": 38
    }
  }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


