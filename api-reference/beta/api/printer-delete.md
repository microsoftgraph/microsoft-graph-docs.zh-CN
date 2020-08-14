---
title: 删除打印机
description: 删除 (注销) 打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 049b3d08cb73bd6b4e502e527f762c23767ab065
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674447"
---
# <a name="delete-printer"></a><span data-ttu-id="bb882-103">删除打印机</span><span class="sxs-lookup"><span data-stu-id="bb882-103">Delete printer</span></span>

<span data-ttu-id="bb882-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb882-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb882-105">删除 (注销) [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="bb882-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb882-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb882-106">Permissions</span></span>
<span data-ttu-id="bb882-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb882-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bb882-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="bb882-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="bb882-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="bb882-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="bb882-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb882-111">Permission type</span></span> | <span data-ttu-id="bb882-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb882-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bb882-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb882-113">Delegated (work or school account)</span></span>| <span data-ttu-id="bb882-114">完全控制</span><span class="sxs-lookup"><span data-stu-id="bb882-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="bb882-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb882-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb882-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb882-116">Not Supported.</span></span>|
|<span data-ttu-id="bb882-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb882-117">Application</span></span>|<span data-ttu-id="bb882-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb882-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb882-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb882-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bb882-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb882-120">Request headers</span></span>
| <span data-ttu-id="bb882-121">名称</span><span class="sxs-lookup"><span data-stu-id="bb882-121">Name</span></span>          | <span data-ttu-id="bb882-122">说明</span><span class="sxs-lookup"><span data-stu-id="bb882-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb882-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb882-123">Authorization</span></span> | <span data-ttu-id="bb882-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb882-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb882-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb882-126">Request body</span></span>
<span data-ttu-id="bb882-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb882-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb882-128">响应</span><span class="sxs-lookup"><span data-stu-id="bb882-128">Response</span></span>
<span data-ttu-id="bb882-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bb882-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb882-131">示例</span><span class="sxs-lookup"><span data-stu-id="bb882-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb882-132">请求</span><span class="sxs-lookup"><span data-stu-id="bb882-132">Request</span></span>
<span data-ttu-id="bb882-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb882-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb882-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb882-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="bb882-135">C#</span><span class="sxs-lookup"><span data-stu-id="bb882-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb882-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb882-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb882-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb882-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bb882-138">响应</span><span class="sxs-lookup"><span data-stu-id="bb882-138">Response</span></span>
<span data-ttu-id="bb882-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb882-139">The following is an example of the response.</span></span>
><span data-ttu-id="bb882-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bb882-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
