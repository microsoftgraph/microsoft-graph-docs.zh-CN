---
title: 向团队添加应用
description: 将应用程序安装到指定的团队。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc5f92212d9fbeb6b061f952ff31c76fcf1f2ce8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375497"
---
# <a name="add-app-to-team"></a><span data-ttu-id="15574-103">向团队添加应用</span><span class="sxs-lookup"><span data-stu-id="15574-103">Add app to team</span></span>

<span data-ttu-id="15574-104">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="15574-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="15574-105">权限</span><span class="sxs-lookup"><span data-stu-id="15574-105">Permissions</span></span>

<span data-ttu-id="15574-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15574-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="15574-108">Permission type</span></span>      | <span data-ttu-id="15574-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15574-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15574-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15574-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15574-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15574-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="15574-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15574-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15574-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="15574-113">Not supported.</span></span>    |
|<span data-ttu-id="15574-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="15574-114">Application</span></span> | <span data-ttu-id="15574-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15574-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15574-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15574-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="15574-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="15574-117">Request headers</span></span>

| <span data-ttu-id="15574-118">标头</span><span class="sxs-lookup"><span data-stu-id="15574-118">Header</span></span>       | <span data-ttu-id="15574-119">值</span><span class="sxs-lookup"><span data-stu-id="15574-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15574-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="15574-120">Authorization</span></span>  | <span data-ttu-id="15574-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15574-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15574-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="15574-123">Request body</span></span>

| <span data-ttu-id="15574-124">属性</span><span class="sxs-lookup"><span data-stu-id="15574-124">Property</span></span>   | <span data-ttu-id="15574-125">类型</span><span class="sxs-lookup"><span data-stu-id="15574-125">Type</span></span> |<span data-ttu-id="15574-126">说明</span><span class="sxs-lookup"><span data-stu-id="15574-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15574-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="15574-127">teamsApp</span></span>| [<span data-ttu-id="15574-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="15574-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="15574-129">要添加的应用程序。</span><span class="sxs-lookup"><span data-stu-id="15574-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="15574-130">响应</span><span class="sxs-lookup"><span data-stu-id="15574-130">Response</span></span>

<span data-ttu-id="15574-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="15574-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15574-133">示例</span><span class="sxs-lookup"><span data-stu-id="15574-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="15574-134">请求</span><span class="sxs-lookup"><span data-stu-id="15574-134">Request</span></span>

<span data-ttu-id="15574-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15574-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="15574-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="15574-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="15574-137">C#</span><span class="sxs-lookup"><span data-stu-id="15574-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15574-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15574-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15574-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="15574-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="15574-140">Java</span><span class="sxs-lookup"><span data-stu-id="15574-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15574-141">响应</span><span class="sxs-lookup"><span data-stu-id="15574-141">Response</span></span>

<span data-ttu-id="15574-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="15574-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
