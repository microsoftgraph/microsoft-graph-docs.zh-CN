---
title: 列出打印机的 printConnectors
description: 检索与打印机关联的连接器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8b2b3bbff54d20de777c37e344190cee07ea4806
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766278"
---
# <a name="list-printconnectors-for-printer"></a><span data-ttu-id="46ee7-103">列出打印机的 printConnectors</span><span class="sxs-lookup"><span data-stu-id="46ee7-103">List printConnectors for printer</span></span>

<span data-ttu-id="46ee7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46ee7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46ee7-105">检索与 **打印机** 关联的连接器 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="46ee7-105">Retrieve a list of **connectors** associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="46ee7-106">权限</span><span class="sxs-lookup"><span data-stu-id="46ee7-106">Permissions</span></span>
<span data-ttu-id="46ee7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46ee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="46ee7-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="46ee7-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="46ee7-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="46ee7-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="46ee7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46ee7-111">Permission type</span></span> | <span data-ttu-id="46ee7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46ee7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="46ee7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46ee7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="46ee7-114">PrintConnector.Read.All、PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ee7-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="46ee7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46ee7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46ee7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46ee7-116">Not Supported.</span></span>|
|<span data-ttu-id="46ee7-117">Application</span><span class="sxs-lookup"><span data-stu-id="46ee7-117">Application</span></span>| <span data-ttu-id="46ee7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="46ee7-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46ee7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46ee7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46ee7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46ee7-120">Optional query parameters</span></span>
<span data-ttu-id="46ee7-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46ee7-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="46ee7-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="46ee7-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46ee7-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="46ee7-123">Request headers</span></span>
| <span data-ttu-id="46ee7-124">名称</span><span class="sxs-lookup"><span data-stu-id="46ee7-124">Name</span></span>      |<span data-ttu-id="46ee7-125">说明</span><span class="sxs-lookup"><span data-stu-id="46ee7-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46ee7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="46ee7-126">Authorization</span></span> | <span data-ttu-id="46ee7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46ee7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46ee7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="46ee7-129">Request body</span></span>
<span data-ttu-id="46ee7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46ee7-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="46ee7-131">响应</span><span class="sxs-lookup"><span data-stu-id="46ee7-131">Response</span></span>
<span data-ttu-id="46ee7-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printConnector](../resources/printconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46ee7-132">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46ee7-133">示例</span><span class="sxs-lookup"><span data-stu-id="46ee7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46ee7-134">请求</span><span class="sxs-lookup"><span data-stu-id="46ee7-134">Request</span></span>
<span data-ttu-id="46ee7-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="46ee7-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46ee7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="46ee7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/connectors
```
# <a name="c"></a>[<span data-ttu-id="46ee7-137">C#</span><span class="sxs-lookup"><span data-stu-id="46ee7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46ee7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46ee7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46ee7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46ee7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46ee7-140">Java</span><span class="sxs-lookup"><span data-stu-id="46ee7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="46ee7-141">响应</span><span class="sxs-lookup"><span data-stu-id="46ee7-141">Response</span></span>
<span data-ttu-id="46ee7-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="46ee7-142">The following is an example of the response.</span></span>
><span data-ttu-id="46ee7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="46ee7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
