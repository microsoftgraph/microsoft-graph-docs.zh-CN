---
title: 获取 printConnector
description: 检索连接器对象的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dee62dd32f88ee85ba20b05604c30d6ac293ee15
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062131"
---
# <a name="get-printconnector"></a><span data-ttu-id="261f4-103">获取 printConnector</span><span class="sxs-lookup"><span data-stu-id="261f4-103">Get printConnector</span></span>

<span data-ttu-id="261f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="261f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="261f4-105">检索**printConnector**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="261f4-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="261f4-106">权限</span><span class="sxs-lookup"><span data-stu-id="261f4-106">Permissions</span></span>
<span data-ttu-id="261f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="261f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="261f4-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="261f4-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="261f4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="261f4-110">Permission type</span></span> | <span data-ttu-id="261f4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="261f4-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="261f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="261f4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="261f4-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="261f4-113">Users.Read.All</span></span> |
|<span data-ttu-id="261f4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="261f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="261f4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="261f4-115">Not Supported.</span></span>|
|<span data-ttu-id="261f4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="261f4-116">Application</span></span>|<span data-ttu-id="261f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="261f4-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="261f4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="261f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="261f4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="261f4-119">Optional query parameters</span></span>
<span data-ttu-id="261f4-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="261f4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="261f4-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="261f4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="261f4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="261f4-122">Request headers</span></span>
| <span data-ttu-id="261f4-123">名称</span><span class="sxs-lookup"><span data-stu-id="261f4-123">Name</span></span>      |<span data-ttu-id="261f4-124">说明</span><span class="sxs-lookup"><span data-stu-id="261f4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="261f4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="261f4-125">Authorization</span></span> | <span data-ttu-id="261f4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="261f4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="261f4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="261f4-128">Request body</span></span>
<span data-ttu-id="261f4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="261f4-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="261f4-130">响应</span><span class="sxs-lookup"><span data-stu-id="261f4-130">Response</span></span>
<span data-ttu-id="261f4-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printConnector](../resources/printconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="261f4-131">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="261f4-132">示例</span><span class="sxs-lookup"><span data-stu-id="261f4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="261f4-133">请求</span><span class="sxs-lookup"><span data-stu-id="261f4-133">Request</span></span>
<span data-ttu-id="261f4-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="261f4-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="261f4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="261f4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="261f4-136">C#</span><span class="sxs-lookup"><span data-stu-id="261f4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="261f4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="261f4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="261f4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="261f4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="261f4-139">响应</span><span class="sxs-lookup"><span data-stu-id="261f4-139">Response</span></span>
<span data-ttu-id="261f4-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="261f4-140">The following is an example of the response.</span></span>
><span data-ttu-id="261f4-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="261f4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1097

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "name": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
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
  "description": "Get printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
