---
title: 更新打印机
description: 更新 printer 对象的属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c511598e200b7583b98e6fba1f7d07fa9f9d98dd
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947722"
---
# <a name="update-printer"></a><span data-ttu-id="e1cd3-103">更新打印机</span><span class="sxs-lookup"><span data-stu-id="e1cd3-103">Update printer</span></span>

<span data-ttu-id="e1cd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1cd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1cd3-105">更新[printer](../resources/printer.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1cd3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e1cd3-106">Permissions</span></span>
<span data-ttu-id="e1cd3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e1cd3-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e1cd3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1cd3-110">Permission type</span></span> | <span data-ttu-id="e1cd3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1cd3-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e1cd3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1cd3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e1cd3-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="e1cd3-113">Users.Read.All</span></span> |
|<span data-ttu-id="e1cd3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1cd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1cd3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-115">Not Supported.</span></span>|
|<span data-ttu-id="e1cd3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1cd3-116">Application</span></span>|<span data-ttu-id="e1cd3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1cd3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1cd3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e1cd3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1cd3-119">Request headers</span></span>
| <span data-ttu-id="e1cd3-120">名称</span><span class="sxs-lookup"><span data-stu-id="e1cd3-120">Name</span></span>       | <span data-ttu-id="e1cd3-121">说明</span><span class="sxs-lookup"><span data-stu-id="e1cd3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e1cd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1cd3-122">Authorization</span></span> | <span data-ttu-id="e1cd3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1cd3-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e1cd3-125">Content-type</span></span>  | <span data-ttu-id="e1cd3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e1cd3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1cd3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1cd3-128">Request body</span></span>
<span data-ttu-id="e1cd3-129">在请求正文中，提供应更新的相关[打印机](../resources/printer.md)字段的值。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-129">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="e1cd3-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e1cd3-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e1cd3-132">属性</span><span class="sxs-lookup"><span data-stu-id="e1cd3-132">Property</span></span>     | <span data-ttu-id="e1cd3-133">类型</span><span class="sxs-lookup"><span data-stu-id="e1cd3-133">Type</span></span>        | <span data-ttu-id="e1cd3-134">说明</span><span class="sxs-lookup"><span data-stu-id="e1cd3-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1cd3-135">location</span><span class="sxs-lookup"><span data-stu-id="e1cd3-135">location</span></span>|[<span data-ttu-id="e1cd3-136">printerLocation</span><span class="sxs-lookup"><span data-stu-id="e1cd3-136">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="e1cd3-137">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-137">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="e1cd3-138">name</span><span class="sxs-lookup"><span data-stu-id="e1cd3-138">name</span></span>|<span data-ttu-id="e1cd3-139">String</span><span class="sxs-lookup"><span data-stu-id="e1cd3-139">String</span></span>|<span data-ttu-id="e1cd3-140">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-140">The name of the printer.</span></span>|

## <a name="response"></a><span data-ttu-id="e1cd3-141">响应</span><span class="sxs-lookup"><span data-stu-id="e1cd3-141">Response</span></span>
<span data-ttu-id="e1cd3-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[printer](../resources/printer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-142">If successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1cd3-143">示例</span><span class="sxs-lookup"><span data-stu-id="e1cd3-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1cd3-144">请求</span><span class="sxs-lookup"><span data-stu-id="e1cd3-144">Request</span></span>
<span data-ttu-id="e1cd3-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1cd3-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1cd3-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e1cd3-147">C#</span><span class="sxs-lookup"><span data-stu-id="e1cd3-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1cd3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1cd3-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1cd3-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1cd3-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e1cd3-150">响应</span><span class="sxs-lookup"><span data-stu-id="e1cd3-150">Response</span></span>
<span data-ttu-id="e1cd3-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-151">The following is an example of the response.</span></span>
><span data-ttu-id="e1cd3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e1cd3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "registeredBy": {},
  "status": {
    "processingState": "idle",
    "processingStateReasons": [],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
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
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
