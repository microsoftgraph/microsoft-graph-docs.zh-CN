---
title: 向团队添加应用
description: 将应用程序安装到指定的团队。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 86902435cad896256775711f48dd4a531adce8f9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931685"
---
# <a name="add-app-to-team"></a><span data-ttu-id="8f0a5-103">向团队添加应用</span><span class="sxs-lookup"><span data-stu-id="8f0a5-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f0a5-104">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f0a5-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f0a5-105">Permissions</span></span>

<span data-ttu-id="8f0a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f0a5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f0a5-108">Permission type</span></span>      | <span data-ttu-id="8f0a5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f0a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f0a5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f0a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f0a5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f0a5-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f0a5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f0a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f0a5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-113">Not supported.</span></span>    |
|<span data-ttu-id="8f0a5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f0a5-114">Application</span></span> | <span data-ttu-id="8f0a5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f0a5-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f0a5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f0a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="8f0a5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f0a5-117">Request headers</span></span>

| <span data-ttu-id="8f0a5-118">标头</span><span class="sxs-lookup"><span data-stu-id="8f0a5-118">Header</span></span>       | <span data-ttu-id="8f0a5-119">值</span><span class="sxs-lookup"><span data-stu-id="8f0a5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f0a5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f0a5-120">Authorization</span></span>  | <span data-ttu-id="8f0a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f0a5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f0a5-123">Request body</span></span>

| <span data-ttu-id="8f0a5-124">属性</span><span class="sxs-lookup"><span data-stu-id="8f0a5-124">Property</span></span>   | <span data-ttu-id="8f0a5-125">类型</span><span class="sxs-lookup"><span data-stu-id="8f0a5-125">Type</span></span> |<span data-ttu-id="8f0a5-126">说明</span><span class="sxs-lookup"><span data-stu-id="8f0a5-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f0a5-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8f0a5-127">teamsApp</span></span>|<span data-ttu-id="8f0a5-128">String</span><span class="sxs-lookup"><span data-stu-id="8f0a5-128">String</span></span>|<span data-ttu-id="8f0a5-129">要添加的应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-129">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="8f0a5-130">响应</span><span class="sxs-lookup"><span data-stu-id="8f0a5-130">Response</span></span>

<span data-ttu-id="8f0a5-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f0a5-133">示例</span><span class="sxs-lookup"><span data-stu-id="8f0a5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f0a5-134">请求</span><span class="sxs-lookup"><span data-stu-id="8f0a5-134">Request</span></span>

<span data-ttu-id="8f0a5-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f0a5-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8f0a5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_teamsApp"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f0a5-137">C#</span><span class="sxs-lookup"><span data-stu-id="8f0a5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f0a5-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f0a5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f0a5-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="8f0a5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f0a5-140">Java</span><span class="sxs-lookup"><span data-stu-id="8f0a5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f0a5-141">响应</span><span class="sxs-lookup"><span data-stu-id="8f0a5-141">Response</span></span>

<span data-ttu-id="8f0a5-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f0a5-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add teamsApp",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
