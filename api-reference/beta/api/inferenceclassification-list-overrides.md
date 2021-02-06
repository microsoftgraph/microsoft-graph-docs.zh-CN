---
title: 列出替代
description: 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的重点收件箱替代。
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: ''
ms.openlocfilehash: 486d99db01c2efbbc0ff295730cf248aaffb643a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130723"
---
# <a name="list-overrides"></a><span data-ttu-id="fa870-103">列出替代</span><span class="sxs-lookup"><span data-stu-id="fa870-103">List overrides</span></span>

<span data-ttu-id="fa870-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa870-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa870-105">获取 [用户设置为](../resources/manage-focused-inbox.md) 始终以特定方式对来自某些发件人的邮件进行分类的重点收件箱替代。</span><span class="sxs-lookup"><span data-stu-id="fa870-105">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="fa870-106">每个替代均对应一个发件人的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="fa870-106">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="fa870-107">最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="fa870-107">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa870-108">权限</span><span class="sxs-lookup"><span data-stu-id="fa870-108">Permissions</span></span>
<span data-ttu-id="fa870-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa870-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa870-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa870-111">Permission type</span></span>      | <span data-ttu-id="fa870-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa870-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa870-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa870-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa870-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fa870-114">Mail.Read</span></span>    |
|<span data-ttu-id="fa870-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa870-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa870-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fa870-116">Mail.Read</span></span>    |
|<span data-ttu-id="fa870-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa870-117">Application</span></span> | <span data-ttu-id="fa870-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fa870-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa870-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa870-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="fa870-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa870-120">Request headers</span></span>
| <span data-ttu-id="fa870-121">名称</span><span class="sxs-lookup"><span data-stu-id="fa870-121">Name</span></span>       | <span data-ttu-id="fa870-122">类型</span><span class="sxs-lookup"><span data-stu-id="fa870-122">Type</span></span> | <span data-ttu-id="fa870-123">说明</span><span class="sxs-lookup"><span data-stu-id="fa870-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fa870-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa870-124">Authorization</span></span>  | <span data-ttu-id="fa870-125">string</span><span class="sxs-lookup"><span data-stu-id="fa870-125">string</span></span>  | <span data-ttu-id="fa870-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa870-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa870-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa870-128">Request body</span></span>
<span data-ttu-id="fa870-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa870-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa870-130">响应</span><span class="sxs-lookup"><span data-stu-id="fa870-130">Response</span></span>

<span data-ttu-id="fa870-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fa870-131">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa870-132">示例</span><span class="sxs-lookup"><span data-stu-id="fa870-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa870-133">请求</span><span class="sxs-lookup"><span data-stu-id="fa870-133">Request</span></span>
<span data-ttu-id="fa870-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa870-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa870-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa870-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="fa870-136">C#</span><span class="sxs-lookup"><span data-stu-id="fa870-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa870-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa870-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa870-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa870-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa870-139">Java</span><span class="sxs-lookup"><span data-stu-id="fa870-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa870-140">响应</span><span class="sxs-lookup"><span data-stu-id="fa870-140">Response</span></span>
<span data-ttu-id="fa870-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa870-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


