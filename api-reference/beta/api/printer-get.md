---
title: 获取打印机
description: 检索打印机对象的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 800dd2748cdd2a3866973670394f65f80f28a424
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895697"
---
# <a name="get-printer"></a><span data-ttu-id="14c6f-103">获取打印机</span><span class="sxs-lookup"><span data-stu-id="14c6f-103">Get printer</span></span>

<span data-ttu-id="14c6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14c6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14c6f-105">检索[打印机](../resources/printer.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14c6f-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14c6f-106">权限</span><span class="sxs-lookup"><span data-stu-id="14c6f-106">Permissions</span></span>
<span data-ttu-id="14c6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14c6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="14c6f-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="14c6f-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="14c6f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14c6f-110">Permission type</span></span> | <span data-ttu-id="14c6f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14c6f-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="14c6f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14c6f-112">Delegated (work or school account)</span></span>| <span data-ttu-id="14c6f-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="14c6f-113">Users.Read.All</span></span> |
|<span data-ttu-id="14c6f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14c6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14c6f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c6f-115">Not Supported.</span></span>|
|<span data-ttu-id="14c6f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14c6f-116">Application</span></span>|<span data-ttu-id="14c6f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c6f-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14c6f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14c6f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/printerShares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14c6f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14c6f-119">Optional query parameters</span></span>
<span data-ttu-id="14c6f-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="14c6f-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="14c6f-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="14c6f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14c6f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="14c6f-122">Request headers</span></span>
| <span data-ttu-id="14c6f-123">名称</span><span class="sxs-lookup"><span data-stu-id="14c6f-123">Name</span></span>      |<span data-ttu-id="14c6f-124">说明</span><span class="sxs-lookup"><span data-stu-id="14c6f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14c6f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14c6f-125">Authorization</span></span> | <span data-ttu-id="14c6f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14c6f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14c6f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="14c6f-128">Request body</span></span>
<span data-ttu-id="14c6f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14c6f-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="14c6f-130">响应</span><span class="sxs-lookup"><span data-stu-id="14c6f-130">Response</span></span>
<span data-ttu-id="14c6f-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printer](../resources/printer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14c6f-131">If successful, this method returns a `200 OK` response code and [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14c6f-132">示例</span><span class="sxs-lookup"><span data-stu-id="14c6f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14c6f-133">请求</span><span class="sxs-lookup"><span data-stu-id="14c6f-133">Request</span></span>
<span data-ttu-id="14c6f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14c6f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/{id}
```
##### <a name="response"></a><span data-ttu-id="14c6f-135">响应</span><span class="sxs-lookup"><span data-stu-id="14c6f-135">Response</span></span>
<span data-ttu-id="14c6f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14c6f-136">The following is an example of the response.</span></span>
><span data-ttu-id="14c6f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14c6f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "registeredBy": {},
  "status": {
    "processingState": "stopped",
    "processingStateReasons": ["disconnected"],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
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
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->