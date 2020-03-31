---
title: 更新 printConnector
description: 更新 printConnector 对象的属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7b4a9a0b74969877ca1336facda8e63462919b6b
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062124"
---
# <a name="update-printconnector"></a><span data-ttu-id="8cc4b-103">更新 printConnector</span><span class="sxs-lookup"><span data-stu-id="8cc4b-103">Update printConnector</span></span>

<span data-ttu-id="8cc4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc4b-105">更新**printConnector**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc4b-106">权限</span><span class="sxs-lookup"><span data-stu-id="8cc4b-106">Permissions</span></span>
<span data-ttu-id="8cc4b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8cc4b-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8cc4b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cc4b-110">Permission type</span></span> | <span data-ttu-id="8cc4b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cc4b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8cc4b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cc4b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="8cc4b-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="8cc4b-113">Users.Read.All</span></span> |
|<span data-ttu-id="8cc4b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cc4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc4b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-115">Not Supported.</span></span>|
|<span data-ttu-id="8cc4b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cc4b-116">Application</span></span>|<span data-ttu-id="8cc4b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc4b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cc4b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8cc4b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cc4b-119">Request headers</span></span>
| <span data-ttu-id="8cc4b-120">名称</span><span class="sxs-lookup"><span data-stu-id="8cc4b-120">Name</span></span>       | <span data-ttu-id="8cc4b-121">说明</span><span class="sxs-lookup"><span data-stu-id="8cc4b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8cc4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc4b-122">Authorization</span></span> | <span data-ttu-id="8cc4b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cc4b-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="8cc4b-125">Content-type</span></span>  | <span data-ttu-id="8cc4b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8cc4b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc4b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cc4b-128">Request body</span></span>
<span data-ttu-id="8cc4b-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8cc4b-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8cc4b-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8cc4b-132">属性</span><span class="sxs-lookup"><span data-stu-id="8cc4b-132">Property</span></span>     | <span data-ttu-id="8cc4b-133">类型</span><span class="sxs-lookup"><span data-stu-id="8cc4b-133">Type</span></span>        | <span data-ttu-id="8cc4b-134">说明</span><span class="sxs-lookup"><span data-stu-id="8cc4b-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cc4b-135">name</span><span class="sxs-lookup"><span data-stu-id="8cc4b-135">name</span></span>|<span data-ttu-id="8cc4b-136">String</span><span class="sxs-lookup"><span data-stu-id="8cc4b-136">String</span></span>|<span data-ttu-id="8cc4b-137">连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-137">The name of the connector.</span></span>|
|<span data-ttu-id="8cc4b-138">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="8cc4b-138">fullyQualifiedDomainName</span></span>|<span data-ttu-id="8cc4b-139">String</span><span class="sxs-lookup"><span data-stu-id="8cc4b-139">String</span></span>|<span data-ttu-id="8cc4b-140">连接器计算机的主机名。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-140">The connector machine's hostname.</span></span>|
|<span data-ttu-id="8cc4b-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc4b-141">operatingSystem</span></span>|<span data-ttu-id="8cc4b-142">String</span><span class="sxs-lookup"><span data-stu-id="8cc4b-142">String</span></span>|<span data-ttu-id="8cc4b-143">连接器计算机的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-143">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="8cc4b-144">appVersion</span><span class="sxs-lookup"><span data-stu-id="8cc4b-144">appVersion</span></span>|<span data-ttu-id="8cc4b-145">String</span><span class="sxs-lookup"><span data-stu-id="8cc4b-145">String</span></span>|<span data-ttu-id="8cc4b-146">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-146">The connector's version.</span></span>|
|<span data-ttu-id="8cc4b-147">位置</span><span class="sxs-lookup"><span data-stu-id="8cc4b-147">location</span></span>|[<span data-ttu-id="8cc4b-148">printerLocation</span><span class="sxs-lookup"><span data-stu-id="8cc4b-148">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="8cc4b-149">连接器的物理位置和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-149">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="8cc4b-150">响应</span><span class="sxs-lookup"><span data-stu-id="8cc4b-150">Response</span></span>
<span data-ttu-id="8cc4b-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[printConnector](../resources/printConnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-151">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cc4b-152">示例</span><span class="sxs-lookup"><span data-stu-id="8cc4b-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cc4b-153">请求</span><span class="sxs-lookup"><span data-stu-id="8cc4b-153">Request</span></span>
<span data-ttu-id="8cc4b-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cc4b-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc4b-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connector"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/connectors/{id}
Content-type: application/json
Content-length: 300

{
  "name": "ConnectorName",
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
# <a name="c"></a>[<span data-ttu-id="8cc4b-156">C#</span><span class="sxs-lookup"><span data-stu-id="8cc4b-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cc4b-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc4b-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cc4b-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc4b-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8cc4b-159">响应</span><span class="sxs-lookup"><span data-stu-id="8cc4b-159">Response</span></span>
<span data-ttu-id="8cc4b-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-160">The following is an example of the response.</span></span>
><span data-ttu-id="8cc4b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8cc4b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 406

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
  "description": "Update printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
