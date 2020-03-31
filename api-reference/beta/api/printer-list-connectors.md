---
title: 列出连接器
description: 检索与打印机关联的连接器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: eaf7b1a13b48a145a770cc94214846f69119b083
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062091"
---
# <a name="list-connectors"></a><span data-ttu-id="e210d-103">列出连接器</span><span class="sxs-lookup"><span data-stu-id="e210d-103">List connectors</span></span>

<span data-ttu-id="e210d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e210d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e210d-105">检索与[打印机](../resources/printer.md)关联的**连接器**列表。</span><span class="sxs-lookup"><span data-stu-id="e210d-105">Retrieve a list of **connectors** associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e210d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e210d-106">Permissions</span></span>
<span data-ttu-id="e210d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e210d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e210d-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e210d-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e210d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e210d-110">Permission type</span></span> | <span data-ttu-id="e210d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e210d-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e210d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e210d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e210d-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="e210d-113">Users.Read.All</span></span> |
|<span data-ttu-id="e210d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e210d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e210d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e210d-115">Not Supported.</span></span>|
|<span data-ttu-id="e210d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e210d-116">Application</span></span>|<span data-ttu-id="e210d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e210d-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e210d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e210d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/connectors
```

## <a name="request-headers"></a><span data-ttu-id="e210d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e210d-119">Request headers</span></span>
| <span data-ttu-id="e210d-120">名称</span><span class="sxs-lookup"><span data-stu-id="e210d-120">Name</span></span>      |<span data-ttu-id="e210d-121">说明</span><span class="sxs-lookup"><span data-stu-id="e210d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e210d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e210d-122">Authorization</span></span> | <span data-ttu-id="e210d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e210d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e210d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e210d-125">Request body</span></span>
<span data-ttu-id="e210d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e210d-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e210d-127">响应</span><span class="sxs-lookup"><span data-stu-id="e210d-127">Response</span></span>
<span data-ttu-id="e210d-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printConnector](../resources/printconnector.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e210d-128">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e210d-129">示例</span><span class="sxs-lookup"><span data-stu-id="e210d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e210d-130">请求</span><span class="sxs-lookup"><span data-stu-id="e210d-130">Request</span></span>
<span data-ttu-id="e210d-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e210d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e210d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e210d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/connectors
```
# <a name="c"></a>[<span data-ttu-id="e210d-133">C#</span><span class="sxs-lookup"><span data-stu-id="e210d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e210d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e210d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e210d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e210d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e210d-136">响应</span><span class="sxs-lookup"><span data-stu-id="e210d-136">Response</span></span>
<span data-ttu-id="e210d-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e210d-137">The following is an example of the response.</span></span>
><span data-ttu-id="e210d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e210d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1373

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printConnector)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
      "deviceHealth": {
        "lastConnectionTime": "2020-02-04T07:00:00.0000000"
      },
      "registeredDateTime": "2020-02-04T07:00:00.0000000",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
