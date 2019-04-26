---
title: 更新 conversationthread
description: 锁定或解除锁定线程，以允许或避免进一步向线程发布。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e4a2fbeb8e92271294ffa9e3fb065a9d9ae64649
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326120"
---
# <a name="update-conversationthread"></a><span data-ttu-id="9188b-103">更新 conversationthread</span><span class="sxs-lookup"><span data-stu-id="9188b-103">Update conversationthread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9188b-104">锁定或解除锁定线程，以允许或避免进一步向线程发布。</span><span class="sxs-lookup"><span data-stu-id="9188b-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="9188b-105">权限</span><span class="sxs-lookup"><span data-stu-id="9188b-105">Permissions</span></span>
<span data-ttu-id="9188b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9188b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9188b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9188b-108">Permission type</span></span>      | <span data-ttu-id="9188b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9188b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9188b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9188b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9188b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9188b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9188b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9188b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9188b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9188b-113">Not supported.</span></span>    |
|<span data-ttu-id="9188b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9188b-114">Application</span></span> | <span data-ttu-id="9188b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9188b-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9188b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9188b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9188b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9188b-117">Request headers</span></span>
| <span data-ttu-id="9188b-118">标头</span><span class="sxs-lookup"><span data-stu-id="9188b-118">Header</span></span>       | <span data-ttu-id="9188b-119">值</span><span class="sxs-lookup"><span data-stu-id="9188b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9188b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9188b-120">Authorization</span></span>  | <span data-ttu-id="9188b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9188b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9188b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9188b-123">Content-Type</span></span>  | <span data-ttu-id="9188b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9188b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9188b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9188b-126">Request body</span></span>
<span data-ttu-id="9188b-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9188b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9188b-130">属性</span><span class="sxs-lookup"><span data-stu-id="9188b-130">Property</span></span>     | <span data-ttu-id="9188b-131">类型</span><span class="sxs-lookup"><span data-stu-id="9188b-131">Type</span></span>   |<span data-ttu-id="9188b-132">说明</span><span class="sxs-lookup"><span data-stu-id="9188b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9188b-133">resource.islocked</span><span class="sxs-lookup"><span data-stu-id="9188b-133">isLocked</span></span>|<span data-ttu-id="9188b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="9188b-134">Boolean</span></span>|<span data-ttu-id="9188b-p105">指示线程是否已锁定。设置为 `true` 以禁止发布。</span><span class="sxs-lookup"><span data-stu-id="9188b-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="9188b-137">响应</span><span class="sxs-lookup"><span data-stu-id="9188b-137">Response</span></span>

<span data-ttu-id="9188b-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9188b-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9188b-139">示例</span><span class="sxs-lookup"><span data-stu-id="9188b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9188b-140">请求</span><span class="sxs-lookup"><span data-stu-id="9188b-140">Request</span></span>
<span data-ttu-id="9188b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9188b-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9188b-142">响应</span><span class="sxs-lookup"><span data-stu-id="9188b-142">Response</span></span>
<span data-ttu-id="9188b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9188b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
