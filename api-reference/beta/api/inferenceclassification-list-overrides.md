---
title: 列出替代
description: 获取用户已将设置为始终以特定方式分类来自特定发件人关注的收件箱覆盖。
ms.openlocfilehash: 343faaacf47d16b723cd8aebc25a6df79ef7e3db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048748"
---
# <a name="list-overrides"></a><span data-ttu-id="4ab4c-103">列出替代</span><span class="sxs-lookup"><span data-stu-id="4ab4c-103">List overrides</span></span>

> <span data-ttu-id="4ab4c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ab4c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ab4c-106">获取用户已将设置为始终以特定方式分类来自特定发件人[关注的收件箱](../resources/manage-focused-inbox.md)覆盖。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-106">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="4ab4c-p102">每个替代均对应一个发件人的 SMTP 地址。最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-p102">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ab4c-109">权限</span><span class="sxs-lookup"><span data-stu-id="4ab4c-109">Permissions</span></span>
<span data-ttu-id="4ab4c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab4c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ab4c-112">Permission type</span></span>      | <span data-ttu-id="4ab4c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ab4c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ab4c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab4c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab4c-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4ab4c-115">Mail.Read</span></span>    |
|<span data-ttu-id="4ab4c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab4c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab4c-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4ab4c-117">Mail.Read</span></span>    |
|<span data-ttu-id="4ab4c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ab4c-118">Application</span></span> | <span data-ttu-id="4ab4c-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4ab4c-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ab4c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ab4c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="4ab4c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ab4c-121">Request headers</span></span>
| <span data-ttu-id="4ab4c-122">名称</span><span class="sxs-lookup"><span data-stu-id="4ab4c-122">Name</span></span>       | <span data-ttu-id="4ab4c-123">类型</span><span class="sxs-lookup"><span data-stu-id="4ab4c-123">Type</span></span> | <span data-ttu-id="4ab4c-124">说明</span><span class="sxs-lookup"><span data-stu-id="4ab4c-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ab4c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab4c-125">Authorization</span></span>  | <span data-ttu-id="4ab4c-126">string</span><span class="sxs-lookup"><span data-stu-id="4ab4c-126">string</span></span>  | <span data-ttu-id="4ab4c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ab4c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ab4c-129">Request body</span></span>
<span data-ttu-id="4ab4c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab4c-131">响应</span><span class="sxs-lookup"><span data-stu-id="4ab4c-131">Response</span></span>

<span data-ttu-id="4ab4c-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-132">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ab4c-133">示例</span><span class="sxs-lookup"><span data-stu-id="4ab4c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ab4c-134">请求</span><span class="sxs-lookup"><span data-stu-id="4ab4c-134">Request</span></span>
<span data-ttu-id="4ab4c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="4ab4c-136">响应</span><span class="sxs-lookup"><span data-stu-id="4ab4c-136">Response</span></span>
<span data-ttu-id="4ab4c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ab4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->