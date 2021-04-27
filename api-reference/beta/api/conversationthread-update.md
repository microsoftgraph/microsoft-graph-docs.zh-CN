---
title: 更新 conversationthread
description: 锁定或解除锁定线程，以允许或避免进一步向线程发布。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e7948c9f988e7d829f6a49292b0b09ba1f7eda52
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047005"
---
# <a name="update-conversationthread"></a><span data-ttu-id="29413-103">更新 conversationthread</span><span class="sxs-lookup"><span data-stu-id="29413-103">Update conversationthread</span></span>

<span data-ttu-id="29413-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29413-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29413-105">锁定或解除锁定线程，以允许或避免进一步向线程发布。</span><span class="sxs-lookup"><span data-stu-id="29413-105">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="29413-106">权限</span><span class="sxs-lookup"><span data-stu-id="29413-106">Permissions</span></span>
<span data-ttu-id="29413-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29413-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="29413-109">Permission type</span></span>      | <span data-ttu-id="29413-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29413-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29413-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29413-111">Delegated (work or school account)</span></span> | <span data-ttu-id="29413-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29413-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="29413-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29413-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29413-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29413-114">Not supported.</span></span>    |
|<span data-ttu-id="29413-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="29413-115">Application</span></span> | <span data-ttu-id="29413-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29413-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29413-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29413-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="29413-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="29413-118">Request headers</span></span>
| <span data-ttu-id="29413-119">标头</span><span class="sxs-lookup"><span data-stu-id="29413-119">Header</span></span>       | <span data-ttu-id="29413-120">值</span><span class="sxs-lookup"><span data-stu-id="29413-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29413-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="29413-121">Authorization</span></span>  | <span data-ttu-id="29413-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29413-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29413-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29413-124">Content-Type</span></span>  | <span data-ttu-id="29413-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="29413-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29413-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29413-127">Request body</span></span>
<span data-ttu-id="29413-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="29413-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="29413-131">属性</span><span class="sxs-lookup"><span data-stu-id="29413-131">Property</span></span>     | <span data-ttu-id="29413-132">类型</span><span class="sxs-lookup"><span data-stu-id="29413-132">Type</span></span>   |<span data-ttu-id="29413-133">说明</span><span class="sxs-lookup"><span data-stu-id="29413-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29413-134">isLocked</span><span class="sxs-lookup"><span data-stu-id="29413-134">isLocked</span></span>|<span data-ttu-id="29413-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="29413-135">Boolean</span></span>|<span data-ttu-id="29413-p105">指示线程是否已锁定。设置为 `true` 以禁止发布。</span><span class="sxs-lookup"><span data-stu-id="29413-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="29413-138">响应</span><span class="sxs-lookup"><span data-stu-id="29413-138">Response</span></span>

<span data-ttu-id="29413-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29413-139">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29413-140">示例</span><span class="sxs-lookup"><span data-stu-id="29413-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29413-141">请求</span><span class="sxs-lookup"><span data-stu-id="29413-141">Request</span></span>
<span data-ttu-id="29413-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29413-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29413-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="29413-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
# <a name="c"></a>[<span data-ttu-id="29413-144">C#</span><span class="sxs-lookup"><span data-stu-id="29413-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29413-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29413-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29413-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29413-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29413-147">Java</span><span class="sxs-lookup"><span data-stu-id="29413-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="29413-148">响应</span><span class="sxs-lookup"><span data-stu-id="29413-148">Response</span></span>
<span data-ttu-id="29413-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="29413-149">Here is an example of the response.</span></span> <span data-ttu-id="29413-150">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="29413-150">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


