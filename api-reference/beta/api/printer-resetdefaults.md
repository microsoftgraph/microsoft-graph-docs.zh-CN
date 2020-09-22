---
title: 打印机： resetDefaults
description: 重置打印机的默认设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 371c76738833eeabfafb68b1b8c6816f831e32ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035615"
---
# <a name="printer-resetdefaults"></a><span data-ttu-id="36ed9-103">打印机： resetDefaults</span><span class="sxs-lookup"><span data-stu-id="36ed9-103">printer: resetDefaults</span></span>

<span data-ttu-id="36ed9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36ed9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ed9-105">重置 [打印机](../resources/printer.md)的默认设置。</span><span class="sxs-lookup"><span data-stu-id="36ed9-105">Reset a [printer](../resources/printer.md)'s default settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="36ed9-106">权限</span><span class="sxs-lookup"><span data-stu-id="36ed9-106">Permissions</span></span>
<span data-ttu-id="36ed9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="36ed9-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="36ed9-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="36ed9-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="36ed9-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="36ed9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36ed9-111">Permission type</span></span> | <span data-ttu-id="36ed9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36ed9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="36ed9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36ed9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="36ed9-114">完全控制和所有打印机。</span><span class="sxs-lookup"><span data-stu-id="36ed9-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="36ed9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36ed9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36ed9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ed9-116">Not Supported.</span></span>|
|<span data-ttu-id="36ed9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36ed9-117">Application</span></span>| <span data-ttu-id="36ed9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ed9-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36ed9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36ed9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/resetDefaults
```
## <a name="request-headers"></a><span data-ttu-id="36ed9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36ed9-120">Request headers</span></span>
| <span data-ttu-id="36ed9-121">名称</span><span class="sxs-lookup"><span data-stu-id="36ed9-121">Name</span></span>          | <span data-ttu-id="36ed9-122">说明</span><span class="sxs-lookup"><span data-stu-id="36ed9-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36ed9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ed9-123">Authorization</span></span> | <span data-ttu-id="36ed9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36ed9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36ed9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36ed9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="36ed9-127">响应</span><span class="sxs-lookup"><span data-stu-id="36ed9-127">Response</span></span>
<span data-ttu-id="36ed9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="36ed9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36ed9-130">示例</span><span class="sxs-lookup"><span data-stu-id="36ed9-130">Example</span></span>
<span data-ttu-id="36ed9-131">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="36ed9-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36ed9-132">请求</span><span class="sxs-lookup"><span data-stu-id="36ed9-132">Request</span></span>
<span data-ttu-id="36ed9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36ed9-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36ed9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="36ed9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-resetdefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/resetDefaults
```
# <a name="c"></a>[<span data-ttu-id="36ed9-135">C#</span><span class="sxs-lookup"><span data-stu-id="36ed9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-resetdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36ed9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36ed9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-resetdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36ed9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36ed9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-resetdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36ed9-138">响应</span><span class="sxs-lookup"><span data-stu-id="36ed9-138">Response</span></span>
<span data-ttu-id="36ed9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36ed9-139">The following is an example of the response.</span></span> 
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
  "description": "printer: resetDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


