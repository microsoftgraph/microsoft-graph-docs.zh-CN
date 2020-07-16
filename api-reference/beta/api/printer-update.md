---
title: 更新打印机
description: 更新 printer 对象的属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fd44a74bd1a0a5a8c872f49515edce23c27d6907
ms.sourcegitcommit: 9f1e02ab486a2c3e0a128e5d36f46cebe4961581
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2020
ms.locfileid: "45024427"
---
# <a name="update-printer"></a><span data-ttu-id="3c886-103">更新打印机</span><span class="sxs-lookup"><span data-stu-id="3c886-103">Update printer</span></span>

<span data-ttu-id="3c886-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c886-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c886-105">更新[printer](../resources/printer.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c886-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c886-106">权限</span><span class="sxs-lookup"><span data-stu-id="3c886-106">Permissions</span></span>
<span data-ttu-id="3c886-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3c886-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="3c886-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> 

<span data-ttu-id="3c886-110">仅允许注册打印机的应用程序使用应用程序权限更新打印机。</span><span class="sxs-lookup"><span data-stu-id="3c886-110">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="3c886-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c886-111">Permission type</span></span> | <span data-ttu-id="3c886-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c886-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3c886-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c886-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3c886-114">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="3c886-114">Users.Read.All</span></span> |
|<span data-ttu-id="3c886-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c886-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c886-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c886-116">Not Supported.</span></span>|
|<span data-ttu-id="3c886-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c886-117">Application</span></span>|<span data-ttu-id="3c886-118">Printer ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="3c886-118">Printer.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c886-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c886-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3c886-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c886-120">Request headers</span></span>
| <span data-ttu-id="3c886-121">名称</span><span class="sxs-lookup"><span data-stu-id="3c886-121">Name</span></span>       | <span data-ttu-id="3c886-122">说明</span><span class="sxs-lookup"><span data-stu-id="3c886-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3c886-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c886-123">Authorization</span></span> | <span data-ttu-id="3c886-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c886-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c886-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3c886-126">Content-type</span></span>  | <span data-ttu-id="3c886-127">`application/json`使用委派权限时， `application/ipp` 使用应用程序权限时。</span><span class="sxs-lookup"><span data-stu-id="3c886-127">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="3c886-128">必需。</span><span class="sxs-lookup"><span data-stu-id="3c886-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c886-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c886-129">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="3c886-130">委派权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="3c886-130">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="3c886-131">如果使用委派权限，则在请求正文中，提供应更新的相关[打印机](../resources/printer.md)字段的值。</span><span class="sxs-lookup"><span data-stu-id="3c886-131">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="3c886-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="3c886-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3c886-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3c886-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c886-134">属性</span><span class="sxs-lookup"><span data-stu-id="3c886-134">Property</span></span>     | <span data-ttu-id="3c886-135">类型</span><span class="sxs-lookup"><span data-stu-id="3c886-135">Type</span></span>        | <span data-ttu-id="3c886-136">说明</span><span class="sxs-lookup"><span data-stu-id="3c886-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c886-137">location</span><span class="sxs-lookup"><span data-stu-id="3c886-137">location</span></span>|[<span data-ttu-id="3c886-138">printerLocation</span><span class="sxs-lookup"><span data-stu-id="3c886-138">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="3c886-139">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="3c886-139">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="3c886-140">name</span><span class="sxs-lookup"><span data-stu-id="3c886-140">name</span></span>|<span data-ttu-id="3c886-141">String</span><span class="sxs-lookup"><span data-stu-id="3c886-141">String</span></span>|<span data-ttu-id="3c886-142">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="3c886-142">The name of the printer.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="3c886-143">应用程序权限和 IPP 有效负载</span><span class="sxs-lookup"><span data-stu-id="3c886-143">Application permissions and IPP payload</span></span>

<span data-ttu-id="3c886-144">如果使用应用程序权限，则请求正文包含一个二进制流，表示[IPP 编码](https://tools.ietf.org/html/rfc8010)中的打印机属性组。</span><span class="sxs-lookup"><span data-stu-id="3c886-144">If using application permissions, the request body contains a binary stream representing the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="3c886-145">客户端必须提供一组具有一个或多个值（包括显式允许的带外值）的一组打印机属性，如[RFC8011 section 4.2](https://tools.ietf.org/html/rfc8011#section-4.2)作业模板属性（"xxx-默认"、"支持 xxx" 和 "xxx-就绪" 属性）中的定义，[第4.4 节](https://tools.ietf.org/html/rfc8011#section-4.4)打印机说明属性以及打印机支持的任何属性扩展。</span><span class="sxs-lookup"><span data-stu-id="3c886-145">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 4.2](https://tools.ietf.org/html/rfc8011#section-4.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 4.4](https://tools.ietf.org/html/rfc8011#section-4.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="3c886-146">提供的每个打印机属性的值将替换目标打印机对象上相应的打印机属性的值。</span><span class="sxs-lookup"><span data-stu-id="3c886-146">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="3c886-147">对于可以具有多个值（1setOf）的属性，客户端提供的所有值都将替换相应的打印机对象属性的所有值。</span><span class="sxs-lookup"><span data-stu-id="3c886-147">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="3c886-148">响应</span><span class="sxs-lookup"><span data-stu-id="3c886-148">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="3c886-149">委派权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="3c886-149">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="3c886-150">如果使用委派权限，如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[printer](../resources/printer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c886-150">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="3c886-151">应用程序权限和 IPP 有效负载</span><span class="sxs-lookup"><span data-stu-id="3c886-151">Application permissions and IPP payload</span></span>

<span data-ttu-id="3c886-152">如果使用应用程序权限，如果成功，此方法将返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3c886-152">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="3c886-153">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c886-153">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c886-154">示例</span><span class="sxs-lookup"><span data-stu-id="3c886-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c886-155">请求</span><span class="sxs-lookup"><span data-stu-id="3c886-155">Request</span></span>
<span data-ttu-id="3c886-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c886-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c886-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c886-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3c886-158">C#</span><span class="sxs-lookup"><span data-stu-id="3c886-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c886-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c886-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c886-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c886-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3c886-161">响应</span><span class="sxs-lookup"><span data-stu-id="3c886-161">Response</span></span>
<span data-ttu-id="3c886-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3c886-162">The following is an example of the response.</span></span>
><span data-ttu-id="3c886-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3c886-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
