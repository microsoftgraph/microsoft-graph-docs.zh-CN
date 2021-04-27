---
title: 删除连接器
description: 删除 (注销) 连接器。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 99a8a4d0da5f3abb4beccfc1a196b8567f690303
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053613"
---
# <a name="delete-connector"></a><span data-ttu-id="9a385-103">删除连接器</span><span class="sxs-lookup"><span data-stu-id="9a385-103">Delete connector</span></span>

<span data-ttu-id="9a385-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a385-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a385-105">删除 (注销) **printConnector**。</span><span class="sxs-lookup"><span data-stu-id="9a385-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a385-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a385-106">Permissions</span></span>
<span data-ttu-id="9a385-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9a385-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9a385-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="9a385-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="9a385-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="9a385-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a385-111">Permission type</span></span> | <span data-ttu-id="9a385-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a385-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9a385-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a385-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9a385-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a385-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="9a385-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a385-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a385-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a385-116">Not Supported.</span></span>|
|<span data-ttu-id="9a385-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a385-117">Application</span></span>|<span data-ttu-id="9a385-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a385-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a385-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a385-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9a385-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a385-120">Request headers</span></span>
| <span data-ttu-id="9a385-121">名称</span><span class="sxs-lookup"><span data-stu-id="9a385-121">Name</span></span>          | <span data-ttu-id="9a385-122">说明</span><span class="sxs-lookup"><span data-stu-id="9a385-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9a385-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a385-123">Authorization</span></span> | <span data-ttu-id="9a385-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a385-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a385-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a385-126">Request body</span></span>
<span data-ttu-id="9a385-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a385-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a385-128">响应</span><span class="sxs-lookup"><span data-stu-id="9a385-128">Response</span></span>
<span data-ttu-id="9a385-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9a385-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="9a385-131">错误条件和消息</span><span class="sxs-lookup"><span data-stu-id="9a385-131">Error conditions and messages</span></span>

|<span data-ttu-id="9a385-132">方案</span><span class="sxs-lookup"><span data-stu-id="9a385-132">Scenario</span></span>|<span data-ttu-id="9a385-133">方法</span><span class="sxs-lookup"><span data-stu-id="9a385-133">Method</span></span>|<span data-ttu-id="9a385-134">代码</span><span class="sxs-lookup"><span data-stu-id="9a385-134">Code</span></span>|<span data-ttu-id="9a385-135">消息</span><span class="sxs-lookup"><span data-stu-id="9a385-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="9a385-136">用户尝试删除已注册一个或多个打印机的连接器</span><span class="sxs-lookup"><span data-stu-id="9a385-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="9a385-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="9a385-137">DELETE</span></span>|<span data-ttu-id="9a385-138">409</span><span class="sxs-lookup"><span data-stu-id="9a385-138">409</span></span>|<span data-ttu-id="9a385-139">删除连接器之前，请注销关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="9a385-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="9a385-140">示例</span><span class="sxs-lookup"><span data-stu-id="9a385-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a385-141">请求</span><span class="sxs-lookup"><span data-stu-id="9a385-141">Request</span></span>
<span data-ttu-id="9a385-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a385-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a385-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a385-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a385-144">C#</span><span class="sxs-lookup"><span data-stu-id="9a385-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a385-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a385-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a385-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a385-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a385-147">Java</span><span class="sxs-lookup"><span data-stu-id="9a385-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a385-148">响应</span><span class="sxs-lookup"><span data-stu-id="9a385-148">Response</span></span>
<span data-ttu-id="9a385-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a385-149">The following is an example of the response.</span></span>
><span data-ttu-id="9a385-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a385-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
