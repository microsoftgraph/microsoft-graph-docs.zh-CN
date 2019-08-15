---
title: 'message: copy'
description: 将邮件复制到文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: af764779525de08157c7adb604eb713f7676a0e7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415153"
---
# <a name="message-copy"></a><span data-ttu-id="b225d-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="b225d-103">message: copy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b225d-104">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="b225d-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b225d-105">权限</span><span class="sxs-lookup"><span data-stu-id="b225d-105">Permissions</span></span>

<span data-ttu-id="b225d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b225d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b225d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b225d-108">Permission type</span></span> | <span data-ttu-id="b225d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b225d-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="b225d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b225d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b225d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b225d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b225d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b225d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b225d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b225d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b225d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b225d-114">Application</span></span> | <span data-ttu-id="b225d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b225d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b225d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b225d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="b225d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b225d-117">Request headers</span></span>

| <span data-ttu-id="b225d-118">标头</span><span class="sxs-lookup"><span data-stu-id="b225d-118">Header</span></span> | <span data-ttu-id="b225d-119">值</span><span class="sxs-lookup"><span data-stu-id="b225d-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="b225d-120">授权</span><span class="sxs-lookup"><span data-stu-id="b225d-120">Authorization</span></span> | <span data-ttu-id="b225d-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="b225d-121"></span></span> <span data-ttu-id="b225d-122">必需。</span><span class="sxs-lookup"><span data-stu-id="b225d-122">Required.</span></span> |
| <span data-ttu-id="b225d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b225d-123">Content-Type</span></span> | <span data-ttu-id="b225d-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="b225d-124"></span></span> <span data-ttu-id="b225d-125">必需。</span><span class="sxs-lookup"><span data-stu-id="b225d-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b225d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b225d-126">Request body</span></span>

<span data-ttu-id="b225d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b225d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b225d-128">参数</span><span class="sxs-lookup"><span data-stu-id="b225d-128">Parameter</span></span> | <span data-ttu-id="b225d-129">类型</span><span class="sxs-lookup"><span data-stu-id="b225d-129">Type</span></span> | <span data-ttu-id="b225d-130">说明</span><span class="sxs-lookup"><span data-stu-id="b225d-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="b225d-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="b225d-131">destinationId</span></span>|<span data-ttu-id="b225d-132">String</span><span class="sxs-lookup"><span data-stu-id="b225d-132">String</span></span>|<span data-ttu-id="b225d-133">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="b225d-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="b225d-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="b225d-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="b225d-135">响应</span><span class="sxs-lookup"><span data-stu-id="b225d-135">Response</span></span>

<span data-ttu-id="b225d-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="b225d-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b225d-137">示例</span><span class="sxs-lookup"><span data-stu-id="b225d-137">Example</span></span>

<span data-ttu-id="b225d-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b225d-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b225d-139">请求</span><span class="sxs-lookup"><span data-stu-id="b225d-139">Request</span></span>

<span data-ttu-id="b225d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b225d-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b225d-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b225d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b225d-142">C#</span><span class="sxs-lookup"><span data-stu-id="b225d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b225d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b225d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b225d-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="b225d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b225d-145">响应</span><span class="sxs-lookup"><span data-stu-id="b225d-145">Response</span></span>

<span data-ttu-id="b225d-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b225d-146">Here is an example of the response.</span></span>

> <span data-ttu-id="b225d-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b225d-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b225d-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b225d-148">All the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
