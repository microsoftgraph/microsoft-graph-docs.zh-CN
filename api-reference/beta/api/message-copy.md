---
title: 'message: copy'
description: 将邮件复制到文件夹。
ms.openlocfilehash: c0c5428ff2f661d865a6cb2cd17bc0a48e177a52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043718"
---
# <a name="message-copy"></a><span data-ttu-id="e10b8-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="e10b8-103">message: copy</span></span>

> <span data-ttu-id="e10b8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e10b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e10b8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e10b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e10b8-106">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="e10b8-106">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e10b8-107">权限</span><span class="sxs-lookup"><span data-stu-id="e10b8-107">Permissions</span></span>

<span data-ttu-id="e10b8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e10b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e10b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e10b8-110">Permission type</span></span> | <span data-ttu-id="e10b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e10b8-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="e10b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e10b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e10b8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e10b8-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e10b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e10b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e10b8-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e10b8-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e10b8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e10b8-116">Application</span></span> | <span data-ttu-id="e10b8-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e10b8-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e10b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e10b8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="e10b8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e10b8-119">Request headers</span></span>

| <span data-ttu-id="e10b8-120">标头</span><span class="sxs-lookup"><span data-stu-id="e10b8-120">Header</span></span> | <span data-ttu-id="e10b8-121">值</span><span class="sxs-lookup"><span data-stu-id="e10b8-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="e10b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e10b8-122">Authorization</span></span> | <span data-ttu-id="e10b8-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="e10b8-123"></span></span> <span data-ttu-id="e10b8-124">必需。</span><span class="sxs-lookup"><span data-stu-id="e10b8-124">Required.</span></span> |
| <span data-ttu-id="e10b8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e10b8-125">Content-Type</span></span> | <span data-ttu-id="e10b8-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="e10b8-126"></span></span> <span data-ttu-id="e10b8-127">必需。</span><span class="sxs-lookup"><span data-stu-id="e10b8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e10b8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e10b8-128">Request body</span></span>

<span data-ttu-id="e10b8-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e10b8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e10b8-130">参数</span><span class="sxs-lookup"><span data-stu-id="e10b8-130">Parameter</span></span> | <span data-ttu-id="e10b8-131">类型</span><span class="sxs-lookup"><span data-stu-id="e10b8-131">Type</span></span> | <span data-ttu-id="e10b8-132">说明</span><span class="sxs-lookup"><span data-stu-id="e10b8-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="e10b8-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="e10b8-133">destinationId</span></span>|<span data-ttu-id="e10b8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e10b8-134">String</span></span>|<span data-ttu-id="e10b8-135">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="e10b8-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="e10b8-136">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="e10b8-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e10b8-137">响应</span><span class="sxs-lookup"><span data-stu-id="e10b8-137">Response</span></span>

<span data-ttu-id="e10b8-138">如果成功，此方法返回`201 Created`响应代码和响应正文的[邮件](../resources/message.md)资源。</span><span class="sxs-lookup"><span data-stu-id="e10b8-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e10b8-139">示例</span><span class="sxs-lookup"><span data-stu-id="e10b8-139">Example</span></span>

<span data-ttu-id="e10b8-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e10b8-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e10b8-141">请求</span><span class="sxs-lookup"><span data-stu-id="e10b8-141">Request</span></span>

<span data-ttu-id="e10b8-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e10b8-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e10b8-143">响应</span><span class="sxs-lookup"><span data-stu-id="e10b8-143">Response</span></span>

<span data-ttu-id="e10b8-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e10b8-144">Here is an example of the response.</span></span>

> <span data-ttu-id="e10b8-145">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e10b8-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e10b8-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e10b8-146">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
