---
title: 删除连接器
description: 删除 () 连接器中注销。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2025816bb917e84f8a0cce7ef6af0214516850bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035910"
---
# <a name="delete-connector"></a><span data-ttu-id="1bc1b-103">删除连接器</span><span class="sxs-lookup"><span data-stu-id="1bc1b-103">Delete connector</span></span>

<span data-ttu-id="1bc1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc1b-105">删除 (注销) **printConnector**。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bc1b-106">权限</span><span class="sxs-lookup"><span data-stu-id="1bc1b-106">Permissions</span></span>
<span data-ttu-id="1bc1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1bc1b-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="1bc1b-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1bc1b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bc1b-111">Permission type</span></span> | <span data-ttu-id="1bc1b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bc1b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1bc1b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bc1b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1bc1b-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="1bc1b-114">User.Read</span></span> |
|<span data-ttu-id="1bc1b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bc1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bc1b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-116">Not Supported.</span></span>|
|<span data-ttu-id="1bc1b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bc1b-117">Application</span></span>|<span data-ttu-id="1bc1b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bc1b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bc1b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1bc1b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bc1b-120">Request headers</span></span>
| <span data-ttu-id="1bc1b-121">名称</span><span class="sxs-lookup"><span data-stu-id="1bc1b-121">Name</span></span>          | <span data-ttu-id="1bc1b-122">说明</span><span class="sxs-lookup"><span data-stu-id="1bc1b-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1bc1b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc1b-123">Authorization</span></span> | <span data-ttu-id="1bc1b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bc1b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bc1b-126">Request body</span></span>
<span data-ttu-id="1bc1b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bc1b-128">响应</span><span class="sxs-lookup"><span data-stu-id="1bc1b-128">Response</span></span>
<span data-ttu-id="1bc1b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="1bc1b-131">错误条件和消息</span><span class="sxs-lookup"><span data-stu-id="1bc1b-131">Error conditions and messages</span></span>

|<span data-ttu-id="1bc1b-132">方案</span><span class="sxs-lookup"><span data-stu-id="1bc1b-132">Scenario</span></span>|<span data-ttu-id="1bc1b-133">方法</span><span class="sxs-lookup"><span data-stu-id="1bc1b-133">Method</span></span>|<span data-ttu-id="1bc1b-134">代码</span><span class="sxs-lookup"><span data-stu-id="1bc1b-134">Code</span></span>|<span data-ttu-id="1bc1b-135">消息</span><span class="sxs-lookup"><span data-stu-id="1bc1b-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="1bc1b-136">用户尝试删除已注册的一个或多个打印机的连接器</span><span class="sxs-lookup"><span data-stu-id="1bc1b-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="1bc1b-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="1bc1b-137">DELETE</span></span>|<span data-ttu-id="1bc1b-138">409</span><span class="sxs-lookup"><span data-stu-id="1bc1b-138">409</span></span>|<span data-ttu-id="1bc1b-139">在删除连接器之前，请注销关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="1bc1b-140">示例</span><span class="sxs-lookup"><span data-stu-id="1bc1b-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bc1b-141">请求</span><span class="sxs-lookup"><span data-stu-id="1bc1b-141">Request</span></span>
<span data-ttu-id="1bc1b-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bc1b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bc1b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="1bc1b-144">C#</span><span class="sxs-lookup"><span data-stu-id="1bc1b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bc1b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bc1b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bc1b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bc1b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1bc1b-147">响应</span><span class="sxs-lookup"><span data-stu-id="1bc1b-147">Response</span></span>
<span data-ttu-id="1bc1b-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-148">The following is an example of the response.</span></span>
><span data-ttu-id="1bc1b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1bc1b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


