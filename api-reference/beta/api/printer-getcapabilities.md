---
title: printer： getCapabilities
description: 获取打印机的功能列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a9d9b1e21d26e39ea50020f56f48f496c83b609c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447684"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="a6c4d-103">printer： getCapabilities</span><span class="sxs-lookup"><span data-stu-id="a6c4d-103">printer: getCapabilities</span></span>

<span data-ttu-id="a6c4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c4d-105">获取打印机的功能 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c4d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a6c4d-106">Permissions</span></span>
<span data-ttu-id="a6c4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a6c4d-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a6c4d-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a6c4d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6c4d-111">Permission type</span></span> | <span data-ttu-id="a6c4d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6c4d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a6c4d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c4d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a6c4d-114">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a6c4d-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a6c4d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c4d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-116">Not Supported.</span></span>|
|<span data-ttu-id="a6c4d-117">Application</span><span class="sxs-lookup"><span data-stu-id="a6c4d-117">Application</span></span>| <span data-ttu-id="a6c4d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c4d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6c4d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="a6c4d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6c4d-120">Request headers</span></span>
| <span data-ttu-id="a6c4d-121">名称</span><span class="sxs-lookup"><span data-stu-id="a6c4d-121">Name</span></span>          | <span data-ttu-id="a6c4d-122">说明</span><span class="sxs-lookup"><span data-stu-id="a6c4d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a6c4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c4d-123">Authorization</span></span> | <span data-ttu-id="a6c4d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6c4d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6c4d-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a6c4d-127">响应</span><span class="sxs-lookup"><span data-stu-id="a6c4d-127">Response</span></span>
<span data-ttu-id="a6c4d-128">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printerCapabilities](../resources/printercapabilities.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-128">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c4d-129">示例</span><span class="sxs-lookup"><span data-stu-id="a6c4d-129">Example</span></span>
<span data-ttu-id="a6c4d-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a6c4d-131">请求</span><span class="sxs-lookup"><span data-stu-id="a6c4d-131">Request</span></span>
<span data-ttu-id="a6c4d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6c4d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c4d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="a6c4d-134">C#</span><span class="sxs-lookup"><span data-stu-id="a6c4d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6c4d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6c4d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6c4d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6c4d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6c4d-137">Java</span><span class="sxs-lookup"><span data-stu-id="a6c4d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-getcapabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a6c4d-138">响应</span><span class="sxs-lookup"><span data-stu-id="a6c4d-138">Response</span></span>
<span data-ttu-id="a6c4d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-139">The following is an example of the response.</span></span>
><span data-ttu-id="a6c4d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a6c4d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerCapabilities"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1159

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.printerCapabilities",
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "supportedDocumentMimeTypes": [
        "application/oxps"
    ],
    "supportedFinishings": [
        "none"
    ],
    "supportedMediaColors": [],
    "supportedMediaTypes": [],
    "supportedMediaSizes": [
        "North America Letter",
        "North America Ledger",
        "North America Legal",
        "North America Invoice",
        "North America Executive",
        "A3",
        "A4",
        "A5",
        "JIS B4",
        "JIS B5"
    ],
    "supportedOrientations": [
        "portrait",
        "landscape"
    ],
    "supportedOutputBins": [
        "tray-1"
    ],
    "supportedDuplexConfigurations": [
        "oneSided"
    ],
    "supportedPresentationDirections": [],
    "supportedColorConfigurations": [
        "color"
    ],
    "supportedPrintQualities": [
        "medium"
    ],
    "supportedPagesPerSheet": null,
    "supportedCopiesPerJob": {
        "minimum": 1,
        "maximum": 1
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: getCapabilities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
