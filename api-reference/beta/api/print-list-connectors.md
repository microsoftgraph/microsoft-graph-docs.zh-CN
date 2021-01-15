---
title: 列出 printConnectors
description: 检索连接器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4fec305bc6239da0bc11a4ccdf61591bd32157c4
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874366"
---
# <a name="list-printconnectors"></a><span data-ttu-id="e2fd0-103">列出 printConnectors</span><span class="sxs-lookup"><span data-stu-id="e2fd0-103">List printConnectors</span></span>

<span data-ttu-id="e2fd0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2fd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2fd0-105">检索打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2fd0-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2fd0-106">Permissions</span></span>
<span data-ttu-id="e2fd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e2fd0-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e2fd0-110">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e2fd0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2fd0-111">Permission type</span></span> | <span data-ttu-id="e2fd0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2fd0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e2fd0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2fd0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e2fd0-114">PrintConnector.Read.All、PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2fd0-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="e2fd0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2fd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2fd0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-116">Not Supported.</span></span>|
|<span data-ttu-id="e2fd0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2fd0-117">Application</span></span>| <span data-ttu-id="e2fd0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2fd0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2fd0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2fd0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2fd0-120">Optional query parameters</span></span>
<span data-ttu-id="e2fd0-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e2fd0-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="e2fd0-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e2fd0-123">Exceptions</span></span>
<span data-ttu-id="e2fd0-124">不支持某些运算符：、 `$count` `$search` 、 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2fd0-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2fd0-125">Request headers</span></span>
| <span data-ttu-id="e2fd0-126">名称</span><span class="sxs-lookup"><span data-stu-id="e2fd0-126">Name</span></span>      |<span data-ttu-id="e2fd0-127">说明</span><span class="sxs-lookup"><span data-stu-id="e2fd0-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2fd0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2fd0-128">Authorization</span></span> | <span data-ttu-id="e2fd0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2fd0-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2fd0-131">Request body</span></span>
<span data-ttu-id="e2fd0-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e2fd0-133">响应</span><span class="sxs-lookup"><span data-stu-id="e2fd0-133">Response</span></span>
<span data-ttu-id="e2fd0-134">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 printConnector](../resources/printconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2fd0-135">示例</span><span class="sxs-lookup"><span data-stu-id="e2fd0-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2fd0-136">请求</span><span class="sxs-lookup"><span data-stu-id="e2fd0-136">Request</span></span>
<span data-ttu-id="e2fd0-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2fd0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2fd0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="e2fd0-139">C#</span><span class="sxs-lookup"><span data-stu-id="e2fd0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2fd0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2fd0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2fd0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2fd0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2fd0-142">Java</span><span class="sxs-lookup"><span data-stu-id="e2fd0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e2fd0-143">响应</span><span class="sxs-lookup"><span data-stu-id="e2fd0-143">Response</span></span>
<span data-ttu-id="e2fd0-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-144">The following is an example of the response.</span></span>
><span data-ttu-id="e2fd0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e2fd0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
