---
title: 列出 printConnectors
description: 检索连接器列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9ef3bb3f197f8c7f0122993c6ca8cb716ddce92b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948874"
---
# <a name="list-printconnectors"></a><span data-ttu-id="31485-103">列出 printConnectors</span><span class="sxs-lookup"><span data-stu-id="31485-103">List printConnectors</span></span>
<span data-ttu-id="31485-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31485-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="31485-105">检索打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="31485-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="31485-106">权限</span><span class="sxs-lookup"><span data-stu-id="31485-106">Permissions</span></span>
<span data-ttu-id="31485-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="31485-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="31485-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="31485-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="31485-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="31485-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="31485-111">Permission type</span></span> | <span data-ttu-id="31485-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31485-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="31485-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31485-113">Delegated (work or school account)</span></span>| <span data-ttu-id="31485-114">PrintConnector.Read.All、PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31485-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="31485-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31485-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31485-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31485-116">Not Supported.</span></span>|
|<span data-ttu-id="31485-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="31485-117">Application</span></span>| <span data-ttu-id="31485-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="31485-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31485-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31485-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31485-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31485-120">Optional query parameters</span></span>
<span data-ttu-id="31485-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31485-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="31485-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="31485-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="31485-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="31485-123">Exceptions</span></span>
<span data-ttu-id="31485-124">不支持某些运算符 `$count` `$search` ：、、。 `$filter`</span><span class="sxs-lookup"><span data-stu-id="31485-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31485-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="31485-125">Request headers</span></span>
| <span data-ttu-id="31485-126">名称</span><span class="sxs-lookup"><span data-stu-id="31485-126">Name</span></span>      |<span data-ttu-id="31485-127">说明</span><span class="sxs-lookup"><span data-stu-id="31485-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31485-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="31485-128">Authorization</span></span> | <span data-ttu-id="31485-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31485-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31485-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="31485-131">Request body</span></span>
<span data-ttu-id="31485-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31485-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31485-133">响应</span><span class="sxs-lookup"><span data-stu-id="31485-133">Response</span></span>

<span data-ttu-id="31485-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printConnector](../resources/printconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="31485-134">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31485-135">示例</span><span class="sxs-lookup"><span data-stu-id="31485-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31485-136">请求</span><span class="sxs-lookup"><span data-stu-id="31485-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="31485-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="31485-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printconnector_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="31485-138">C#</span><span class="sxs-lookup"><span data-stu-id="31485-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printconnector-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31485-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31485-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printconnector-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31485-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31485-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printconnector-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31485-141">Java</span><span class="sxs-lookup"><span data-stu-id="31485-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printconnector-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31485-142">响应</span><span class="sxs-lookup"><span data-stu-id="31485-142">Response</span></span>
<span data-ttu-id="31485-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="31485-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "Connector1",
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

