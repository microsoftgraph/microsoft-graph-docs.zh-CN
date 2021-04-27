---
title: printer： getCapabilities
description: 获取打印机的功能列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2e3720014b3094d8d8696b6931f37586590b7d8a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049910"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="6b180-103">printer： getCapabilities</span><span class="sxs-lookup"><span data-stu-id="6b180-103">printer: getCapabilities</span></span>

<span data-ttu-id="6b180-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b180-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b180-105">获取打印机 的功能 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="6b180-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b180-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b180-106">Permissions</span></span>
<span data-ttu-id="6b180-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6b180-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="6b180-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="6b180-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="6b180-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="6b180-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b180-111">Permission type</span></span> | <span data-ttu-id="6b180-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b180-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6b180-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b180-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6b180-114">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6b180-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="6b180-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b180-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b180-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b180-116">Not Supported.</span></span>|
|<span data-ttu-id="6b180-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b180-117">Application</span></span>| <span data-ttu-id="6b180-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b180-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b180-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b180-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="6b180-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b180-120">Request headers</span></span>
| <span data-ttu-id="6b180-121">名称</span><span class="sxs-lookup"><span data-stu-id="6b180-121">Name</span></span>          | <span data-ttu-id="6b180-122">说明</span><span class="sxs-lookup"><span data-stu-id="6b180-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6b180-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b180-123">Authorization</span></span> | <span data-ttu-id="6b180-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b180-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b180-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b180-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6b180-127">响应</span><span class="sxs-lookup"><span data-stu-id="6b180-127">Response</span></span>
<span data-ttu-id="6b180-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printerCapabilities](../resources/printercapabilities.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b180-128">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b180-129">示例</span><span class="sxs-lookup"><span data-stu-id="6b180-129">Example</span></span>
<span data-ttu-id="6b180-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6b180-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6b180-131">请求</span><span class="sxs-lookup"><span data-stu-id="6b180-131">Request</span></span>
<span data-ttu-id="6b180-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b180-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b180-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b180-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="6b180-134">C#</span><span class="sxs-lookup"><span data-stu-id="6b180-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b180-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b180-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b180-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b180-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b180-137">Java</span><span class="sxs-lookup"><span data-stu-id="6b180-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-getcapabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6b180-138">响应</span><span class="sxs-lookup"><span data-stu-id="6b180-138">Response</span></span>
<span data-ttu-id="6b180-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b180-139">The following is an example of the response.</span></span>
><span data-ttu-id="6b180-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b180-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
