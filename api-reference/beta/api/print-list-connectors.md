---
title: 获取连接器
description: 检索连接器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b71230de9c0b4c64eff35bf699a0168d355594ac
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895962"
---
# <a name="list-connectors"></a><span data-ttu-id="c465c-103">列出连接器</span><span class="sxs-lookup"><span data-stu-id="c465c-103">List connectors</span></span>

<span data-ttu-id="c465c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c465c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c465c-105">检索连接器列表。</span><span class="sxs-lookup"><span data-stu-id="c465c-105">Retrieve a list of connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="c465c-106">权限</span><span class="sxs-lookup"><span data-stu-id="c465c-106">Permissions</span></span>
<span data-ttu-id="c465c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c465c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c465c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c465c-109">Permission type</span></span> | <span data-ttu-id="c465c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c465c-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c465c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c465c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c465c-112">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="c465c-112">Users.Read.All</span></span> |
|<span data-ttu-id="c465c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c465c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c465c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c465c-114">Not Supported.</span></span>|
|<span data-ttu-id="c465c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c465c-115">Application</span></span>|<span data-ttu-id="c465c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c465c-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c465c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c465c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c465c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c465c-118">Optional query parameters</span></span>
<span data-ttu-id="c465c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c465c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c465c-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c465c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="c465c-121">异常</span><span class="sxs-lookup"><span data-stu-id="c465c-121">Exceptions</span></span>
* <span data-ttu-id="c465c-122">`$count`和`$filter`运算符不受支持。</span><span class="sxs-lookup"><span data-stu-id="c465c-122">The `$count` and `$filter` operators are not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c465c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c465c-123">Request headers</span></span>
| <span data-ttu-id="c465c-124">名称</span><span class="sxs-lookup"><span data-stu-id="c465c-124">Name</span></span>      |<span data-ttu-id="c465c-125">说明</span><span class="sxs-lookup"><span data-stu-id="c465c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c465c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c465c-126">Authorization</span></span> | <span data-ttu-id="c465c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c465c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c465c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c465c-129">Request body</span></span>
<span data-ttu-id="c465c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c465c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c465c-131">响应</span><span class="sxs-lookup"><span data-stu-id="c465c-131">Response</span></span>
<span data-ttu-id="c465c-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[连接器](../resources/printconnector.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c465c-132">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c465c-133">示例</span><span class="sxs-lookup"><span data-stu-id="c465c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c465c-134">请求</span><span class="sxs-lookup"><span data-stu-id="c465c-134">Request</span></span>
<span data-ttu-id="c465c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c465c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/beta/print/connectors
```
##### <a name="response"></a><span data-ttu-id="c465c-136">响应</span><span class="sxs-lookup"><span data-stu-id="c465c-136">Response</span></span>
<span data-ttu-id="c465c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c465c-137">The following is an example of the response.</span></span>
><span data-ttu-id="c465c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c465c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors",
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
      "registeredBy": {},
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