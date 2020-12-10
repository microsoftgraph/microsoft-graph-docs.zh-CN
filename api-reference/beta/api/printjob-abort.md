---
title: printJob： abort
description: 中止打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a17344dbac7282b12db4b8ebb011f922ceaa01d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617132"
---
# <a name="printjob-abort"></a><span data-ttu-id="3c972-103">printJob： abort</span><span class="sxs-lookup"><span data-stu-id="3c972-103">printJob: abort</span></span>

<span data-ttu-id="3c972-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c972-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c972-105">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="3c972-105">Abort a print job.</span></span> <span data-ttu-id="3c972-106">只有使用应用程序权限的应用程序才可以中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="3c972-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c972-107">权限</span><span class="sxs-lookup"><span data-stu-id="3c972-107">Permissions</span></span>
<span data-ttu-id="3c972-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c972-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3c972-110">除了以下权限之外，应用程序的租户也必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="3c972-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="3c972-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c972-111">Permission type</span></span> | <span data-ttu-id="3c972-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c972-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3c972-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c972-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3c972-114">不支持</span><span class="sxs-lookup"><span data-stu-id="3c972-114">Not Supported</span></span> |
|<span data-ttu-id="3c972-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c972-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c972-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c972-116">Not Supported.</span></span>|
|<span data-ttu-id="3c972-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c972-117">Application</span></span>| <span data-ttu-id="3c972-118">PrintJob、PrintJob 和所有 ReadWriteBasic</span><span class="sxs-lookup"><span data-stu-id="3c972-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c972-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c972-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="3c972-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c972-120">Request headers</span></span>
| <span data-ttu-id="3c972-121">名称</span><span class="sxs-lookup"><span data-stu-id="3c972-121">Name</span></span>          | <span data-ttu-id="3c972-122">说明</span><span class="sxs-lookup"><span data-stu-id="3c972-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3c972-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c972-123">Authorization</span></span> | <span data-ttu-id="3c972-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c972-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c972-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c972-126">Request body</span></span>
<span data-ttu-id="3c972-127">在请求正文中，可以选择提供中止作业的原因。</span><span class="sxs-lookup"><span data-stu-id="3c972-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="3c972-128">属性</span><span class="sxs-lookup"><span data-stu-id="3c972-128">Property</span></span>     | <span data-ttu-id="3c972-129">类型</span><span class="sxs-lookup"><span data-stu-id="3c972-129">Type</span></span>        | <span data-ttu-id="3c972-130">说明</span><span class="sxs-lookup"><span data-stu-id="3c972-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c972-131">reason</span><span class="sxs-lookup"><span data-stu-id="3c972-131">reason</span></span>|<span data-ttu-id="3c972-132">String</span><span class="sxs-lookup"><span data-stu-id="3c972-132">String</span></span>|<span data-ttu-id="3c972-133">中止作业的原因。</span><span class="sxs-lookup"><span data-stu-id="3c972-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="3c972-134">响应</span><span class="sxs-lookup"><span data-stu-id="3c972-134">Response</span></span>
<span data-ttu-id="3c972-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c972-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c972-137">示例</span><span class="sxs-lookup"><span data-stu-id="3c972-137">Example</span></span>
<span data-ttu-id="3c972-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3c972-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="3c972-139">请求</span><span class="sxs-lookup"><span data-stu-id="3c972-139">Request</span></span>
<span data-ttu-id="3c972-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c972-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```

### <a name="response"></a><span data-ttu-id="3c972-141">响应</span><span class="sxs-lookup"><span data-stu-id="3c972-141">Response</span></span>
<span data-ttu-id="3c972-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3c972-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: abort",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
