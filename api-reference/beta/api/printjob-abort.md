---
title: printJob： abort
description: 中止打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 597d92e051940d94a53364c624a8d0d20ef23dce
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080633"
---
# <a name="printjob-abort"></a><span data-ttu-id="52db1-103">printJob： abort</span><span class="sxs-lookup"><span data-stu-id="52db1-103">printJob: abort</span></span>

<span data-ttu-id="52db1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52db1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52db1-105">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="52db1-105">Abort a print job.</span></span> <span data-ttu-id="52db1-106">只有使用应用程序权限的应用程序才能中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="52db1-106">Only applications using application permissions can abort a print job.</span></span>

<span data-ttu-id="52db1-107">只有在关联的打印作业上存在由请求应用创建的触发器启动的 [printTask](../resources/printTask.md) 状态时，中止打印作业才能 `processing` 成功。</span><span class="sxs-lookup"><span data-stu-id="52db1-107">Aborting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="52db1-108">若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="52db1-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="52db1-109">权限</span><span class="sxs-lookup"><span data-stu-id="52db1-109">Permissions</span></span>
<span data-ttu-id="52db1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52db1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="52db1-112">除了以下权限之外，应用的租户还必须具有活动的通用打印订阅，并且必须具有 Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="52db1-112">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="52db1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="52db1-113">Permission type</span></span> | <span data-ttu-id="52db1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52db1-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="52db1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52db1-115">Delegated (work or school account)</span></span>| <span data-ttu-id="52db1-116">不支持</span><span class="sxs-lookup"><span data-stu-id="52db1-116">Not Supported</span></span> |
|<span data-ttu-id="52db1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52db1-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52db1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="52db1-118">Not Supported.</span></span>|
|<span data-ttu-id="52db1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="52db1-119">Application</span></span>| <span data-ttu-id="52db1-120">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="52db1-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52db1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52db1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="52db1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="52db1-122">Request headers</span></span>
| <span data-ttu-id="52db1-123">名称</span><span class="sxs-lookup"><span data-stu-id="52db1-123">Name</span></span>          | <span data-ttu-id="52db1-124">说明</span><span class="sxs-lookup"><span data-stu-id="52db1-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="52db1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="52db1-125">Authorization</span></span> | <span data-ttu-id="52db1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52db1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52db1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="52db1-128">Request body</span></span>
<span data-ttu-id="52db1-129">在请求正文中，可以选择提供作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="52db1-129">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="52db1-130">属性</span><span class="sxs-lookup"><span data-stu-id="52db1-130">Property</span></span>     | <span data-ttu-id="52db1-131">类型</span><span class="sxs-lookup"><span data-stu-id="52db1-131">Type</span></span>        | <span data-ttu-id="52db1-132">说明</span><span class="sxs-lookup"><span data-stu-id="52db1-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52db1-133">reason</span><span class="sxs-lookup"><span data-stu-id="52db1-133">reason</span></span>|<span data-ttu-id="52db1-134">String</span><span class="sxs-lookup"><span data-stu-id="52db1-134">String</span></span>|<span data-ttu-id="52db1-135">作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="52db1-135">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="52db1-136">响应</span><span class="sxs-lookup"><span data-stu-id="52db1-136">Response</span></span>
<span data-ttu-id="52db1-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="52db1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52db1-139">示例</span><span class="sxs-lookup"><span data-stu-id="52db1-139">Example</span></span>
<span data-ttu-id="52db1-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="52db1-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="52db1-141">请求</span><span class="sxs-lookup"><span data-stu-id="52db1-141">Request</span></span>
<span data-ttu-id="52db1-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="52db1-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="52db1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="52db1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```
# <a name="c"></a>[<span data-ttu-id="52db1-144">C#</span><span class="sxs-lookup"><span data-stu-id="52db1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52db1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52db1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52db1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52db1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52db1-147">Java</span><span class="sxs-lookup"><span data-stu-id="52db1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52db1-148">响应</span><span class="sxs-lookup"><span data-stu-id="52db1-148">Response</span></span>
<span data-ttu-id="52db1-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="52db1-149">The following is an example of the response.</span></span> 
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
