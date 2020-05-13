---
title: 删除 printerShare
description: 删除打印机共享（共享关联打印机）。 此操作无法撤消。 如果将来再次共享打印机，则之前安装该打印机的所有 Windows 用户都需要发现并重新安装它。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0f890a5311321a100d32419dfaa9515c714c6030
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216915"
---
# <a name="delete-printershare"></a><span data-ttu-id="e51c9-105">删除 printerShare</span><span class="sxs-lookup"><span data-stu-id="e51c9-105">Delete printerShare</span></span>

<span data-ttu-id="e51c9-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e51c9-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e51c9-107">删除打印机共享（共享关联[打印机](../resources/printer.md)）。</span><span class="sxs-lookup"><span data-stu-id="e51c9-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="e51c9-108">此操作无法撤消。</span><span class="sxs-lookup"><span data-stu-id="e51c9-108">This action cannot be undone.</span></span> <span data-ttu-id="e51c9-109">如果将来再次共享[打印机](../resources/printer.md)，则之前安装该[打印机](../resources/printer.md)的所有 Windows 用户都需要发现并重新安装该打印机。</span><span class="sxs-lookup"><span data-stu-id="e51c9-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="e51c9-110">权限</span><span class="sxs-lookup"><span data-stu-id="e51c9-110">Permissions</span></span>
<span data-ttu-id="e51c9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e51c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e51c9-113">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e51c9-113">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e51c9-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e51c9-114">Permission type</span></span> | <span data-ttu-id="e51c9-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e51c9-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e51c9-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e51c9-116">Delegated (work or school account)</span></span>| <span data-ttu-id="e51c9-117">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="e51c9-117">Users.Read.All</span></span> |
|<span data-ttu-id="e51c9-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e51c9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e51c9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e51c9-119">Not Supported.</span></span>|
|<span data-ttu-id="e51c9-120">Application</span><span class="sxs-lookup"><span data-stu-id="e51c9-120">Application</span></span>|<span data-ttu-id="e51c9-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="e51c9-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e51c9-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e51c9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="e51c9-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e51c9-123">Request headers</span></span>
| <span data-ttu-id="e51c9-124">名称</span><span class="sxs-lookup"><span data-stu-id="e51c9-124">Name</span></span>          | <span data-ttu-id="e51c9-125">说明</span><span class="sxs-lookup"><span data-stu-id="e51c9-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e51c9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e51c9-126">Authorization</span></span> | <span data-ttu-id="e51c9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e51c9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e51c9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e51c9-129">Request body</span></span>
<span data-ttu-id="e51c9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e51c9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e51c9-131">响应</span><span class="sxs-lookup"><span data-stu-id="e51c9-131">Response</span></span>
<span data-ttu-id="e51c9-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e51c9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e51c9-134">示例</span><span class="sxs-lookup"><span data-stu-id="e51c9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e51c9-135">请求</span><span class="sxs-lookup"><span data-stu-id="e51c9-135">Request</span></span>
<span data-ttu-id="e51c9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e51c9-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e51c9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e51c9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="e51c9-138">C#</span><span class="sxs-lookup"><span data-stu-id="e51c9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e51c9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e51c9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e51c9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e51c9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e51c9-141">响应</span><span class="sxs-lookup"><span data-stu-id="e51c9-141">Response</span></span>
<span data-ttu-id="e51c9-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e51c9-142">The following is an example of the response.</span></span>
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
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
