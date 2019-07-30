---
title: 为用户安装应用程序
description: 在指定用户的个人作用域中安装应用程序。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 08c0339c7d8923a5d6988245d8b2f488197c82ba
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931442"
---
# <a name="install-app-for-user"></a><span data-ttu-id="67563-103">为用户安装应用程序</span><span class="sxs-lookup"><span data-stu-id="67563-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67563-104">在指定[用户](../resources/user.md)的个人作用域中安装[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="67563-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67563-105">权限</span><span class="sxs-lookup"><span data-stu-id="67563-105">Permissions</span></span>

<span data-ttu-id="67563-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67563-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="67563-108">Permission type</span></span>      | <span data-ttu-id="67563-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67563-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67563-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67563-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67563-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67563-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="67563-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67563-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67563-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="67563-113">Not supported.</span></span>    |
|<span data-ttu-id="67563-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="67563-114">Application</span></span> | <span data-ttu-id="67563-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67563-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67563-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67563-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="67563-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="67563-117">Request headers</span></span>

| <span data-ttu-id="67563-118">标头</span><span class="sxs-lookup"><span data-stu-id="67563-118">Header</span></span>       | <span data-ttu-id="67563-119">值</span><span class="sxs-lookup"><span data-stu-id="67563-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67563-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="67563-120">Authorization</span></span>  | <span data-ttu-id="67563-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67563-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67563-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="67563-123">Request body</span></span>

<span data-ttu-id="67563-124">请求正文应包含要添加的现有目录应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="67563-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="67563-125">属性</span><span class="sxs-lookup"><span data-stu-id="67563-125">Property</span></span>   | <span data-ttu-id="67563-126">类型</span><span class="sxs-lookup"><span data-stu-id="67563-126">Type</span></span> |<span data-ttu-id="67563-127">说明</span><span class="sxs-lookup"><span data-stu-id="67563-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67563-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="67563-128">teamsApp</span></span>|<span data-ttu-id="67563-129">String</span><span class="sxs-lookup"><span data-stu-id="67563-129">String</span></span>|<span data-ttu-id="67563-130">要添加的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="67563-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="67563-131">响应</span><span class="sxs-lookup"><span data-stu-id="67563-131">Response</span></span>

<span data-ttu-id="67563-p103">如果成功，此方法返回 `201 Created` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="67563-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67563-134">示例</span><span class="sxs-lookup"><span data-stu-id="67563-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="67563-135">请求</span><span class="sxs-lookup"><span data-stu-id="67563-135">Request</span></span>

<span data-ttu-id="67563-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67563-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67563-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="67563-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67563-138">C#</span><span class="sxs-lookup"><span data-stu-id="67563-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67563-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="67563-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67563-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="67563-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67563-141">Java</span><span class="sxs-lookup"><span data-stu-id="67563-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="67563-142">响应</span><span class="sxs-lookup"><span data-stu-id="67563-142">Response</span></span>

<span data-ttu-id="67563-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67563-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
