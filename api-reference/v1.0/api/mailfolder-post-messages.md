---
title: 创建邮件
description: 使用此 API 在 mailfolder 中新建邮件。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 18c72dc42d2ced2f1aaee5819598da1e28a5c8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848270"
---
# <a name="create-message"></a><span data-ttu-id="a677c-103">创建邮件</span><span class="sxs-lookup"><span data-stu-id="a677c-103">Create Message</span></span>

<span data-ttu-id="a677c-104">使用此 API 在 mailfolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="a677c-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a677c-105">权限</span><span class="sxs-lookup"><span data-stu-id="a677c-105">Permissions</span></span>
<span data-ttu-id="a677c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a677c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a677c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a677c-108">Permission type</span></span>      | <span data-ttu-id="a677c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a677c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a677c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a677c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a677c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a677c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a677c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a677c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a677c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a677c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a677c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a677c-114">Application</span></span> | <span data-ttu-id="a677c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a677c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a677c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a677c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="a677c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a677c-117">Request headers</span></span>
| <span data-ttu-id="a677c-118">标头</span><span class="sxs-lookup"><span data-stu-id="a677c-118">Header</span></span>       | <span data-ttu-id="a677c-119">值</span><span class="sxs-lookup"><span data-stu-id="a677c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a677c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a677c-120">Authorization</span></span>  | <span data-ttu-id="a677c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a677c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a677c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a677c-123">Content-Type</span></span>  | <span data-ttu-id="a677c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a677c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a677c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a677c-126">Request body</span></span>
<span data-ttu-id="a677c-127">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a677c-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a677c-128">响应</span><span class="sxs-lookup"><span data-stu-id="a677c-128">Response</span></span>

<span data-ttu-id="a677c-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a677c-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a677c-130">示例</span><span class="sxs-lookup"><span data-stu-id="a677c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a677c-131">请求</span><span class="sxs-lookup"><span data-stu-id="a677c-131">Request</span></span>
<span data-ttu-id="a677c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a677c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
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
<span data-ttu-id="a677c-133">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a677c-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a677c-134">响应</span><span class="sxs-lookup"><span data-stu-id="a677c-134">Response</span></span>
<span data-ttu-id="a677c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a677c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
