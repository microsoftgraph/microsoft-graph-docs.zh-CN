---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 2fb7dd31c19c820e8f2d9618fa37331d65abfac3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410841"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="019f6-103">riskyUser: 消除</span><span class="sxs-lookup"><span data-stu-id="019f6-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="019f6-104">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="019f6-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="019f6-105">消除一个或多个[riskyUser](../resources/riskyuser.md)对象的风险。</span><span class="sxs-lookup"><span data-stu-id="019f6-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="019f6-106">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="019f6-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="019f6-107">权限</span><span class="sxs-lookup"><span data-stu-id="019f6-107">Permissions</span></span>
<span data-ttu-id="019f6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="019f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="019f6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="019f6-110">Permission type</span></span>      | <span data-ttu-id="019f6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="019f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="019f6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="019f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="019f6-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="019f6-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="019f6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="019f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="019f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="019f6-115">Not supported.</span></span>    |
|<span data-ttu-id="019f6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="019f6-116">Application</span></span> | <span data-ttu-id="019f6-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="019f6-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="019f6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="019f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="019f6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="019f6-119">Request headers</span></span>
| <span data-ttu-id="019f6-120">名称</span><span class="sxs-lookup"><span data-stu-id="019f6-120">Name</span></span>      |<span data-ttu-id="019f6-121">说明</span><span class="sxs-lookup"><span data-stu-id="019f6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="019f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="019f6-122">Authorization</span></span>  | <span data-ttu-id="019f6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="019f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="019f6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="019f6-125">Request body</span></span>
<span data-ttu-id="019f6-126">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="019f6-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="019f6-127">响应</span><span class="sxs-lookup"><span data-stu-id="019f6-127">Response</span></span>

<span data-ttu-id="019f6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="019f6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="019f6-130">示例</span><span class="sxs-lookup"><span data-stu-id="019f6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="019f6-131">请求</span><span class="sxs-lookup"><span data-stu-id="019f6-131">Request</span></span>
<span data-ttu-id="019f6-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="019f6-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="019f6-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="019f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="019f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="019f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="019f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="019f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="019f6-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="019f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="019f6-137">响应</span><span class="sxs-lookup"><span data-stu-id="019f6-137">Response</span></span>
<span data-ttu-id="019f6-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="019f6-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
