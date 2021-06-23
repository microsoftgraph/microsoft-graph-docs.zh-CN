---
title: 为用户卸载应用
description: 卸载指定用户的个人范围内的应用。
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b8bee27b4179cad4d2451ec61fda7e8304142de9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060325"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="0f212-103">为用户卸载应用</span><span class="sxs-lookup"><span data-stu-id="0f212-103">Uninstall app for user</span></span>

<span data-ttu-id="0f212-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f212-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f212-105">从 [指定](../resources/teamsappinstallation.md) 用户的个人作用域卸载 [应用](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="0f212-105">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f212-106">权限</span><span class="sxs-lookup"><span data-stu-id="0f212-106">Permissions</span></span>

<span data-ttu-id="0f212-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f212-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f212-109">Permission type</span></span>      | <span data-ttu-id="0f212-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f212-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f212-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f212-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f212-112">TeamsAppInstallation.ReadWriteSelfForUser、TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="0f212-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="0f212-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f212-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f212-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f212-114">Not supported.</span></span>    |
|<span data-ttu-id="0f212-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f212-115">Application</span></span> | <span data-ttu-id="0f212-116">TeamsAppInstallation.ReadWriteSelfForUser.All、TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="0f212-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f212-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f212-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{user-id | user-principal-name}/teamwork/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="0f212-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f212-118">Request headers</span></span>

| <span data-ttu-id="0f212-119">标头</span><span class="sxs-lookup"><span data-stu-id="0f212-119">Header</span></span>       | <span data-ttu-id="0f212-120">值</span><span class="sxs-lookup"><span data-stu-id="0f212-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f212-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f212-121">Authorization</span></span>  | <span data-ttu-id="0f212-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f212-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f212-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f212-124">Request body</span></span>

<span data-ttu-id="0f212-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f212-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f212-126">响应</span><span class="sxs-lookup"><span data-stu-id="0f212-126">Response</span></span>

<span data-ttu-id="0f212-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0f212-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f212-129">示例</span><span class="sxs-lookup"><span data-stu-id="0f212-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f212-130">请求</span><span class="sxs-lookup"><span data-stu-id="0f212-130">Request</span></span>

<span data-ttu-id="0f212-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0f212-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0f212-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f212-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```
# <a name="c"></a>[<span data-ttu-id="0f212-133">C#</span><span class="sxs-lookup"><span data-stu-id="0f212-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f212-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f212-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f212-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f212-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f212-136">Java</span><span class="sxs-lookup"><span data-stu-id="0f212-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f212-137">响应</span><span class="sxs-lookup"><span data-stu-id="0f212-137">Response</span></span>

<span data-ttu-id="0f212-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0f212-138">The following is an example of the response.</span></span>

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
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
