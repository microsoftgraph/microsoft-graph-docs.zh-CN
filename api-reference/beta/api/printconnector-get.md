---
title: 获取 printConnector
description: 检索连接器对象的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d6fef9ad3a7e5166f13fce08ac3bf77b3c8a1336
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848792"
---
# <a name="get-printconnector"></a><span data-ttu-id="21c67-103">获取 printConnector</span><span class="sxs-lookup"><span data-stu-id="21c67-103">Get printConnector</span></span>

<span data-ttu-id="21c67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21c67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21c67-105">检索 **printConnector** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21c67-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21c67-106">权限</span><span class="sxs-lookup"><span data-stu-id="21c67-106">Permissions</span></span>
<span data-ttu-id="21c67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21c67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="21c67-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="21c67-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="21c67-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="21c67-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="21c67-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="21c67-111">Permission type</span></span> | <span data-ttu-id="21c67-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21c67-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="21c67-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21c67-113">Delegated (work or school account)</span></span>| <span data-ttu-id="21c67-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="21c67-114">User.Read</span></span> |
|<span data-ttu-id="21c67-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21c67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21c67-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21c67-116">Not Supported.</span></span>|
|<span data-ttu-id="21c67-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="21c67-117">Application</span></span>|<span data-ttu-id="21c67-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="21c67-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21c67-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21c67-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21c67-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="21c67-120">Optional query parameters</span></span>
<span data-ttu-id="21c67-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="21c67-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="21c67-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="21c67-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="21c67-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="21c67-123">Request headers</span></span>
| <span data-ttu-id="21c67-124">名称</span><span class="sxs-lookup"><span data-stu-id="21c67-124">Name</span></span>      |<span data-ttu-id="21c67-125">说明</span><span class="sxs-lookup"><span data-stu-id="21c67-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21c67-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="21c67-126">Authorization</span></span> | <span data-ttu-id="21c67-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21c67-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21c67-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="21c67-129">Request body</span></span>
<span data-ttu-id="21c67-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21c67-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="21c67-131">响应</span><span class="sxs-lookup"><span data-stu-id="21c67-131">Response</span></span>
<span data-ttu-id="21c67-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printConnector](../resources/printconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21c67-132">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21c67-133">示例</span><span class="sxs-lookup"><span data-stu-id="21c67-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21c67-134">请求</span><span class="sxs-lookup"><span data-stu-id="21c67-134">Request</span></span>
<span data-ttu-id="21c67-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21c67-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21c67-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="21c67-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="21c67-137">C#</span><span class="sxs-lookup"><span data-stu-id="21c67-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21c67-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21c67-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21c67-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21c67-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="21c67-140">响应</span><span class="sxs-lookup"><span data-stu-id="21c67-140">Response</span></span>
<span data-ttu-id="21c67-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="21c67-141">The following is an example of the response.</span></span>
><span data-ttu-id="21c67-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="21c67-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "displayName": "ConnectorName",
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
