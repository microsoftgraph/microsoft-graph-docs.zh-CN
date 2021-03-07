---
title: 获取 printConnector
description: 检索连接器对象的属性和关系。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0d04dd07b5e3e6afa80f9104a223feb409b0e63b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516971"
---
# <a name="get-printconnector"></a><span data-ttu-id="2a483-103">获取 printConnector</span><span class="sxs-lookup"><span data-stu-id="2a483-103">Get printConnector</span></span>
<span data-ttu-id="2a483-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2a483-105">检索 **printConnector 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="2a483-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a483-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2a483-106">Permissions</span></span>
<span data-ttu-id="2a483-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2a483-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="2a483-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2a483-110">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="2a483-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2a483-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a483-111">Permission type</span></span> | <span data-ttu-id="2a483-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a483-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2a483-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a483-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2a483-114">PrintConnector.Read.All、PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a483-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="2a483-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a483-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a483-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a483-116">Not Supported.</span></span>|
|<span data-ttu-id="2a483-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a483-117">Application</span></span>|<span data-ttu-id="2a483-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a483-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a483-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a483-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors/{printConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a483-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2a483-120">Optional query parameters</span></span>
<span data-ttu-id="2a483-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2a483-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2a483-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2a483-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a483-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a483-123">Request headers</span></span>
|<span data-ttu-id="2a483-124">名称</span><span class="sxs-lookup"><span data-stu-id="2a483-124">Name</span></span>|<span data-ttu-id="2a483-125">说明</span><span class="sxs-lookup"><span data-stu-id="2a483-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a483-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a483-126">Authorization</span></span>|<span data-ttu-id="2a483-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a483-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a483-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a483-129">Request body</span></span>
<span data-ttu-id="2a483-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a483-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a483-131">响应</span><span class="sxs-lookup"><span data-stu-id="2a483-131">Response</span></span>

<span data-ttu-id="2a483-132">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [printConnector](../resources/printconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a483-132">If successful, this method returns a `200 OK` response code and a [printConnector](../resources/printconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a483-133">示例</span><span class="sxs-lookup"><span data-stu-id="2a483-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a483-134">请求</span><span class="sxs-lookup"><span data-stu-id="2a483-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```


### <a name="response"></a><span data-ttu-id="2a483-135">响应</span><span class="sxs-lookup"><span data-stu-id="2a483-135">Response</span></span>
<span data-ttu-id="2a483-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2a483-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors/$entity",
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
```

