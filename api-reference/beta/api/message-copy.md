---
title: 'message: copy'
description: 将邮件复制到文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cacc827079089cf977a28f5bb45bb1ac62884275
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934714"
---
# <a name="message-copy"></a><span data-ttu-id="50b8e-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="50b8e-103">message: copy</span></span>

> <span data-ttu-id="50b8e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="50b8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50b8e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="50b8e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50b8e-106">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="50b8e-106">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="50b8e-107">权限</span><span class="sxs-lookup"><span data-stu-id="50b8e-107">Permissions</span></span>

<span data-ttu-id="50b8e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50b8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50b8e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="50b8e-110">Permission type</span></span> | <span data-ttu-id="50b8e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50b8e-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="50b8e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50b8e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50b8e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50b8e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50b8e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50b8e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50b8e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50b8e-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50b8e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="50b8e-116">Application</span></span> | <span data-ttu-id="50b8e-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50b8e-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50b8e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50b8e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="50b8e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50b8e-119">Request headers</span></span>

| <span data-ttu-id="50b8e-120">标头</span><span class="sxs-lookup"><span data-stu-id="50b8e-120">Header</span></span> | <span data-ttu-id="50b8e-121">值</span><span class="sxs-lookup"><span data-stu-id="50b8e-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="50b8e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b8e-122">Authorization</span></span> | <span data-ttu-id="50b8e-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="50b8e-123"></span></span> <span data-ttu-id="50b8e-124">必需。</span><span class="sxs-lookup"><span data-stu-id="50b8e-124">Required.</span></span> |
| <span data-ttu-id="50b8e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50b8e-125">Content-Type</span></span> | <span data-ttu-id="50b8e-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="50b8e-126"></span></span> <span data-ttu-id="50b8e-127">必需。</span><span class="sxs-lookup"><span data-stu-id="50b8e-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50b8e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="50b8e-128">Request body</span></span>

<span data-ttu-id="50b8e-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="50b8e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50b8e-130">参数</span><span class="sxs-lookup"><span data-stu-id="50b8e-130">Parameter</span></span> | <span data-ttu-id="50b8e-131">类型</span><span class="sxs-lookup"><span data-stu-id="50b8e-131">Type</span></span> | <span data-ttu-id="50b8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="50b8e-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="50b8e-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="50b8e-133">destinationId</span></span>|<span data-ttu-id="50b8e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="50b8e-134">String</span></span>|<span data-ttu-id="50b8e-135">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="50b8e-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="50b8e-136">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="50b8e-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="50b8e-137">响应</span><span class="sxs-lookup"><span data-stu-id="50b8e-137">Response</span></span>

<span data-ttu-id="50b8e-138">如果成功，此方法返回`201 Created`响应代码和响应正文的[邮件](../resources/message.md)资源。</span><span class="sxs-lookup"><span data-stu-id="50b8e-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b8e-139">示例</span><span class="sxs-lookup"><span data-stu-id="50b8e-139">Example</span></span>

<span data-ttu-id="50b8e-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="50b8e-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="50b8e-141">请求</span><span class="sxs-lookup"><span data-stu-id="50b8e-141">Request</span></span>

<span data-ttu-id="50b8e-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50b8e-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="50b8e-143">响应</span><span class="sxs-lookup"><span data-stu-id="50b8e-143">Response</span></span>

<span data-ttu-id="50b8e-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="50b8e-144">Here is an example of the response.</span></span>

> <span data-ttu-id="50b8e-145">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="50b8e-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50b8e-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="50b8e-146">All the properties will be returned from an actual call.</span></span>
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
