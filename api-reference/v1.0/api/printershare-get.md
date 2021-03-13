---
title: 获取 printerShare
description: 检索打印机共享的属性和关系。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e9a16d9d615b780d921ff49291d6b15edda2ed3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771608"
---
# <a name="get-printershare"></a><span data-ttu-id="e2f5f-103">获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="e2f5f-103">Get printerShare</span></span>
<span data-ttu-id="e2f5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2f5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e2f5f-105">检索打印机共享的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2f5f-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2f5f-106">Permissions</span></span>
<span data-ttu-id="e2f5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e2f5f-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e2f5f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2f5f-110">Permission type</span></span> | <span data-ttu-id="e2f5f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2f5f-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e2f5f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2f5f-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e2f5f-113">PrinterShare.ReadBasic.All、PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f5f-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="e2f5f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2f5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2f5f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-115">Not Supported.</span></span>|
|<span data-ttu-id="e2f5f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2f5f-116">Application</span></span>|<span data-ttu-id="e2f5f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2f5f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2f5f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2f5f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2f5f-119">Optional query parameters</span></span>
<span data-ttu-id="e2f5f-120">此方法支持一些 OData 查询参数（包括 和 ） `$select` `$expand` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-120">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="e2f5f-121">例如：</span><span class="sxs-lookup"><span data-stu-id="e2f5f-121">For example:</span></span> 

<span data-ttu-id="e2f5f-122">例如</span><span class="sxs-lookup"><span data-stu-id="e2f5f-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="e2f5f-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="e2f5f-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e2f5f-124">Exceptions</span></span>
* <span data-ttu-id="e2f5f-125">`$count`运算符不受支持。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-125">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2f5f-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2f5f-126">Request headers</span></span>
|<span data-ttu-id="e2f5f-127">名称</span><span class="sxs-lookup"><span data-stu-id="e2f5f-127">Name</span></span>|<span data-ttu-id="e2f5f-128">说明</span><span class="sxs-lookup"><span data-stu-id="e2f5f-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e2f5f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2f5f-129">Authorization</span></span>|<span data-ttu-id="e2f5f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2f5f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2f5f-132">Request body</span></span>
<span data-ttu-id="e2f5f-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e2f5f-134">响应</span><span class="sxs-lookup"><span data-stu-id="e2f5f-134">Response</span></span>
<span data-ttu-id="e2f5f-135">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-135">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="e2f5f-136">默认情况下，该响应将不包含 [printerCapabilities](../resources/printerCapabilities.md)。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-136">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="e2f5f-137">若要获取 **printerCapabilities，** 请使用 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-137">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="response"></a><span data-ttu-id="e2f5f-138">响应</span><span class="sxs-lookup"><span data-stu-id="e2f5f-138">Response</span></span>

<span data-ttu-id="e2f5f-139">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-139">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2f5f-140">示例</span><span class="sxs-lookup"><span data-stu-id="e2f5f-140">Examples</span></span>

### <a name="example-1-get-a-printershare"></a><span data-ttu-id="e2f5f-141">示例 1：获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="e2f5f-141">Example 1: Get a printerShare</span></span>

#### <a name="request"></a><span data-ttu-id="e2f5f-142">请求</span><span class="sxs-lookup"><span data-stu-id="e2f5f-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e2f5f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2f5f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```
# <a name="c"></a>[<span data-ttu-id="e2f5f-144">C#</span><span class="sxs-lookup"><span data-stu-id="e2f5f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2f5f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2f5f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2f5f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2f5f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2f5f-147">Java</span><span class="sxs-lookup"><span data-stu-id="e2f5f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e2f5f-148">响应</span><span class="sxs-lookup"><span data-stu-id="e2f5f-148">Response</span></span>
<span data-ttu-id="e2f5f-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
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
```

### <a name="example-2-get-a-printershare-and-its-capabilities"></a><span data-ttu-id="e2f5f-150">示例 2：获取 printerShare 及其功能</span><span class="sxs-lookup"><span data-stu-id="e2f5f-150">Example 2: Get a printerShare and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="e2f5f-151">请求</span><span class="sxs-lookup"><span data-stu-id="e2f5f-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e2f5f-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2f5f-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}?$select=id,displayName,capabilities
```
# <a name="c"></a>[<span data-ttu-id="e2f5f-153">C#</span><span class="sxs-lookup"><span data-stu-id="e2f5f-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-capabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2f5f-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2f5f-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-capabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2f5f-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2f5f-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-capabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2f5f-156">Java</span><span class="sxs-lookup"><span data-stu-id="e2f5f-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-capabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e2f5f-157">响应</span><span class="sxs-lookup"><span data-stu-id="e2f5f-157">Response</span></span>

<span data-ttu-id="e2f5f-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2f5f-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
--> 
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "PrinterShare Name",
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
