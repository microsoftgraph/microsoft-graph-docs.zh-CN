---
title: 获取打印机
description: 检索打印机对象的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c98ecee9c0dfa075831c0df5cee9142540b58e1a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674440"
---
# <a name="get-printer"></a><span data-ttu-id="59f73-103">获取打印机</span><span class="sxs-lookup"><span data-stu-id="59f73-103">Get printer</span></span>

<span data-ttu-id="59f73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59f73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59f73-105">检索 [打印机](../resources/printer.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59f73-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59f73-106">权限</span><span class="sxs-lookup"><span data-stu-id="59f73-106">Permissions</span></span>
<span data-ttu-id="59f73-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="59f73-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="59f73-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="59f73-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="59f73-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="59f73-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="59f73-111">Permission type</span></span> | <span data-ttu-id="59f73-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59f73-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="59f73-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59f73-113">Delegated (work or school account)</span></span>| <span data-ttu-id="59f73-114">Printer。 all，完全控制，All，All</span><span class="sxs-lookup"><span data-stu-id="59f73-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="59f73-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59f73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59f73-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59f73-116">Not Supported.</span></span>|
|<span data-ttu-id="59f73-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59f73-117">Application</span></span>| <span data-ttu-id="59f73-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="59f73-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59f73-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59f73-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59f73-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59f73-120">Optional query parameters</span></span>
<span data-ttu-id="59f73-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59f73-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="59f73-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="59f73-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="59f73-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="59f73-123">Request headers</span></span>
| <span data-ttu-id="59f73-124">名称</span><span class="sxs-lookup"><span data-stu-id="59f73-124">Name</span></span>      |<span data-ttu-id="59f73-125">说明</span><span class="sxs-lookup"><span data-stu-id="59f73-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59f73-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="59f73-126">Authorization</span></span> | <span data-ttu-id="59f73-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59f73-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59f73-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="59f73-129">Request body</span></span>
<span data-ttu-id="59f73-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59f73-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="59f73-131">响应</span><span class="sxs-lookup"><span data-stu-id="59f73-131">Response</span></span>
<span data-ttu-id="59f73-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printer](../resources/printer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59f73-132">If successful, this method returns a `200 OK` response code and [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59f73-133">示例</span><span class="sxs-lookup"><span data-stu-id="59f73-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59f73-134">请求</span><span class="sxs-lookup"><span data-stu-id="59f73-134">Request</span></span>
<span data-ttu-id="59f73-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59f73-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59f73-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="59f73-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="59f73-137">C#</span><span class="sxs-lookup"><span data-stu-id="59f73-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59f73-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59f73-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59f73-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59f73-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59f73-140">响应</span><span class="sxs-lookup"><span data-stu-id="59f73-140">Response</span></span>
<span data-ttu-id="59f73-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="59f73-141">The following is an example of the response.</span></span>
><span data-ttu-id="59f73-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="59f73-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
