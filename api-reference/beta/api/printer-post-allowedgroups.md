---
title: 创建 allowedGroup
description: 向指定的组授予向关联打印机提交打印作业的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4271d1a621f11ead23347ededf43c1bb4d021714
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947827"
---
# <a name="create-allowedgroup"></a><span data-ttu-id="18fda-103">创建 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="18fda-103">Create allowedGroup</span></span>

<span data-ttu-id="18fda-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18fda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18fda-105">向指定的组授予向关联[打印机](../resources/printer.md)提交**打印作业**的权限。</span><span class="sxs-lookup"><span data-stu-id="18fda-105">Grant the specified group access to submit **print jobs** to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18fda-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="18fda-106">Permissions</span></span>
<span data-ttu-id="18fda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="18fda-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="18fda-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="18fda-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="18fda-110">Permission type</span></span> | <span data-ttu-id="18fda-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18fda-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="18fda-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18fda-112">Delegated (work or school account)</span></span>| <span data-ttu-id="18fda-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="18fda-113">Users.Read.All</span></span> |
|<span data-ttu-id="18fda-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18fda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18fda-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="18fda-115">Not Supported.</span></span>|
|<span data-ttu-id="18fda-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="18fda-116">Application</span></span>|<span data-ttu-id="18fda-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="18fda-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18fda-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18fda-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="18fda-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="18fda-119">Request headers</span></span>
| <span data-ttu-id="18fda-120">名称</span><span class="sxs-lookup"><span data-stu-id="18fda-120">Name</span></span>          | <span data-ttu-id="18fda-121">说明</span><span class="sxs-lookup"><span data-stu-id="18fda-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="18fda-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18fda-122">Authorization</span></span> | <span data-ttu-id="18fda-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18fda-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18fda-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="18fda-125">Content-type</span></span>  | <span data-ttu-id="18fda-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="18fda-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18fda-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="18fda-128">Request body</span></span>
<span data-ttu-id="18fda-129">在请求正文中，通过使用`@odata.id`格式提供对组实体的引用，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="18fda-129">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="18fda-130">响应</span><span class="sxs-lookup"><span data-stu-id="18fda-130">Response</span></span>
<span data-ttu-id="18fda-131">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18fda-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18fda-132">示例</span><span class="sxs-lookup"><span data-stu-id="18fda-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18fda-133">请求</span><span class="sxs-lookup"><span data-stu-id="18fda-133">Request</span></span>
<span data-ttu-id="18fda-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18fda-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18fda-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="18fda-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="18fda-136">C#</span><span class="sxs-lookup"><span data-stu-id="18fda-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18fda-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18fda-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18fda-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18fda-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="18fda-139">在请求正文中，通过在 JSON 正文的`@odata.id`字段中包含组的 MICROSOFT Graph URI，提供对组实体的引用。</span><span class="sxs-lookup"><span data-stu-id="18fda-139">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

##### <a name="response"></a><span data-ttu-id="18fda-140">响应</span><span class="sxs-lookup"><span data-stu-id="18fda-140">Response</span></span>
<span data-ttu-id="18fda-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="18fda-141">The following is an example of the response.</span></span> 
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
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
