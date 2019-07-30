---
title: 从团队中删除应用
description: 从指定的团队中卸载应用程序。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 59caed63c53dacd86b6303dfdf29ad018e0f4677
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932428"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="f6f1c-103">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="f6f1c-103">Remove app from team</span></span>

<span data-ttu-id="f6f1c-104">从指定的[团队](../resources/team.md)中卸载[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6f1c-105">权限</span><span class="sxs-lookup"><span data-stu-id="f6f1c-105">Permissions</span></span>

<span data-ttu-id="f6f1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f1c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6f1c-108">Permission type</span></span>      | <span data-ttu-id="f6f1c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6f1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6f1c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6f1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6f1c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f1c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6f1c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6f1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6f1c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-113">Not supported.</span></span>    |
|<span data-ttu-id="f6f1c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6f1c-114">Application</span></span> | <span data-ttu-id="f6f1c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f1c-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="f6f1c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6f1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6f1c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6f1c-117">Request headers</span></span>

| <span data-ttu-id="f6f1c-118">标头</span><span class="sxs-lookup"><span data-stu-id="f6f1c-118">Header</span></span>       | <span data-ttu-id="f6f1c-119">值</span><span class="sxs-lookup"><span data-stu-id="f6f1c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6f1c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6f1c-120">Authorization</span></span>  | <span data-ttu-id="f6f1c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6f1c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6f1c-123">Request body</span></span>

<span data-ttu-id="f6f1c-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6f1c-125">响应</span><span class="sxs-lookup"><span data-stu-id="f6f1c-125">Response</span></span>

<span data-ttu-id="f6f1c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6f1c-128">示例</span><span class="sxs-lookup"><span data-stu-id="f6f1c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6f1c-129">请求</span><span class="sxs-lookup"><span data-stu-id="f6f1c-129">Request</span></span>

<span data-ttu-id="f6f1c-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6f1c-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f6f1c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->

```http
DELETE /teams/{id}/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6f1c-132">C#</span><span class="sxs-lookup"><span data-stu-id="f6f1c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6f1c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6f1c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6f1c-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="f6f1c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f6f1c-135">Java</span><span class="sxs-lookup"><span data-stu-id="f6f1c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6f1c-136">响应</span><span class="sxs-lookup"><span data-stu-id="f6f1c-136">Response</span></span>

<span data-ttu-id="f6f1c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6f1c-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
