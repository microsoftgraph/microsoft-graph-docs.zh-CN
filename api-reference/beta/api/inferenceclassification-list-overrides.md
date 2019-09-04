---
title: 列表替代
description: 获取重点收件箱覆盖, 用户已设置为始终按特定方式对来自特定发件人的邮件进行分类。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 567f4f28459014f47ef619bdc8c4a3000c818264
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721479"
---
# <a name="list-overrides"></a><span data-ttu-id="68e62-103">列表替代</span><span class="sxs-lookup"><span data-stu-id="68e62-103">List overrides</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e62-104">获取[重点收件箱](../resources/manage-focused-inbox.md)覆盖, 用户已设置为始终按特定方式对来自特定发件人的邮件进行分类。</span><span class="sxs-lookup"><span data-stu-id="68e62-104">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="68e62-105">每个替代均对应一个发件人的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="68e62-105">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="68e62-106">最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="68e62-106">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="68e62-107">权限</span><span class="sxs-lookup"><span data-stu-id="68e62-107">Permissions</span></span>
<span data-ttu-id="68e62-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68e62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="68e62-110">Permission type</span></span>      | <span data-ttu-id="68e62-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68e62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68e62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68e62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68e62-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="68e62-113">Mail.Read</span></span>    |
|<span data-ttu-id="68e62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68e62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e62-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="68e62-115">Mail.Read</span></span>    |
|<span data-ttu-id="68e62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="68e62-116">Application</span></span> | <span data-ttu-id="68e62-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="68e62-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="68e62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68e62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="68e62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="68e62-119">Request headers</span></span>
| <span data-ttu-id="68e62-120">名称</span><span class="sxs-lookup"><span data-stu-id="68e62-120">Name</span></span>       | <span data-ttu-id="68e62-121">类型</span><span class="sxs-lookup"><span data-stu-id="68e62-121">Type</span></span> | <span data-ttu-id="68e62-122">说明</span><span class="sxs-lookup"><span data-stu-id="68e62-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68e62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68e62-123">Authorization</span></span>  | <span data-ttu-id="68e62-124">string</span><span class="sxs-lookup"><span data-stu-id="68e62-124">string</span></span>  | <span data-ttu-id="68e62-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68e62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68e62-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="68e62-127">Request body</span></span>
<span data-ttu-id="68e62-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68e62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68e62-129">响应</span><span class="sxs-lookup"><span data-stu-id="68e62-129">Response</span></span>

<span data-ttu-id="68e62-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="68e62-130">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68e62-131">示例</span><span class="sxs-lookup"><span data-stu-id="68e62-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68e62-132">请求</span><span class="sxs-lookup"><span data-stu-id="68e62-132">Request</span></span>
<span data-ttu-id="68e62-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68e62-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="68e62-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="68e62-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68e62-135">C#</span><span class="sxs-lookup"><span data-stu-id="68e62-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68e62-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68e62-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68e62-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="68e62-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="68e62-138">响应</span><span class="sxs-lookup"><span data-stu-id="68e62-138">Response</span></span>
<span data-ttu-id="68e62-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68e62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
