---
title: 列出 printConnectors
description: 检索连接器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2ba08b47fca02c67c3d55762747b010bf4b77ad6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042995"
---
# <a name="list-printconnectors"></a><span data-ttu-id="9a890-103">列出 printConnectors</span><span class="sxs-lookup"><span data-stu-id="9a890-103">List printConnectors</span></span>

<span data-ttu-id="9a890-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a890-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a890-105">检索打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="9a890-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a890-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a890-106">Permissions</span></span>
<span data-ttu-id="9a890-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9a890-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="9a890-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="9a890-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="9a890-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="9a890-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a890-111">Permission type</span></span> | <span data-ttu-id="9a890-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a890-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9a890-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a890-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9a890-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="9a890-114">User.Read</span></span> |
|<span data-ttu-id="9a890-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a890-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a890-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a890-116">Not Supported.</span></span>|
|<span data-ttu-id="9a890-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a890-117">Application</span></span>| <span data-ttu-id="9a890-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a890-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a890-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a890-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a890-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a890-120">Optional query parameters</span></span>
<span data-ttu-id="9a890-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9a890-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9a890-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9a890-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="9a890-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="9a890-123">Exceptions</span></span>
<span data-ttu-id="9a890-124">某些运算符不受支持： `$count` 、 `$orderby` 、 `$search` 、 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="9a890-124">Some operators are not supported: `$count`, `$orderby`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a890-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a890-125">Request headers</span></span>
| <span data-ttu-id="9a890-126">名称</span><span class="sxs-lookup"><span data-stu-id="9a890-126">Name</span></span>      |<span data-ttu-id="9a890-127">说明</span><span class="sxs-lookup"><span data-stu-id="9a890-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a890-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a890-128">Authorization</span></span> | <span data-ttu-id="9a890-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a890-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a890-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a890-131">Request body</span></span>
<span data-ttu-id="9a890-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a890-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9a890-133">响应</span><span class="sxs-lookup"><span data-stu-id="9a890-133">Response</span></span>
<span data-ttu-id="9a890-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printConnector](../resources/printconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9a890-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a890-135">示例</span><span class="sxs-lookup"><span data-stu-id="9a890-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a890-136">请求</span><span class="sxs-lookup"><span data-stu-id="9a890-136">Request</span></span>
<span data-ttu-id="9a890-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a890-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a890-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a890-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="9a890-139">C#</span><span class="sxs-lookup"><span data-stu-id="9a890-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a890-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a890-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a890-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a890-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9a890-142">响应</span><span class="sxs-lookup"><span data-stu-id="9a890-142">Response</span></span>
<span data-ttu-id="9a890-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a890-143">The following is an example of the response.</span></span>
><span data-ttu-id="9a890-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9a890-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


