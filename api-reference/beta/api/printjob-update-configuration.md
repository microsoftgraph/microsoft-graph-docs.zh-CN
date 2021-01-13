---
title: 更新 printJob 配置
description: 更新打印作业的配置
author: tomsato-ms
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1f4d2f1c5573e7f4ad4ae150c598788ab40163ab
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843579"
---
# <a name="update-printjob-configuration"></a><span data-ttu-id="df557-103">更新 printJob 配置</span><span class="sxs-lookup"><span data-stu-id="df557-103">Update printJob configuration</span></span>

<span data-ttu-id="df557-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df557-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df557-105">更新 [打印](../resources/printjobconfiguration.md) 作业 [的配置属性](../resources/printjob.md)。</span><span class="sxs-lookup"><span data-stu-id="df557-105">Update the [configuration](../resources/printjobconfiguration.md) property of a [print job](../resources/printjob.md).</span></span>

<span data-ttu-id="df557-106">只有在关联的打印作业上存在 [printTask](../resources/printTask.md) 状态（由请求创建应用的触发器启动）时，更新打印作业配置才能 `processing` 成功。</span><span class="sxs-lookup"><span data-stu-id="df557-106">Updating a print job configuration will only succeed if there is a [printTask](../resources/printTask.md) in `processing` state on the associated print job, started by a trigger that requesting app created.</span></span> <span data-ttu-id="df557-107">若要详细了解如何注册任务触发器，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="df557-107">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="df557-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="df557-108">Permissions</span></span>
<span data-ttu-id="df557-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df557-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="df557-111">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅（Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限）以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="df557-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="df557-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="df557-112">Permission type</span></span> | <span data-ttu-id="df557-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df557-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="df557-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df557-114">Delegated (work or school account)</span></span>| <span data-ttu-id="df557-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="df557-115">Not supported.</span></span> |
|<span data-ttu-id="df557-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df557-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df557-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="df557-117">Not Supported.</span></span>|
|<span data-ttu-id="df557-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="df557-118">Application</span></span>| <span data-ttu-id="df557-119">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df557-119">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df557-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df557-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a><span data-ttu-id="df557-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="df557-121">Request headers</span></span>
| <span data-ttu-id="df557-122">名称</span><span class="sxs-lookup"><span data-stu-id="df557-122">Name</span></span>          | <span data-ttu-id="df557-123">说明</span><span class="sxs-lookup"><span data-stu-id="df557-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="df557-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df557-124">Authorization</span></span> | <span data-ttu-id="df557-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df557-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df557-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df557-127">Request body</span></span>
<span data-ttu-id="df557-128">在请求正文中，提供相关 [printJobConfiguration 字段](../resources/printjobconfiguration.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="df557-128">In the request body, supply the values of the relevant [printJobConfiguration](../resources/printjobconfiguration.md) fields.</span></span> <span data-ttu-id="df557-129">请求正文中未包含的现有属性将保留其以前的值。</span><span class="sxs-lookup"><span data-stu-id="df557-129">Existing properties that are not included in the request body will maintain their previous values.</span></span>

## <a name="response"></a><span data-ttu-id="df557-130">响应</span><span class="sxs-lookup"><span data-stu-id="df557-130">Response</span></span>
<span data-ttu-id="df557-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="df557-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df557-132">示例</span><span class="sxs-lookup"><span data-stu-id="df557-132">Example</span></span>
<span data-ttu-id="df557-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="df557-133">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="df557-134">请求</span><span class="sxs-lookup"><span data-stu-id="df557-134">Request</span></span>
<span data-ttu-id="df557-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df557-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="df557-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="df557-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

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
# <a name="c"></a>[<span data-ttu-id="df557-137">C#</span><span class="sxs-lookup"><span data-stu-id="df557-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-update-configuration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df557-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df557-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-update-configuration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df557-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df557-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-update-configuration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df557-140">Java</span><span class="sxs-lookup"><span data-stu-id="df557-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-update-configuration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="df557-141">响应</span><span class="sxs-lookup"><span data-stu-id="df557-141">Response</span></span>
<span data-ttu-id="df557-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df557-142">The following is an example of the response.</span></span> 
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


