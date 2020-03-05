---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: cb6d0e5aae8894408c274c4ad628e38552577d3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453868"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="71b7b-103">riskyUser：消除</span><span class="sxs-lookup"><span data-stu-id="71b7b-103">riskyUser: dismiss</span></span>

<span data-ttu-id="71b7b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="71b7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="71b7b-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="71b7b-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="71b7b-106">消除一个或多个[riskyUser](../resources/riskyuser.md)对象的风险。</span><span class="sxs-lookup"><span data-stu-id="71b7b-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="71b7b-107">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="71b7b-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="71b7b-108">权限</span><span class="sxs-lookup"><span data-stu-id="71b7b-108">Permissions</span></span>
<span data-ttu-id="71b7b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71b7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b7b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71b7b-111">Permission type</span></span>      | <span data-ttu-id="71b7b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71b7b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b7b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71b7b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="71b7b-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71b7b-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="71b7b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71b7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b7b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b7b-116">Not supported.</span></span>    |
|<span data-ttu-id="71b7b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71b7b-117">Application</span></span> | <span data-ttu-id="71b7b-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71b7b-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b7b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71b7b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="71b7b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71b7b-120">Request headers</span></span>
| <span data-ttu-id="71b7b-121">名称</span><span class="sxs-lookup"><span data-stu-id="71b7b-121">Name</span></span>      |<span data-ttu-id="71b7b-122">说明</span><span class="sxs-lookup"><span data-stu-id="71b7b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71b7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71b7b-123">Authorization</span></span>  | <span data-ttu-id="71b7b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71b7b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71b7b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71b7b-126">Request body</span></span>
<span data-ttu-id="71b7b-127">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="71b7b-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="71b7b-128">响应</span><span class="sxs-lookup"><span data-stu-id="71b7b-128">Response</span></span>

<span data-ttu-id="71b7b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71b7b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71b7b-131">示例</span><span class="sxs-lookup"><span data-stu-id="71b7b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71b7b-132">请求</span><span class="sxs-lookup"><span data-stu-id="71b7b-132">Request</span></span>
<span data-ttu-id="71b7b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71b7b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71b7b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="71b7b-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71b7b-135">C#</span><span class="sxs-lookup"><span data-stu-id="71b7b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71b7b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71b7b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71b7b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71b7b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="71b7b-138">响应</span><span class="sxs-lookup"><span data-stu-id="71b7b-138">Response</span></span>
<span data-ttu-id="71b7b-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71b7b-139">Here is an example of the response.</span></span>
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
