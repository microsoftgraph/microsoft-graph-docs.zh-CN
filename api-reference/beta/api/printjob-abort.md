---
title: printJob： abort
description: 中止打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cfd82c356463f3e642d5817ff0203c2bec8627db
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515448"
---
# <a name="printjob-abort"></a><span data-ttu-id="f7c40-103">printJob： abort</span><span class="sxs-lookup"><span data-stu-id="f7c40-103">printJob: abort</span></span>

<span data-ttu-id="f7c40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7c40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c40-105">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="f7c40-105">Abort a print job.</span></span> <span data-ttu-id="f7c40-106">只有使用应用程序权限的应用程序才能中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="f7c40-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c40-107">权限</span><span class="sxs-lookup"><span data-stu-id="f7c40-107">Permissions</span></span>
<span data-ttu-id="f7c40-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7c40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f7c40-110">除了以下权限外，应用的租户还必须具有活动的通用打印订阅，并且必须具有 Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="f7c40-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="f7c40-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7c40-111">Permission type</span></span> | <span data-ttu-id="f7c40-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7c40-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f7c40-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c40-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f7c40-114">不支持</span><span class="sxs-lookup"><span data-stu-id="f7c40-114">Not Supported</span></span> |
|<span data-ttu-id="f7c40-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c40-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7c40-116">Not Supported.</span></span>|
|<span data-ttu-id="f7c40-117">Application</span><span class="sxs-lookup"><span data-stu-id="f7c40-117">Application</span></span>| <span data-ttu-id="f7c40-118">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f7c40-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7c40-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7c40-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="f7c40-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7c40-120">Request headers</span></span>
| <span data-ttu-id="f7c40-121">名称</span><span class="sxs-lookup"><span data-stu-id="f7c40-121">Name</span></span>          | <span data-ttu-id="f7c40-122">说明</span><span class="sxs-lookup"><span data-stu-id="f7c40-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7c40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7c40-123">Authorization</span></span> | <span data-ttu-id="f7c40-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7c40-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7c40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7c40-126">Request body</span></span>
<span data-ttu-id="f7c40-127">在请求正文中，可以选择提供作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="f7c40-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="f7c40-128">属性</span><span class="sxs-lookup"><span data-stu-id="f7c40-128">Property</span></span>     | <span data-ttu-id="f7c40-129">类型</span><span class="sxs-lookup"><span data-stu-id="f7c40-129">Type</span></span>        | <span data-ttu-id="f7c40-130">说明</span><span class="sxs-lookup"><span data-stu-id="f7c40-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7c40-131">reason</span><span class="sxs-lookup"><span data-stu-id="f7c40-131">reason</span></span>|<span data-ttu-id="f7c40-132">String</span><span class="sxs-lookup"><span data-stu-id="f7c40-132">String</span></span>|<span data-ttu-id="f7c40-133">作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="f7c40-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="f7c40-134">响应</span><span class="sxs-lookup"><span data-stu-id="f7c40-134">Response</span></span>
<span data-ttu-id="f7c40-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f7c40-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c40-137">示例</span><span class="sxs-lookup"><span data-stu-id="f7c40-137">Example</span></span>
<span data-ttu-id="f7c40-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f7c40-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="f7c40-139">请求</span><span class="sxs-lookup"><span data-stu-id="f7c40-139">Request</span></span>
<span data-ttu-id="f7c40-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7c40-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7c40-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c40-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```
# <a name="c"></a>[<span data-ttu-id="f7c40-142">C#</span><span class="sxs-lookup"><span data-stu-id="f7c40-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7c40-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7c40-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7c40-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7c40-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7c40-145">Java</span><span class="sxs-lookup"><span data-stu-id="f7c40-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7c40-146">响应</span><span class="sxs-lookup"><span data-stu-id="f7c40-146">Response</span></span>
<span data-ttu-id="f7c40-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7c40-147">The following is an example of the response.</span></span> 
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
