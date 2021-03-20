---
title: 列出共享项
description: 检索打印机共享的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dfabbed35d669fcf539c33b8ec64f39622f4c476
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945067"
---
# <a name="list-shares"></a><span data-ttu-id="5f76b-103">列出共享项</span><span class="sxs-lookup"><span data-stu-id="5f76b-103">List shares</span></span>
<span data-ttu-id="5f76b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f76b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5f76b-105">检索 **printerShares 列表**。</span><span class="sxs-lookup"><span data-stu-id="5f76b-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f76b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5f76b-106">Permissions</span></span>
<span data-ttu-id="5f76b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f76b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5f76b-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="5f76b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="5f76b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f76b-110">Permission type</span></span> | <span data-ttu-id="5f76b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f76b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5f76b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f76b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5f76b-113">PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f76b-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="5f76b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f76b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f76b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f76b-115">Not Supported.</span></span>|
|<span data-ttu-id="5f76b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f76b-116">Application</span></span>|<span data-ttu-id="5f76b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f76b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f76b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f76b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f76b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f76b-119">Optional query parameters</span></span>
<span data-ttu-id="5f76b-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f76b-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f76b-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5f76b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="5f76b-122">若要查看每个打印机共享功能的列表，请包含可选的 `$select=capabilities` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="5f76b-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="5f76b-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="5f76b-123">Exceptions</span></span>
<span data-ttu-id="5f76b-124">不支持某些运算符 `$count` `$orderby` ：、、。 `$search`</span><span class="sxs-lookup"><span data-stu-id="5f76b-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f76b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f76b-125">Request headers</span></span>
|<span data-ttu-id="5f76b-126">名称</span><span class="sxs-lookup"><span data-stu-id="5f76b-126">Name</span></span>|<span data-ttu-id="5f76b-127">说明</span><span class="sxs-lookup"><span data-stu-id="5f76b-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f76b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f76b-128">Authorization</span></span>|<span data-ttu-id="5f76b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f76b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f76b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f76b-131">Request body</span></span>
<span data-ttu-id="5f76b-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f76b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f76b-133">响应</span><span class="sxs-lookup"><span data-stu-id="5f76b-133">Response</span></span>

<span data-ttu-id="5f76b-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printerShare](../resources/printershare.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f76b-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="5f76b-135">**注意**：该响应将不包含 **defaults** **和 capabilities** 属性。</span><span class="sxs-lookup"><span data-stu-id="5f76b-135">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="5f76b-136">可以通过获取 [printerShare](printershare-get.md) 请求获取这些属性。</span><span class="sxs-lookup"><span data-stu-id="5f76b-136">You can get these properties via a [Get printerShare](printershare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="5f76b-137">示例</span><span class="sxs-lookup"><span data-stu-id="5f76b-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f76b-138">请求</span><span class="sxs-lookup"><span data-stu-id="5f76b-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f76b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f76b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printershare_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares
```
# <a name="c"></a>[<span data-ttu-id="5f76b-140">C#</span><span class="sxs-lookup"><span data-stu-id="5f76b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printershare-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f76b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f76b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printershare-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f76b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f76b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printershare-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f76b-143">Java</span><span class="sxs-lookup"><span data-stu-id="5f76b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printershare-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5f76b-144">响应</span><span class="sxs-lookup"><span data-stu-id="5f76b-144">Response</span></span>
<span data-ttu-id="5f76b-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5f76b-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares",
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

