---
title: 从 printerShare 中删除 allowedGroup
description: 撤销指定组向关联的打印机共享提交打印作业的访问权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: be6d50dad54ac5f9c7995c4dd9b39b49d5b5c1fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777354"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="9b891-103">从 printerShare 中删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="9b891-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="9b891-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b891-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b891-105">撤销指定组向关联的 [printerShare](../resources/printershare.md)提交打印作业的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9b891-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b891-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b891-106">Permissions</span></span>
<span data-ttu-id="9b891-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9b891-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9b891-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="9b891-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="9b891-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="9b891-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b891-111">Permission type</span></span> | <span data-ttu-id="9b891-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b891-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9b891-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b891-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9b891-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b891-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="9b891-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b891-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b891-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b891-116">Not Supported.</span></span>|
|<span data-ttu-id="9b891-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b891-117">Application</span></span>|<span data-ttu-id="9b891-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b891-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b891-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b891-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9b891-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b891-120">Request headers</span></span>
| <span data-ttu-id="9b891-121">名称</span><span class="sxs-lookup"><span data-stu-id="9b891-121">Name</span></span>          | <span data-ttu-id="9b891-122">说明</span><span class="sxs-lookup"><span data-stu-id="9b891-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9b891-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b891-123">Authorization</span></span> | <span data-ttu-id="9b891-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b891-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b891-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b891-126">Request body</span></span>
<span data-ttu-id="9b891-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b891-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b891-128">响应</span><span class="sxs-lookup"><span data-stu-id="9b891-128">Response</span></span>
<span data-ttu-id="9b891-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9b891-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b891-131">示例</span><span class="sxs-lookup"><span data-stu-id="9b891-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b891-132">请求</span><span class="sxs-lookup"><span data-stu-id="9b891-132">Request</span></span>
<span data-ttu-id="9b891-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b891-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b891-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b891-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="9b891-135">C#</span><span class="sxs-lookup"><span data-stu-id="9b891-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-allowedgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b891-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b891-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-allowedgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b891-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b891-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-allowedgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b891-138">Java</span><span class="sxs-lookup"><span data-stu-id="9b891-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-allowedgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b891-139">响应</span><span class="sxs-lookup"><span data-stu-id="9b891-139">Response</span></span>
<span data-ttu-id="9b891-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b891-140">The following is an example of the response.</span></span>
><span data-ttu-id="9b891-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b891-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
