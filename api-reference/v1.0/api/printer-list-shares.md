---
title: 列出 printerShares for a printer
description: 检索 printerShares 与打印机关联的列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d719cc04c4b4bc0694f42e80ce7ae317bc8ef104
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956251"
---
# <a name="list-printershares-for-a-printer"></a><span data-ttu-id="b941f-103">列出 printerShares for a printer</span><span class="sxs-lookup"><span data-stu-id="b941f-103">List printerShares for a printer</span></span>
<span data-ttu-id="b941f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b941f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b941f-105">检索与打印机关联的打印机共享 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="b941f-105">Retrieve a list of printer shares associated with the [printer](../resources/printer.md).</span></span>
><span data-ttu-id="b941f-106">**注意：** 目前，每个 **打印机** 仅支持一个打印机共享。</span><span class="sxs-lookup"><span data-stu-id="b941f-106">**Note:** Currently, only **one** printer share per printer is supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="b941f-107">权限</span><span class="sxs-lookup"><span data-stu-id="b941f-107">Permissions</span></span>
<span data-ttu-id="b941f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b941f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b941f-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="b941f-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="b941f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b941f-111">Permission type</span></span> | <span data-ttu-id="b941f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b941f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b941f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b941f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b941f-114">PrinterShare.ReadBasic.All、PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b941f-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="b941f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b941f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b941f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b941f-116">Not Supported.</span></span>|
|<span data-ttu-id="b941f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b941f-117">Application</span></span>| <span data-ttu-id="b941f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b941f-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b941f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b941f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b941f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b941f-120">Optional query parameters</span></span>
<span data-ttu-id="b941f-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b941f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b941f-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b941f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b941f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b941f-123">Request headers</span></span>
|<span data-ttu-id="b941f-124">名称</span><span class="sxs-lookup"><span data-stu-id="b941f-124">Name</span></span>|<span data-ttu-id="b941f-125">说明</span><span class="sxs-lookup"><span data-stu-id="b941f-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b941f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b941f-126">Authorization</span></span>|<span data-ttu-id="b941f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b941f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b941f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b941f-129">Request body</span></span>
<span data-ttu-id="b941f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b941f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b941f-131">响应</span><span class="sxs-lookup"><span data-stu-id="b941f-131">Response</span></span>

<span data-ttu-id="b941f-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printerShare](../resources/printershare.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b941f-132">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="b941f-133">**注意**：该响应将不包含 **defaults** **和 capabilities** 属性。</span><span class="sxs-lookup"><span data-stu-id="b941f-133">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="b941f-134">可以使用 Get [printerShare](printerShare-get.md) 请求查询这些属性。</span><span class="sxs-lookup"><span data-stu-id="b941f-134">These properties can be queried using a [Get printerShare](printerShare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="b941f-135">示例</span><span class="sxs-lookup"><span data-stu-id="b941f-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b941f-136">请求</span><span class="sxs-lookup"><span data-stu-id="b941f-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b941f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b941f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printershare_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/shares
```
# <a name="c"></a>[<span data-ttu-id="b941f-138">C#</span><span class="sxs-lookup"><span data-stu-id="b941f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printershare-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b941f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b941f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printershare-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b941f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b941f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printershare-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b941f-141">Java</span><span class="sxs-lookup"><span data-stu-id="b941f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printershare-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b941f-142">响应</span><span class="sxs-lookup"><span data-stu-id="b941f-142">Response</span></span>
<span data-ttu-id="b941f-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b941f-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printerShare)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/shares",
      "id": "d837c17b-3296-4384-a053-828d56e10f50",
      "displayName": "PrinterShare Name",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "isAcceptingJobs": true,
      "allowAllUsers": false,
      "status": {
        "state": "stopped",
        "details": [
          "disconnected"
        ],
        "description": ""
      },
      "defaults": {
        "copiesPerJob": 1,
        "finishings": [
          "none"
        ],
        "mediaColor": "Unknown",
        "mediaType": "stationery",
        "mediaSize": "North America Letter",
        "pagesPerSheet": 1,
        "orientation": "portrait",
        "outputBin": "auto",
        "inputBin": "auto",
        "contentType": "application/oxps",
        "fitPdfToPage": false,
        "multipageLayout": null,
        "colorMode": "color",
        "quality": "medium",
        "duplexMode": "oneSided",
        "dpi": 600,
        "scaling": null
      },
      "location": {
        "latitude": 47.6450,
        "longitude": -122.1409,
        "altitudeInMeters": 3,
        "streetAddress": "One Microsoft Way",
        "subUnit": [
          "Main Plaza",
          "Unit 400"
        ],
        "city": "Redmond",
        "postalCode": "98052",
        "countryOrRegion": "USA",
        "site": "Puget Sound",
        "building": "Studio E",
        "floor": "1",
        "floorDescription": "First Floor",
        "roomName": "1234",
        "roomDescription": "First floor copy room",
        "organization": [
          "C+AI",
          "Microsoft Graph"
        ],
        "subdivision": [
          "King County",
          "Red West"
        ],
        "stateOrProvince": "Washington"
      }
    }
  ]
}
```

