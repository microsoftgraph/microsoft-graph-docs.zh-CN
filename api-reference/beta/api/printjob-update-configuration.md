---
title: 更新 printJob 配置
description: 更新打印作业的配置
author: tomsato-ms
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 85063072fb1a9c8d7ec4e5a12805b2fe65a50ddd
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753088"
---
# <a name="update-printjob-configuration"></a><span data-ttu-id="b599b-103">更新 printJob 配置</span><span class="sxs-lookup"><span data-stu-id="b599b-103">Update printJob configuration</span></span>

<span data-ttu-id="b599b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b599b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b599b-105">更新 [打印](../resources/printjobconfiguration.md) 作业 [的配置属性](../resources/printjob.md)。</span><span class="sxs-lookup"><span data-stu-id="b599b-105">Update the [configuration](../resources/printjobconfiguration.md) property of a [print job](../resources/printjob.md).</span></span>

<span data-ttu-id="b599b-106">更新打印作业配置需要通过为打印机注册任务触发器使打印作业进入一个保存状态。</span><span class="sxs-lookup"><span data-stu-id="b599b-106">Updating a print job configuration requires the print job to be in a held state by registering a task trigger for the printer.</span></span> <span data-ttu-id="b599b-107">若要详细了解如何注册任务触发器，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="b599b-107">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="b599b-108">权限</span><span class="sxs-lookup"><span data-stu-id="b599b-108">Permissions</span></span>
<span data-ttu-id="b599b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b599b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b599b-111">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="b599b-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="b599b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b599b-112">Permission type</span></span> | <span data-ttu-id="b599b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b599b-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b599b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b599b-114">Delegated (work or school account)</span></span>| <span data-ttu-id="b599b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b599b-115">Not supported.</span></span> |
|<span data-ttu-id="b599b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b599b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b599b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b599b-117">Not Supported.</span></span>|
|<span data-ttu-id="b599b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b599b-118">Application</span></span>| <span data-ttu-id="b599b-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b599b-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b599b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b599b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a><span data-ttu-id="b599b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b599b-121">Request headers</span></span>
| <span data-ttu-id="b599b-122">名称</span><span class="sxs-lookup"><span data-stu-id="b599b-122">Name</span></span>          | <span data-ttu-id="b599b-123">说明</span><span class="sxs-lookup"><span data-stu-id="b599b-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b599b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b599b-124">Authorization</span></span> | <span data-ttu-id="b599b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b599b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b599b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b599b-127">Request body</span></span>
<span data-ttu-id="b599b-128">在请求正文中，提供相关 [printJobConfiguration 字段](../resources/printjobconfiguration.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="b599b-128">In the request body, supply the values of the relevant [printJobConfiguration](../resources/printjobconfiguration.md) fields.</span></span> <span data-ttu-id="b599b-129">请求正文中未包含的现有属性将保留其以前的值。</span><span class="sxs-lookup"><span data-stu-id="b599b-129">Existing properties that are not included in the request body will maintain their previous values.</span></span>

## <a name="response"></a><span data-ttu-id="b599b-130">响应</span><span class="sxs-lookup"><span data-stu-id="b599b-130">Response</span></span>
<span data-ttu-id="b599b-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b599b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b599b-132">示例</span><span class="sxs-lookup"><span data-stu-id="b599b-132">Example</span></span>
<span data-ttu-id="b599b-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b599b-133">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="b599b-134">请求</span><span class="sxs-lookup"><span data-stu-id="b599b-134">Request</span></span>
<span data-ttu-id="b599b-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b599b-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b599b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b599b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

{
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
```
# <a name="javascript"></a>[<span data-ttu-id="b599b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b599b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-update-configuration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b599b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b599b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-update-configuration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b599b-139">响应</span><span class="sxs-lookup"><span data-stu-id="b599b-139">Response</span></span>
<span data-ttu-id="b599b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b599b-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


