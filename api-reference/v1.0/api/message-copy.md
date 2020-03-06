---
title: 'message: copy'
description: 将邮件复制到文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 70ef296ae46b868c7980546462cc0ba37c793e60
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511570"
---
# <a name="message-copy"></a><span data-ttu-id="882a5-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="882a5-103">message: copy</span></span>

<span data-ttu-id="882a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="882a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="882a5-105">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="882a5-105">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="882a5-106">权限</span><span class="sxs-lookup"><span data-stu-id="882a5-106">Permissions</span></span>

<span data-ttu-id="882a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="882a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="882a5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="882a5-109">Permission type</span></span> | <span data-ttu-id="882a5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="882a5-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="882a5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="882a5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="882a5-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="882a5-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="882a5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="882a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="882a5-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="882a5-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="882a5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="882a5-115">Application</span></span> | <span data-ttu-id="882a5-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="882a5-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="882a5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="882a5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="882a5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="882a5-118">Request headers</span></span>

| <span data-ttu-id="882a5-119">标头</span><span class="sxs-lookup"><span data-stu-id="882a5-119">Header</span></span> | <span data-ttu-id="882a5-120">值</span><span class="sxs-lookup"><span data-stu-id="882a5-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="882a5-121">授权</span><span class="sxs-lookup"><span data-stu-id="882a5-121">Authorization</span></span> | <span data-ttu-id="882a5-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="882a5-122">`Bearer {token}`.</span></span> <span data-ttu-id="882a5-123">必需。</span><span class="sxs-lookup"><span data-stu-id="882a5-123">Required.</span></span> |
| <span data-ttu-id="882a5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="882a5-124">Content-Type</span></span> | <span data-ttu-id="882a5-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="882a5-125">`application/json`.</span></span> <span data-ttu-id="882a5-126">必需。</span><span class="sxs-lookup"><span data-stu-id="882a5-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="882a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="882a5-127">Request body</span></span>

<span data-ttu-id="882a5-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="882a5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="882a5-129">参数</span><span class="sxs-lookup"><span data-stu-id="882a5-129">Parameter</span></span> | <span data-ttu-id="882a5-130">类型</span><span class="sxs-lookup"><span data-stu-id="882a5-130">Type</span></span> | <span data-ttu-id="882a5-131">说明</span><span class="sxs-lookup"><span data-stu-id="882a5-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="882a5-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="882a5-132">destinationId</span></span>|<span data-ttu-id="882a5-133">String</span><span class="sxs-lookup"><span data-stu-id="882a5-133">String</span></span>|<span data-ttu-id="882a5-134">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="882a5-134">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="882a5-135">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="882a5-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="882a5-136">响应</span><span class="sxs-lookup"><span data-stu-id="882a5-136">Response</span></span>

<span data-ttu-id="882a5-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="882a5-137">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="882a5-138">示例</span><span class="sxs-lookup"><span data-stu-id="882a5-138">Example</span></span>

<span data-ttu-id="882a5-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="882a5-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="882a5-140">请求</span><span class="sxs-lookup"><span data-stu-id="882a5-140">Request</span></span>
<span data-ttu-id="882a5-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="882a5-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="882a5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="882a5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="882a5-143">C#</span><span class="sxs-lookup"><span data-stu-id="882a5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="882a5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="882a5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="882a5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="882a5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="882a5-146">Java</span><span class="sxs-lookup"><span data-stu-id="882a5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="882a5-147">响应</span><span class="sxs-lookup"><span data-stu-id="882a5-147">Response</span></span>

<span data-ttu-id="882a5-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="882a5-148">Here is an example of the response.</span></span>

> <span data-ttu-id="882a5-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="882a5-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="882a5-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="882a5-150">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
