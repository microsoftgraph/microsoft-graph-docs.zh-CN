---
title: 创建 allowedGroup
description: 向指定的组授予向关联打印机提交打印作业的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 22512c6de88d85c09c0924fbc66eef9b760c6ce0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216803"
---
# <a name="create-allowedgroup"></a><span data-ttu-id="85f26-103">创建 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="85f26-103">Create allowedGroup</span></span>

<span data-ttu-id="85f26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85f26-105">向指定的组授予将打印作业提交到关联的[printerShare](../resources/printershare.md)的权限。</span><span class="sxs-lookup"><span data-stu-id="85f26-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85f26-106">权限</span><span class="sxs-lookup"><span data-stu-id="85f26-106">Permissions</span></span>
<span data-ttu-id="85f26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="85f26-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="85f26-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="85f26-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="85f26-110">Permission type</span></span> | <span data-ttu-id="85f26-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85f26-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="85f26-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85f26-112">Delegated (work or school account)</span></span>| <span data-ttu-id="85f26-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="85f26-113">Users.Read.All</span></span> |
|<span data-ttu-id="85f26-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85f26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85f26-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="85f26-115">Not Supported.</span></span>|
|<span data-ttu-id="85f26-116">Application</span><span class="sxs-lookup"><span data-stu-id="85f26-116">Application</span></span>|<span data-ttu-id="85f26-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="85f26-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85f26-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85f26-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="85f26-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="85f26-119">Request headers</span></span>
| <span data-ttu-id="85f26-120">名称</span><span class="sxs-lookup"><span data-stu-id="85f26-120">Name</span></span>          | <span data-ttu-id="85f26-121">说明</span><span class="sxs-lookup"><span data-stu-id="85f26-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85f26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85f26-122">Authorization</span></span> | <span data-ttu-id="85f26-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85f26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85f26-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="85f26-125">Content-type</span></span>  | <span data-ttu-id="85f26-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="85f26-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85f26-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="85f26-128">Request body</span></span>
<span data-ttu-id="85f26-129">在请求正文中，通过使用格式提供对组实体的引用 `@odata.id` ，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="85f26-129">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="85f26-130">响应</span><span class="sxs-lookup"><span data-stu-id="85f26-130">Response</span></span>
<span data-ttu-id="85f26-131">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85f26-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85f26-132">示例</span><span class="sxs-lookup"><span data-stu-id="85f26-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="85f26-133">请求</span><span class="sxs-lookup"><span data-stu-id="85f26-133">Request</span></span>
<span data-ttu-id="85f26-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="85f26-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="85f26-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="85f26-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="85f26-136">C#</span><span class="sxs-lookup"><span data-stu-id="85f26-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85f26-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85f26-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85f26-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85f26-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="85f26-139">在请求正文中，通过在 JSON 正文的字段中包含组的 Microsoft Graph URI，提供对组实体的引用 `@odata.id` 。</span><span class="sxs-lookup"><span data-stu-id="85f26-139">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="85f26-140">响应</span><span class="sxs-lookup"><span data-stu-id="85f26-140">Response</span></span>
<span data-ttu-id="85f26-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85f26-141">The following is an example of the response.</span></span> 
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
