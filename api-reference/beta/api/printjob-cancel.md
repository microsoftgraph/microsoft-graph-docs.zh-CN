---
title: printJob：取消
description: 取消打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b34df3331f2c395f54366adaac0d7edcae321973
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782570"
---
# <a name="printjob-cancel"></a><span data-ttu-id="d7499-103">printJob：取消</span><span class="sxs-lookup"><span data-stu-id="d7499-103">printJob: cancel</span></span>

<span data-ttu-id="d7499-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7499-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7499-105">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="d7499-105">Cancel a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7499-106">权限</span><span class="sxs-lookup"><span data-stu-id="d7499-106">Permissions</span></span>
<span data-ttu-id="d7499-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d7499-109">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="d7499-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="d7499-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7499-110">Permission type</span></span> | <span data-ttu-id="d7499-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7499-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d7499-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7499-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d7499-113">PrintJob、ReadWriteBasic、PrintJob、All、ReadWriteBasic、All</span><span class="sxs-lookup"><span data-stu-id="d7499-113">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="d7499-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7499-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7499-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7499-115">Not Supported.</span></span>|
|<span data-ttu-id="d7499-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7499-116">Application</span></span>| <span data-ttu-id="d7499-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7499-117">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7499-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7499-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="d7499-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7499-119">Request headers</span></span>
| <span data-ttu-id="d7499-120">名称</span><span class="sxs-lookup"><span data-stu-id="d7499-120">Name</span></span>          | <span data-ttu-id="d7499-121">说明</span><span class="sxs-lookup"><span data-stu-id="d7499-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d7499-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7499-122">Authorization</span></span> | <span data-ttu-id="d7499-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7499-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7499-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7499-125">Request body</span></span>
<span data-ttu-id="d7499-126">请求正文应为空。</span><span class="sxs-lookup"><span data-stu-id="d7499-126">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="d7499-127">响应</span><span class="sxs-lookup"><span data-stu-id="d7499-127">Response</span></span>
<span data-ttu-id="d7499-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d7499-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7499-130">示例</span><span class="sxs-lookup"><span data-stu-id="d7499-130">Example</span></span>
<span data-ttu-id="d7499-131">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d7499-131">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="d7499-132">请求</span><span class="sxs-lookup"><span data-stu-id="d7499-132">Request</span></span>
<span data-ttu-id="d7499-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7499-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7499-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7499-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="d7499-135">C#</span><span class="sxs-lookup"><span data-stu-id="d7499-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7499-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7499-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7499-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7499-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7499-138">响应</span><span class="sxs-lookup"><span data-stu-id="d7499-138">Response</span></span>
<span data-ttu-id="d7499-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7499-139">The following is an example of the response.</span></span> 
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
  "description": "printJob: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


