---
title: 列表替代
description: 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。
localization_priority: Normal
ms.openlocfilehash: ab8324ac892df570ed0d28fabb7b31f3280adcef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577614"
---
# <a name="list-overrides"></a><span data-ttu-id="63ad0-103">列表替代</span><span class="sxs-lookup"><span data-stu-id="63ad0-103">List overrides</span></span>

<span data-ttu-id="63ad0-104">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="63ad0-104">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="63ad0-p101">每个替代均对应一个发件人的 SMTP 地址。最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="63ad0-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="63ad0-107">权限</span><span class="sxs-lookup"><span data-stu-id="63ad0-107">Permissions</span></span>
<span data-ttu-id="63ad0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63ad0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63ad0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="63ad0-110">Permission type</span></span>      | <span data-ttu-id="63ad0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63ad0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63ad0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63ad0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63ad0-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="63ad0-113">Mail.Read</span></span>    |
|<span data-ttu-id="63ad0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63ad0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ad0-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="63ad0-115">Mail.Read</span></span>    |
|<span data-ttu-id="63ad0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="63ad0-116">Application</span></span> | <span data-ttu-id="63ad0-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="63ad0-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="63ad0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63ad0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="63ad0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="63ad0-119">Request headers</span></span>
| <span data-ttu-id="63ad0-120">名称</span><span class="sxs-lookup"><span data-stu-id="63ad0-120">Name</span></span>       | <span data-ttu-id="63ad0-121">类型</span><span class="sxs-lookup"><span data-stu-id="63ad0-121">Type</span></span> | <span data-ttu-id="63ad0-122">说明</span><span class="sxs-lookup"><span data-stu-id="63ad0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="63ad0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63ad0-123">Authorization</span></span>  | <span data-ttu-id="63ad0-124">string</span><span class="sxs-lookup"><span data-stu-id="63ad0-124">string</span></span>  | <span data-ttu-id="63ad0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63ad0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63ad0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63ad0-127">Request body</span></span>
<span data-ttu-id="63ad0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63ad0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63ad0-129">响应</span><span class="sxs-lookup"><span data-stu-id="63ad0-129">Response</span></span>

<span data-ttu-id="63ad0-p104">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象集合。如果用户未设置任何替代，则返回空集合。</span><span class="sxs-lookup"><span data-stu-id="63ad0-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="63ad0-132">示例</span><span class="sxs-lookup"><span data-stu-id="63ad0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63ad0-133">请求</span><span class="sxs-lookup"><span data-stu-id="63ad0-133">Request</span></span>
<span data-ttu-id="63ad0-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63ad0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="63ad0-135">响应</span><span class="sxs-lookup"><span data-stu-id="63ad0-135">Response</span></span>
<span data-ttu-id="63ad0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63ad0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
