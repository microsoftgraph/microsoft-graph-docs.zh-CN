---
title: 确认 riskyUser 已泄露
description: 确认 riskyUser 对象是否已泄露。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: ca2cbaacdc84f7c7aee3f1894beef562dd094ba9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871036"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="160b7-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="160b7-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="160b7-104">**注意:** RiskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="160b7-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="160b7-105">确认一个或多个[riskyUser](../resources/riskyuser.md)对象已泄露。</span><span class="sxs-lookup"><span data-stu-id="160b7-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="160b7-106">此操作将目标用户的风险级别设置为 "高"。</span><span class="sxs-lookup"><span data-stu-id="160b7-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="160b7-107">权限</span><span class="sxs-lookup"><span data-stu-id="160b7-107">Permissions</span></span>
<span data-ttu-id="160b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="160b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="160b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="160b7-110">Permission type</span></span>      | <span data-ttu-id="160b7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="160b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="160b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="160b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="160b7-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="160b7-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="160b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="160b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="160b7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="160b7-115">Not supported.</span></span>    |
|<span data-ttu-id="160b7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="160b7-116">Application</span></span> | <span data-ttu-id="160b7-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="160b7-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="160b7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="160b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="160b7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="160b7-119">Request headers</span></span>
| <span data-ttu-id="160b7-120">名称</span><span class="sxs-lookup"><span data-stu-id="160b7-120">Name</span></span>      |<span data-ttu-id="160b7-121">说明</span><span class="sxs-lookup"><span data-stu-id="160b7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="160b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="160b7-122">Authorization</span></span>  | <span data-ttu-id="160b7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="160b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="160b7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="160b7-125">Request body</span></span>
<span data-ttu-id="160b7-126">指定要在请求正文中消除的有风险的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="160b7-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="160b7-127">响应</span><span class="sxs-lookup"><span data-stu-id="160b7-127">Response</span></span>

<span data-ttu-id="160b7-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="160b7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="160b7-130">示例</span><span class="sxs-lookup"><span data-stu-id="160b7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="160b7-131">请求</span><span class="sxs-lookup"><span data-stu-id="160b7-131">Request</span></span>
<span data-ttu-id="160b7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="160b7-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="160b7-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="160b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="160b7-134">C#</span><span class="sxs-lookup"><span data-stu-id="160b7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="160b7-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="160b7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="160b7-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="160b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="160b7-137">Java</span><span class="sxs-lookup"><span data-stu-id="160b7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="160b7-138">响应</span><span class="sxs-lookup"><span data-stu-id="160b7-138">Response</span></span>
<span data-ttu-id="160b7-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="160b7-139">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
