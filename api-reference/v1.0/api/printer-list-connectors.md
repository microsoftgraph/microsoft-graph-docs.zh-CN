---
title: 列出打印机的 printConnectors
description: 检索与打印机关联的连接器列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: b1b1acb6a0f998d272d04eef43e94a3ddfd92016
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956321"
---
# <a name="list-printconnectors-for-a-printer"></a><span data-ttu-id="c71d3-103">列出打印机的 printConnectors</span><span class="sxs-lookup"><span data-stu-id="c71d3-103">List printConnectors for a printer</span></span>
<span data-ttu-id="c71d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c71d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c71d3-105">检索与 [打印机关联的 printConnectors](../resources/printconnector.md) [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="c71d3-105">Retrieve a list of [printConnectors](../resources/printconnector.md) associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c71d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="c71d3-106">Permissions</span></span>
<span data-ttu-id="c71d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c71d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c71d3-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="c71d3-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="c71d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c71d3-110">Permission type</span></span> | <span data-ttu-id="c71d3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c71d3-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c71d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c71d3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c71d3-113">PrintConnector.Read.All、PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c71d3-113">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="c71d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c71d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c71d3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c71d3-115">Not Supported.</span></span>|
|<span data-ttu-id="c71d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c71d3-116">Application</span></span>| <span data-ttu-id="c71d3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c71d3-117">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c71d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c71d3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c71d3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c71d3-119">Optional query parameters</span></span>
<span data-ttu-id="c71d3-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c71d3-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c71d3-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c71d3-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c71d3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c71d3-122">Request headers</span></span>
|<span data-ttu-id="c71d3-123">名称</span><span class="sxs-lookup"><span data-stu-id="c71d3-123">Name</span></span>|<span data-ttu-id="c71d3-124">说明</span><span class="sxs-lookup"><span data-stu-id="c71d3-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c71d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c71d3-125">Authorization</span></span>|<span data-ttu-id="c71d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c71d3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c71d3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c71d3-128">Request body</span></span>
<span data-ttu-id="c71d3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c71d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c71d3-130">响应</span><span class="sxs-lookup"><span data-stu-id="c71d3-130">Response</span></span>

<span data-ttu-id="c71d3-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printConnector](../resources/printconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c71d3-131">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c71d3-132">示例</span><span class="sxs-lookup"><span data-stu-id="c71d3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c71d3-133">请求</span><span class="sxs-lookup"><span data-stu-id="c71d3-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c71d3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c71d3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printconnector_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/connectors
```
# <a name="c"></a>[<span data-ttu-id="c71d3-135">C#</span><span class="sxs-lookup"><span data-stu-id="c71d3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printconnector-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c71d3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c71d3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printconnector-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c71d3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c71d3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printconnector-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c71d3-138">Java</span><span class="sxs-lookup"><span data-stu-id="c71d3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printconnector-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c71d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="c71d3-139">Response</span></span>
<span data-ttu-id="c71d3-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c71d3-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printConnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
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

