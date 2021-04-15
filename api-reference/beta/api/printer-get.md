---
title: 获取打印机
description: 检索打印机对象的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 42804622f94207e304ada3a9538f860415ddbf53
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766250"
---
# <a name="get-printer"></a><span data-ttu-id="005ac-103">获取打印机</span><span class="sxs-lookup"><span data-stu-id="005ac-103">Get printer</span></span>

<span data-ttu-id="005ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="005ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="005ac-105">检索打印机对象 [的属性和](../resources/printer.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="005ac-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="005ac-106">权限</span><span class="sxs-lookup"><span data-stu-id="005ac-106">Permissions</span></span>
<span data-ttu-id="005ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="005ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="005ac-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="005ac-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="005ac-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="005ac-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="005ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="005ac-111">Permission type</span></span> | <span data-ttu-id="005ac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="005ac-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="005ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="005ac-113">Delegated (work or school account)</span></span>| <span data-ttu-id="005ac-114">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="005ac-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="005ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="005ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="005ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="005ac-116">Not Supported.</span></span>|
|<span data-ttu-id="005ac-117">Application</span><span class="sxs-lookup"><span data-stu-id="005ac-117">Application</span></span>| <span data-ttu-id="005ac-118">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="005ac-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="005ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="005ac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="005ac-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="005ac-120">Optional query parameters</span></span>
<span data-ttu-id="005ac-121">此方法支持一些 OData 查询参数，$select、$expand自定义响应。</span><span class="sxs-lookup"><span data-stu-id="005ac-121">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="005ac-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="005ac-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="005ac-123">例如</span><span class="sxs-lookup"><span data-stu-id="005ac-123">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
## <a name="request-headers"></a><span data-ttu-id="005ac-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="005ac-124">Request headers</span></span>
| <span data-ttu-id="005ac-125">名称</span><span class="sxs-lookup"><span data-stu-id="005ac-125">Name</span></span>      |<span data-ttu-id="005ac-126">说明</span><span class="sxs-lookup"><span data-stu-id="005ac-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="005ac-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="005ac-127">Authorization</span></span> | <span data-ttu-id="005ac-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="005ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="005ac-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="005ac-130">Request body</span></span>
<span data-ttu-id="005ac-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="005ac-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="005ac-132">响应</span><span class="sxs-lookup"><span data-stu-id="005ac-132">Response</span></span>
<span data-ttu-id="005ac-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printer](../resources/printer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="005ac-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="005ac-134">默认情况下，该响应将不包含 [printerCapabilities](../resources/printerCapabilities.md)。</span><span class="sxs-lookup"><span data-stu-id="005ac-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="005ac-135">若要获取 **printerCapabilities，** 请使用 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="005ac-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="005ac-136">示例</span><span class="sxs-lookup"><span data-stu-id="005ac-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="005ac-137">请求</span><span class="sxs-lookup"><span data-stu-id="005ac-137">Request</span></span>
<span data-ttu-id="005ac-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="005ac-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="005ac-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="005ac-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="005ac-140">C#</span><span class="sxs-lookup"><span data-stu-id="005ac-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="005ac-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="005ac-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="005ac-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="005ac-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="005ac-143">Java</span><span class="sxs-lookup"><span data-stu-id="005ac-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="005ac-144">响应</span><span class="sxs-lookup"><span data-stu-id="005ac-144">Response</span></span>
<span data-ttu-id="005ac-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="005ac-145">The following is an example of the response.</span></span>
><span data-ttu-id="005ac-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="005ac-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
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
    "latitude": 1.1,
    "longitude": 2.2,
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

<span data-ttu-id="005ac-148">下面是使用 $select=id，displayName，capabilities 时的响应示例</span><span class="sxs-lookup"><span data-stu-id="005ac-148">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="005ac-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="005ac-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
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
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
