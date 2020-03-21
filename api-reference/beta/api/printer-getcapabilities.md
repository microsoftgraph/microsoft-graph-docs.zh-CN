---
title: 打印机： getCapabilities
description: 获取打印机的功能列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 675b82605f4bde04b92702204693c3c81b4bd603
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895696"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="e4f1b-103">打印机： getCapabilities</span><span class="sxs-lookup"><span data-stu-id="e4f1b-103">printer: getCapabilities</span></span>

<span data-ttu-id="e4f1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f1b-105">获取[打印机](../resources/printer.md)的功能列表。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4f1b-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4f1b-106">Permissions</span></span>
<span data-ttu-id="e4f1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e4f1b-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e4f1b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4f1b-110">Permission type</span></span> | <span data-ttu-id="e4f1b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4f1b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e4f1b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f1b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e4f1b-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="e4f1b-113">Users.Read.All</span></span> |
|<span data-ttu-id="e4f1b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4f1b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-115">Not Supported.</span></span>|
|<span data-ttu-id="e4f1b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4f1b-116">Application</span></span>|<span data-ttu-id="e4f1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4f1b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4f1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="e4f1b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4f1b-119">Request headers</span></span>
| <span data-ttu-id="e4f1b-120">名称</span><span class="sxs-lookup"><span data-stu-id="e4f1b-120">Name</span></span>          | <span data-ttu-id="e4f1b-121">说明</span><span class="sxs-lookup"><span data-stu-id="e4f1b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e4f1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4f1b-122">Authorization</span></span> | <span data-ttu-id="e4f1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4f1b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4f1b-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e4f1b-126">响应</span><span class="sxs-lookup"><span data-stu-id="e4f1b-126">Response</span></span>
<span data-ttu-id="e4f1b-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printerCapabilities](../resources/printercapabilities.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-127">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4f1b-128">示例</span><span class="sxs-lookup"><span data-stu-id="e4f1b-128">Example</span></span>
<span data-ttu-id="e4f1b-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-129">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e4f1b-130">请求</span><span class="sxs-lookup"><span data-stu-id="e4f1b-130">Request</span></span>
<span data-ttu-id="e4f1b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```

##### <a name="response"></a><span data-ttu-id="e4f1b-132">响应</span><span class="sxs-lookup"><span data-stu-id="e4f1b-132">Response</span></span>
<span data-ttu-id="e4f1b-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-133">The following is an example of the response.</span></span>
><span data-ttu-id="e4f1b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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