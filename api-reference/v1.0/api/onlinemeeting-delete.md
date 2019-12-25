---
title: 删除 onlineMeeting
description: 删除联机会议。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e2c8b66ab247c629513de0698cef30de8420525c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865822"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="56fc3-103">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="56fc3-103">Delete onlineMeeting</span></span>

<span data-ttu-id="56fc3-104">删除[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="56fc3-104">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="56fc3-105">权限</span><span class="sxs-lookup"><span data-stu-id="56fc3-105">Permissions</span></span>

| <span data-ttu-id="56fc3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="56fc3-106">Permission type</span></span> | <span data-ttu-id="56fc3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56fc3-107">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="56fc3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56fc3-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="56fc3-109">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56fc3-109">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="56fc3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56fc3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56fc3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="56fc3-111">Not Supported.</span></span>                         |
| <span data-ttu-id="56fc3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="56fc3-112">Application</span></span>                            | <span data-ttu-id="56fc3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="56fc3-113">Not Supported.</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="56fc3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56fc3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56fc3-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="56fc3-115">Request headers</span></span>
| <span data-ttu-id="56fc3-116">名称</span><span class="sxs-lookup"><span data-stu-id="56fc3-116">Name</span></span>          | <span data-ttu-id="56fc3-117">说明</span><span class="sxs-lookup"><span data-stu-id="56fc3-117">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="56fc3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="56fc3-118">Authorization</span></span> | <span data-ttu-id="56fc3-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56fc3-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56fc3-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="56fc3-121">Request body</span></span>
<span data-ttu-id="56fc3-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56fc3-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56fc3-123">响应</span><span class="sxs-lookup"><span data-stu-id="56fc3-123">Response</span></span>
<span data-ttu-id="56fc3-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="56fc3-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56fc3-126">示例</span><span class="sxs-lookup"><span data-stu-id="56fc3-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56fc3-127">请求</span><span class="sxs-lookup"><span data-stu-id="56fc3-127">Request</span></span>
<span data-ttu-id="56fc3-128">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="56fc3-128">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="56fc3-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="56fc3-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56fc3-130">C#</span><span class="sxs-lookup"><span data-stu-id="56fc3-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56fc3-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56fc3-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56fc3-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56fc3-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56fc3-133">响应</span><span class="sxs-lookup"><span data-stu-id="56fc3-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
