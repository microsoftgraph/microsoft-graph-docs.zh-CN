---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: b88070f32a021f1d79aa85c091cadc52f2f600ea
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264986"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="1043b-103">riskyUser: 消除</span><span class="sxs-lookup"><span data-stu-id="1043b-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="1043b-104">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="1043b-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="1043b-105">消除一个或多个[riskyUser](../resources/riskyuser.md)对象的风险。</span><span class="sxs-lookup"><span data-stu-id="1043b-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="1043b-106">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="1043b-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="1043b-107">权限</span><span class="sxs-lookup"><span data-stu-id="1043b-107">Permissions</span></span>
<span data-ttu-id="1043b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1043b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1043b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1043b-110">Permission type</span></span>      | <span data-ttu-id="1043b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1043b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1043b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1043b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1043b-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="1043b-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="1043b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1043b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1043b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1043b-115">Not supported.</span></span>    |
|<span data-ttu-id="1043b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1043b-116">Application</span></span> | <span data-ttu-id="1043b-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="1043b-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1043b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1043b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="1043b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1043b-119">Request headers</span></span>
| <span data-ttu-id="1043b-120">名称</span><span class="sxs-lookup"><span data-stu-id="1043b-120">Name</span></span>      |<span data-ttu-id="1043b-121">说明</span><span class="sxs-lookup"><span data-stu-id="1043b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1043b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1043b-122">Authorization</span></span>  | <span data-ttu-id="1043b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1043b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1043b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1043b-125">Request body</span></span>
<span data-ttu-id="1043b-126">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="1043b-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="1043b-127">响应</span><span class="sxs-lookup"><span data-stu-id="1043b-127">Response</span></span>

<span data-ttu-id="1043b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1043b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1043b-130">示例</span><span class="sxs-lookup"><span data-stu-id="1043b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1043b-131">请求</span><span class="sxs-lookup"><span data-stu-id="1043b-131">Request</span></span>
<span data-ttu-id="1043b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1043b-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1043b-133">响应</span><span class="sxs-lookup"><span data-stu-id="1043b-133">Response</span></span>
<span data-ttu-id="1043b-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1043b-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1043b-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1043b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1043b-136">C#</span><span class="sxs-lookup"><span data-stu-id="1043b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1043b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="1043b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1043b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="1043b-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
