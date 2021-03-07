---
title: 列出 printConnectors
description: 检索连接器列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3c6c7f8507599cb22eb0e37bc95860d10a5e3c9f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516974"
---
# <a name="list-printconnectors"></a><span data-ttu-id="eb7bc-103">列出 printConnectors</span><span class="sxs-lookup"><span data-stu-id="eb7bc-103">List printConnectors</span></span>
<span data-ttu-id="eb7bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb7bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="eb7bc-105">检索打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb7bc-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eb7bc-106">Permissions</span></span>
<span data-ttu-id="eb7bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eb7bc-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="eb7bc-110">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="eb7bc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb7bc-111">Permission type</span></span> | <span data-ttu-id="eb7bc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb7bc-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eb7bc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb7bc-113">Delegated (work or school account)</span></span>| <span data-ttu-id="eb7bc-114">PrintConnector.Read.All、PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb7bc-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="eb7bc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb7bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb7bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-116">Not Supported.</span></span>|
|<span data-ttu-id="eb7bc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb7bc-117">Application</span></span>| <span data-ttu-id="eb7bc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb7bc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb7bc-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb7bc-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb7bc-120">Optional query parameters</span></span>
<span data-ttu-id="eb7bc-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb7bc-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="eb7bc-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="eb7bc-123">Exceptions</span></span>
<span data-ttu-id="eb7bc-124">不支持某些运算符：、 `$count` `$search` 、 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb7bc-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb7bc-125">Request headers</span></span>
| <span data-ttu-id="eb7bc-126">名称</span><span class="sxs-lookup"><span data-stu-id="eb7bc-126">Name</span></span>      |<span data-ttu-id="eb7bc-127">说明</span><span class="sxs-lookup"><span data-stu-id="eb7bc-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb7bc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb7bc-128">Authorization</span></span> | <span data-ttu-id="eb7bc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb7bc-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb7bc-131">Request body</span></span>
<span data-ttu-id="eb7bc-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb7bc-133">响应</span><span class="sxs-lookup"><span data-stu-id="eb7bc-133">Response</span></span>

<span data-ttu-id="eb7bc-134">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printConnector](../resources/printconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-134">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb7bc-135">示例</span><span class="sxs-lookup"><span data-stu-id="eb7bc-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb7bc-136">请求</span><span class="sxs-lookup"><span data-stu-id="eb7bc-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors
```

### <a name="response"></a><span data-ttu-id="eb7bc-137">响应</span><span class="sxs-lookup"><span data-stu-id="eb7bc-137">Response</span></span>
<span data-ttu-id="eb7bc-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb7bc-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

