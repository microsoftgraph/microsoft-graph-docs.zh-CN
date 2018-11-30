---
title: 删除 Outlook 类别
description: 删除指定的 outlookCategory 对象。
ms.openlocfilehash: a240df167918892face0da8932af0f2ff3d23152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043331"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="23ae9-103">删除 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="23ae9-103">Delete Outlook category</span></span>

> <span data-ttu-id="23ae9-104">**重要说明**： 在 Microsoft Graph 中的 /beta 版本下的 Api 在预览，并会受到更改。</span><span class="sxs-lookup"><span data-stu-id="23ae9-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23ae9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23ae9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23ae9-106">删除指定的 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23ae9-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23ae9-107">权限</span><span class="sxs-lookup"><span data-stu-id="23ae9-107">Permissions</span></span>
<span data-ttu-id="23ae9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23ae9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ae9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="23ae9-110">Permission type</span></span>      | <span data-ttu-id="23ae9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23ae9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23ae9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23ae9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23ae9-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ae9-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="23ae9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23ae9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ae9-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ae9-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="23ae9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="23ae9-116">Application</span></span> | <span data-ttu-id="23ae9-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ae9-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23ae9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23ae9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23ae9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23ae9-119">Optional query parameters</span></span>
<span data-ttu-id="23ae9-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23ae9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23ae9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="23ae9-121">Request headers</span></span>
| <span data-ttu-id="23ae9-122">名称</span><span class="sxs-lookup"><span data-stu-id="23ae9-122">Name</span></span>      |<span data-ttu-id="23ae9-123">说明</span><span class="sxs-lookup"><span data-stu-id="23ae9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23ae9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="23ae9-124">Authorization</span></span>  | <span data-ttu-id="23ae9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23ae9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23ae9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="23ae9-127">Request body</span></span>
<span data-ttu-id="23ae9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23ae9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23ae9-129">响应</span><span class="sxs-lookup"><span data-stu-id="23ae9-129">Response</span></span>

<span data-ttu-id="23ae9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="23ae9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ae9-132">示例</span><span class="sxs-lookup"><span data-stu-id="23ae9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23ae9-133">请求</span><span class="sxs-lookup"><span data-stu-id="23ae9-133">Request</span></span>
<span data-ttu-id="23ae9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23ae9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="23ae9-135">响应</span><span class="sxs-lookup"><span data-stu-id="23ae9-135">Response</span></span>
<span data-ttu-id="23ae9-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="23ae9-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->