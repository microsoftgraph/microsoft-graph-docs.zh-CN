---
title: printJob： redirect
description: 将打印作业重定向到其他打印机。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 844fbf0d990a51a199fade3f8bbd9719fd77bae0
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517276"
---
# <a name="printjob-redirect"></a><span data-ttu-id="1f98b-103">printJob： redirect</span><span class="sxs-lookup"><span data-stu-id="1f98b-103">printJob: redirect</span></span>
<span data-ttu-id="1f98b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f98b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1f98b-105">将 [打印作业重定向到](../resources/printjob.md) 其他 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="1f98b-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="1f98b-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="1f98b-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f98b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1f98b-107">Permissions</span></span>
<span data-ttu-id="1f98b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f98b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1f98b-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="1f98b-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="1f98b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f98b-111">Permission type</span></span> | <span data-ttu-id="1f98b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f98b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1f98b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f98b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1f98b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f98b-114">Not supported.</span></span> |
|<span data-ttu-id="1f98b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f98b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f98b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f98b-116">Not Supported.</span></span>|
|<span data-ttu-id="1f98b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f98b-117">Application</span></span>| <span data-ttu-id="1f98b-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1f98b-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f98b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f98b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="1f98b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f98b-120">Request headers</span></span>
|<span data-ttu-id="1f98b-121">名称</span><span class="sxs-lookup"><span data-stu-id="1f98b-121">Name</span></span>|<span data-ttu-id="1f98b-122">说明</span><span class="sxs-lookup"><span data-stu-id="1f98b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f98b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f98b-123">Authorization</span></span>|<span data-ttu-id="1f98b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f98b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f98b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f98b-126">Content-Type</span></span>|<span data-ttu-id="1f98b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1f98b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f98b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f98b-129">Request body</span></span>
<span data-ttu-id="1f98b-130">在请求正文中，提供打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="1f98b-130">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="1f98b-131">属性</span><span class="sxs-lookup"><span data-stu-id="1f98b-131">Property</span></span>     | <span data-ttu-id="1f98b-132">类型</span><span class="sxs-lookup"><span data-stu-id="1f98b-132">Type</span></span>        | <span data-ttu-id="1f98b-133">Description</span><span class="sxs-lookup"><span data-stu-id="1f98b-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f98b-134">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="1f98b-134">destinationPrinterId</span></span>|<span data-ttu-id="1f98b-135">String</span><span class="sxs-lookup"><span data-stu-id="1f98b-135">String</span></span>|<span data-ttu-id="1f98b-136">打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="1f98b-136">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="1f98b-137">configuration</span><span class="sxs-lookup"><span data-stu-id="1f98b-137">configuration</span></span>|<span data-ttu-id="1f98b-138">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f98b-138">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="1f98b-139">更新了打印作业的配置。</span><span class="sxs-lookup"><span data-stu-id="1f98b-139">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="1f98b-140">响应</span><span class="sxs-lookup"><span data-stu-id="1f98b-140">Response</span></span>
<span data-ttu-id="1f98b-141">如果成功，此方法将返回一个响应代码和一个为目标打印机排队 `200 OK` 的 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f98b-141">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="examples"></a><span data-ttu-id="1f98b-142">示例</span><span class="sxs-lookup"><span data-stu-id="1f98b-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f98b-143">请求</span><span class="sxs-lookup"><span data-stu-id="1f98b-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob_redirect"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/redirect
Content-Type: application/json
Content-length: 128

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea",
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

### <a name="response"></a><span data-ttu-id="1f98b-144">响应</span><span class="sxs-lookup"><span data-stu-id="1f98b-144">Response</span></span>
<span data-ttu-id="1f98b-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1f98b-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea')/jobs/$entity",
  "id": "24123",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "processing",
    "description": "The print job is currently being processed by the printer.",
    "details": ["interpreting"]
  },
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

