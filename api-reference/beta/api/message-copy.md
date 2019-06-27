---
title: 'message: copy'
description: 将邮件复制到文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 54e9811f808e099ba8232f7984fdff85ce342a9c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266092"
---
# <a name="message-copy"></a><span data-ttu-id="c8a9c-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="c8a9c-103">message: copy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8a9c-104">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8a9c-105">权限</span><span class="sxs-lookup"><span data-stu-id="c8a9c-105">Permissions</span></span>

<span data-ttu-id="c8a9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8a9c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8a9c-108">Permission type</span></span> | <span data-ttu-id="c8a9c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8a9c-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c8a9c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8a9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8a9c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8a9c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c8a9c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8a9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8a9c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8a9c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c8a9c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8a9c-114">Application</span></span> | <span data-ttu-id="c8a9c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8a9c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8a9c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8a9c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="c8a9c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8a9c-117">Request headers</span></span>

| <span data-ttu-id="c8a9c-118">标头</span><span class="sxs-lookup"><span data-stu-id="c8a9c-118">Header</span></span> | <span data-ttu-id="c8a9c-119">值</span><span class="sxs-lookup"><span data-stu-id="c8a9c-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c8a9c-120">授权</span><span class="sxs-lookup"><span data-stu-id="c8a9c-120">Authorization</span></span> | <span data-ttu-id="c8a9c-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c8a9c-121"></span></span> <span data-ttu-id="c8a9c-122">必需。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-122">Required.</span></span> |
| <span data-ttu-id="c8a9c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8a9c-123">Content-Type</span></span> | <span data-ttu-id="c8a9c-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c8a9c-124"></span></span> <span data-ttu-id="c8a9c-125">必需。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8a9c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8a9c-126">Request body</span></span>

<span data-ttu-id="c8a9c-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8a9c-128">参数</span><span class="sxs-lookup"><span data-stu-id="c8a9c-128">Parameter</span></span> | <span data-ttu-id="c8a9c-129">类型</span><span class="sxs-lookup"><span data-stu-id="c8a9c-129">Type</span></span> | <span data-ttu-id="c8a9c-130">说明</span><span class="sxs-lookup"><span data-stu-id="c8a9c-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c8a9c-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="c8a9c-131">destinationId</span></span>|<span data-ttu-id="c8a9c-132">String</span><span class="sxs-lookup"><span data-stu-id="c8a9c-132">String</span></span>|<span data-ttu-id="c8a9c-133">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c8a9c-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="c8a9c-135">响应</span><span class="sxs-lookup"><span data-stu-id="c8a9c-135">Response</span></span>

<span data-ttu-id="c8a9c-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8a9c-137">示例</span><span class="sxs-lookup"><span data-stu-id="c8a9c-137">Example</span></span>

<span data-ttu-id="c8a9c-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c8a9c-139">请求</span><span class="sxs-lookup"><span data-stu-id="c8a9c-139">Request</span></span>

<span data-ttu-id="c8a9c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c8a9c-141">响应</span><span class="sxs-lookup"><span data-stu-id="c8a9c-141">Response</span></span>

<span data-ttu-id="c8a9c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-142">Here is an example of the response.</span></span>

> <span data-ttu-id="c8a9c-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c8a9c-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8a9c-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c8a9c-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c8a9c-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c8a9c-146">C#</span><span class="sxs-lookup"><span data-stu-id="c8a9c-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_copy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8a9c-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8a9c-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_copy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c8a9c-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="c8a9c-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_copy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
