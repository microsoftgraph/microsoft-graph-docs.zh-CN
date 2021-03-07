---
title: 获取 printerShare
description: 检索打印机共享的属性和关系。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3e5bc385fb6e928ba82bb36660bb8af7bf794034
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517288"
---
# <a name="get-printershare"></a><span data-ttu-id="876d4-103">获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="876d4-103">Get printerShare</span></span>
<span data-ttu-id="876d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="876d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="876d4-105">检索打印机共享的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="876d4-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="876d4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="876d4-106">Permissions</span></span>
<span data-ttu-id="876d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="876d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="876d4-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="876d4-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="876d4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="876d4-110">Permission type</span></span> | <span data-ttu-id="876d4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="876d4-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="876d4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="876d4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="876d4-113">PrinterShare.ReadBasic.All、PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="876d4-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="876d4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="876d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="876d4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="876d4-115">Not Supported.</span></span>|
|<span data-ttu-id="876d4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="876d4-116">Application</span></span>|<span data-ttu-id="876d4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="876d4-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="876d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="876d4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="876d4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="876d4-119">Optional query parameters</span></span>
<span data-ttu-id="876d4-120">此方法支持一些 OData 查询参数，包括 `$select` 和， `$expand` 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="876d4-120">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="876d4-121">例如：</span><span class="sxs-lookup"><span data-stu-id="876d4-121">For example:</span></span> 

<span data-ttu-id="876d4-122">例如</span><span class="sxs-lookup"><span data-stu-id="876d4-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="876d4-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="876d4-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="876d4-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="876d4-124">Exceptions</span></span>
* <span data-ttu-id="876d4-125">不支持 `$count` 运算符。</span><span class="sxs-lookup"><span data-stu-id="876d4-125">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="876d4-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="876d4-126">Request headers</span></span>
|<span data-ttu-id="876d4-127">名称</span><span class="sxs-lookup"><span data-stu-id="876d4-127">Name</span></span>|<span data-ttu-id="876d4-128">说明</span><span class="sxs-lookup"><span data-stu-id="876d4-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="876d4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="876d4-129">Authorization</span></span>|<span data-ttu-id="876d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="876d4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="876d4-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="876d4-132">Request body</span></span>
<span data-ttu-id="876d4-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="876d4-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="876d4-134">响应</span><span class="sxs-lookup"><span data-stu-id="876d4-134">Response</span></span>
<span data-ttu-id="876d4-135">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="876d4-135">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="876d4-136">默认情况下，响应将不包含[printerCapabilities。](../resources/printerCapabilities.md)</span><span class="sxs-lookup"><span data-stu-id="876d4-136">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="876d4-137">若要获取 **printerCapabilities，** 请使用 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="876d4-137">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="response"></a><span data-ttu-id="876d4-138">响应</span><span class="sxs-lookup"><span data-stu-id="876d4-138">Response</span></span>

<span data-ttu-id="876d4-139">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="876d4-139">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="876d4-140">示例</span><span class="sxs-lookup"><span data-stu-id="876d4-140">Examples</span></span>

### <a name="example-1-get-a-printershare"></a><span data-ttu-id="876d4-141">示例 1：获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="876d4-141">Example 1: Get a printerShare</span></span>

#### <a name="request"></a><span data-ttu-id="876d4-142">请求</span><span class="sxs-lookup"><span data-stu-id="876d4-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```

#### <a name="response"></a><span data-ttu-id="876d4-143">响应</span><span class="sxs-lookup"><span data-stu-id="876d4-143">Response</span></span>
<span data-ttu-id="876d4-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="876d4-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-a-printershare-and-its-capabilities"></a><span data-ttu-id="876d4-145">示例 2：获取 printerShare 及其功能</span><span class="sxs-lookup"><span data-stu-id="876d4-145">Example 2: Get a printerShare and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="876d4-146">请求</span><span class="sxs-lookup"><span data-stu-id="876d4-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}?$select=id,displayName,capabilities
```

#### <a name="response"></a><span data-ttu-id="876d4-147">响应</span><span class="sxs-lookup"><span data-stu-id="876d4-147">Response</span></span>

<span data-ttu-id="876d4-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="876d4-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
