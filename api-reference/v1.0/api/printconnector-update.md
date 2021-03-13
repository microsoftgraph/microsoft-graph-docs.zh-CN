---
title: 更新 printConnector
description: 更新 printConnector 对象的属性。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 97d92185d5035e0617028336e0adece1c39232de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776961"
---
# <a name="update-printconnector"></a><span data-ttu-id="69227-103">更新 printConnector</span><span class="sxs-lookup"><span data-stu-id="69227-103">Update printConnector</span></span>
<span data-ttu-id="69227-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69227-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="69227-105">更新 **printConnector 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="69227-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69227-106">权限</span><span class="sxs-lookup"><span data-stu-id="69227-106">Permissions</span></span>
<span data-ttu-id="69227-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69227-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="69227-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="69227-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="69227-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="69227-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="69227-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69227-111">Permission type</span></span> | <span data-ttu-id="69227-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69227-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="69227-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69227-113">Delegated (work or school account)</span></span>| <span data-ttu-id="69227-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69227-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="69227-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69227-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69227-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69227-116">Not Supported.</span></span>|
|<span data-ttu-id="69227-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69227-117">Application</span></span>|<span data-ttu-id="69227-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69227-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69227-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69227-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="69227-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69227-120">Request headers</span></span>
|<span data-ttu-id="69227-121">名称</span><span class="sxs-lookup"><span data-stu-id="69227-121">Name</span></span>|<span data-ttu-id="69227-122">说明</span><span class="sxs-lookup"><span data-stu-id="69227-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69227-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69227-123">Authorization</span></span>|<span data-ttu-id="69227-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69227-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69227-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69227-126">Content-Type</span></span>|<span data-ttu-id="69227-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="69227-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69227-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="69227-129">Request body</span></span>
<span data-ttu-id="69227-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="69227-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="69227-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="69227-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="69227-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="69227-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="69227-133">响应</span><span class="sxs-lookup"><span data-stu-id="69227-133">Response</span></span>
<span data-ttu-id="69227-134">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [printConnector](../resources/printConnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69227-134">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69227-135">示例</span><span class="sxs-lookup"><span data-stu-id="69227-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69227-136">请求</span><span class="sxs-lookup"><span data-stu-id="69227-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="69227-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="69227-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printconnector"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
Content-Type: application/json
Content-length: 308

{
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[<span data-ttu-id="69227-138">C#</span><span class="sxs-lookup"><span data-stu-id="69227-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69227-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69227-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69227-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69227-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69227-141">Java</span><span class="sxs-lookup"><span data-stu-id="69227-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="69227-142">响应</span><span class="sxs-lookup"><span data-stu-id="69227-142">Response</span></span>
<span data-ttu-id="69227-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="69227-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

