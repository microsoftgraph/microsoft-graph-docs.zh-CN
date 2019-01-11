---
title: 删除照片
description: 删除照片。
localization_priority: Normal
ms.openlocfilehash: 117f4acbf5a45d9db64ccc5d3fc0ccc4d1c64896
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829258"
---
# <a name="delete-photo"></a><span data-ttu-id="8c3db-103">删除照片</span><span class="sxs-lookup"><span data-stu-id="8c3db-103">Delete photo</span></span>

> <span data-ttu-id="8c3db-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8c3db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c3db-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8c3db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c3db-106">删除照片。</span><span class="sxs-lookup"><span data-stu-id="8c3db-106">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c3db-107">权限</span><span class="sxs-lookup"><span data-stu-id="8c3db-107">Permissions</span></span>
<span data-ttu-id="8c3db-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c3db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c3db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c3db-110">Permission type</span></span>      | <span data-ttu-id="8c3db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c3db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c3db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c3db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c3db-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c3db-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c3db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c3db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c3db-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c3db-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c3db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c3db-116">Application</span></span> | <span data-ttu-id="8c3db-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c3db-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c3db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c3db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="8c3db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c3db-119">Request headers</span></span>
| <span data-ttu-id="8c3db-120">名称</span><span class="sxs-lookup"><span data-stu-id="8c3db-120">Name</span></span>       | <span data-ttu-id="8c3db-121">类型</span><span class="sxs-lookup"><span data-stu-id="8c3db-121">Type</span></span> | <span data-ttu-id="8c3db-122">说明</span><span class="sxs-lookup"><span data-stu-id="8c3db-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c3db-123">if-match</span><span class="sxs-lookup"><span data-stu-id="8c3db-123">if-match</span></span>  | <span data-ttu-id="8c3db-124">string</span><span class="sxs-lookup"><span data-stu-id="8c3db-124">string</span></span>  | <span data-ttu-id="8c3db-125">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="8c3db-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="8c3db-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c3db-126">Authorization</span></span>  | <span data-ttu-id="8c3db-127">string</span><span class="sxs-lookup"><span data-stu-id="8c3db-127">string</span></span>  | <span data-ttu-id="8c3db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c3db-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c3db-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c3db-130">Request body</span></span>
<span data-ttu-id="8c3db-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c3db-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c3db-132">响应</span><span class="sxs-lookup"><span data-stu-id="8c3db-132">Response</span></span>

<span data-ttu-id="8c3db-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8c3db-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c3db-135">示例</span><span class="sxs-lookup"><span data-stu-id="8c3db-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c3db-136">请求</span><span class="sxs-lookup"><span data-stu-id="8c3db-136">Request</span></span>
<span data-ttu-id="8c3db-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c3db-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="8c3db-138">响应</span><span class="sxs-lookup"><span data-stu-id="8c3db-138">Response</span></span>
<span data-ttu-id="8c3db-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8c3db-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
