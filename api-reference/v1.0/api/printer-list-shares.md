---
title: 列出打印机的 printerShares
description: 检索与打印机关联的 printerShares 列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7e03ae03b239bc7a538f8d488b8b244952b40bf3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517220"
---
# <a name="list-printershares-for-a-printer"></a><span data-ttu-id="3cdb5-103">列出打印机的 printerShares</span><span class="sxs-lookup"><span data-stu-id="3cdb5-103">List printerShares for a printer</span></span>
<span data-ttu-id="3cdb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cdb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3cdb5-105">检索与打印机关联的打印机共享 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-105">Retrieve a list of printer shares associated with the [printer](../resources/printer.md).</span></span>
><span data-ttu-id="3cdb5-106">**注意：** 目前，每个 **打印机** 仅支持一个打印机共享。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-106">**Note:** Currently, only **one** printer share per printer is supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cdb5-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3cdb5-107">Permissions</span></span>
<span data-ttu-id="3cdb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3cdb5-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="3cdb5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cdb5-111">Permission type</span></span> | <span data-ttu-id="3cdb5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cdb5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3cdb5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cdb5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3cdb5-114">PrinterShare.ReadBasic.All、PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cdb5-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="3cdb5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cdb5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cdb5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-116">Not Supported.</span></span>|
|<span data-ttu-id="3cdb5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cdb5-117">Application</span></span>| <span data-ttu-id="3cdb5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cdb5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cdb5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cdb5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cdb5-120">Optional query parameters</span></span>
<span data-ttu-id="3cdb5-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3cdb5-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cdb5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cdb5-123">Request headers</span></span>
|<span data-ttu-id="3cdb5-124">名称</span><span class="sxs-lookup"><span data-stu-id="3cdb5-124">Name</span></span>|<span data-ttu-id="3cdb5-125">说明</span><span class="sxs-lookup"><span data-stu-id="3cdb5-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cdb5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cdb5-126">Authorization</span></span>|<span data-ttu-id="3cdb5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cdb5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cdb5-129">Request body</span></span>
<span data-ttu-id="3cdb5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cdb5-131">响应</span><span class="sxs-lookup"><span data-stu-id="3cdb5-131">Response</span></span>

<span data-ttu-id="3cdb5-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printerShare](../resources/printershare.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-132">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="3cdb5-133">**注意**：响应将不包含 **默认值\*\*\*\*和功能** 属性。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-133">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="3cdb5-134">可以使用 Get [printerShare](printerShare-get.md) 请求查询这些属性。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-134">These properties can be queried using a [Get printerShare](printerShare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="3cdb5-135">示例</span><span class="sxs-lookup"><span data-stu-id="3cdb5-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cdb5-136">请求</span><span class="sxs-lookup"><span data-stu-id="3cdb5-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/shares
```


### <a name="response"></a><span data-ttu-id="3cdb5-137">响应</span><span class="sxs-lookup"><span data-stu-id="3cdb5-137">Response</span></span>
<span data-ttu-id="3cdb5-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cdb5-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

