---
title: 创建 allowedUser
description: 向指定的用户授予向关联打印机提交打印作业的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5ce2564b2878a3dff998c938366f132c08098a73
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947799"
---
# <a name="create-alloweduser"></a><span data-ttu-id="4ae2e-103">创建 allowedUser</span><span class="sxs-lookup"><span data-stu-id="4ae2e-103">Create allowedUser</span></span>

<span data-ttu-id="4ae2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ae2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae2e-105">向指定的用户授予向关联[打印机](../resources/printer.md)提交**打印作业**的权限。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-105">Grant the specified user access to submit **print jobs** to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ae2e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ae2e-106">Permissions</span></span>
<span data-ttu-id="4ae2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ae2e-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4ae2e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ae2e-110">Permission type</span></span> | <span data-ttu-id="4ae2e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ae2e-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4ae2e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae2e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4ae2e-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="4ae2e-113">Users.Read.All</span></span> |
|<span data-ttu-id="4ae2e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ae2e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-115">Not Supported.</span></span>|
|<span data-ttu-id="4ae2e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ae2e-116">Application</span></span>|<span data-ttu-id="4ae2e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ae2e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ae2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/allowedUsers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4ae2e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ae2e-119">Request headers</span></span>
| <span data-ttu-id="4ae2e-120">名称</span><span class="sxs-lookup"><span data-stu-id="4ae2e-120">Name</span></span>          | <span data-ttu-id="4ae2e-121">说明</span><span class="sxs-lookup"><span data-stu-id="4ae2e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4ae2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae2e-122">Authorization</span></span> | <span data-ttu-id="4ae2e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ae2e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4ae2e-125">Content-type</span></span>  | <span data-ttu-id="4ae2e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4ae2e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae2e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ae2e-128">Request body</span></span>
<span data-ttu-id="4ae2e-129">在请求正文中，通过使用`@odata.id`格式提供对用户实体的引用，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-129">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="4ae2e-130">响应</span><span class="sxs-lookup"><span data-stu-id="4ae2e-130">Response</span></span>
<span data-ttu-id="4ae2e-131">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ae2e-132">示例</span><span class="sxs-lookup"><span data-stu-id="4ae2e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ae2e-133">请求</span><span class="sxs-lookup"><span data-stu-id="4ae2e-133">Request</span></span>
<span data-ttu-id="4ae2e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ae2e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ae2e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_alloweduser_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers/$ref
Content-type: application/json
Content-length: 66

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="4ae2e-136">C#</span><span class="sxs-lookup"><span data-stu-id="4ae2e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-alloweduser-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ae2e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ae2e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-alloweduser-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ae2e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ae2e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-alloweduser-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4ae2e-139">在请求正文中，通过在 JSON 正文的`@odata.id`字段中添加用户的 MICROSOFT Graph URI，提供对用户实体的引用。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-139">In the request body, supply a reference to a user entity by including the user's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

##### <a name="response"></a><span data-ttu-id="4ae2e-140">响应</span><span class="sxs-lookup"><span data-stu-id="4ae2e-140">Response</span></span>
<span data-ttu-id="4ae2e-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ae2e-141">The following is an example of the response.</span></span> 
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
  "description": "Create allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
