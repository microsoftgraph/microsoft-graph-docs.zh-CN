---
title: 向团队添加应用
description: 将应用程序安装到指定的团队。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 084b759ef13ab72831b3ba73c8a5901c75ab5832
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978410"
---
# <a name="add-app-to-team"></a><span data-ttu-id="aa148-103">向团队添加应用</span><span class="sxs-lookup"><span data-stu-id="aa148-103">Add app to team</span></span>

<span data-ttu-id="aa148-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa148-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa148-105">将 [应用程序](../resources/teamsapp.md) 安装到指定的 [团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="aa148-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aa148-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa148-106">Permissions</span></span>

<span data-ttu-id="aa148-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa148-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa148-109">Permission type</span></span>      | <span data-ttu-id="aa148-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa148-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa148-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa148-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa148-112">TeamsAppInstallation，ReadWriteForTeam，all，All，All</span><span class="sxs-lookup"><span data-stu-id="aa148-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="aa148-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa148-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa148-114">Not supported.</span></span>    |
|<span data-ttu-id="aa148-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa148-115">Application</span></span> | <span data-ttu-id="aa148-116">TeamsAppInstallation、ReadWriteForTeam、all、ReadWrite。所有</span><span class="sxs-lookup"><span data-stu-id="aa148-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa148-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa148-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="aa148-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa148-118">Request headers</span></span>

| <span data-ttu-id="aa148-119">标头</span><span class="sxs-lookup"><span data-stu-id="aa148-119">Header</span></span>       | <span data-ttu-id="aa148-120">值</span><span class="sxs-lookup"><span data-stu-id="aa148-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa148-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa148-121">Authorization</span></span>  | <span data-ttu-id="aa148-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa148-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa148-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa148-124">Request body</span></span>

| <span data-ttu-id="aa148-125">属性</span><span class="sxs-lookup"><span data-stu-id="aa148-125">Property</span></span>   | <span data-ttu-id="aa148-126">类型</span><span class="sxs-lookup"><span data-stu-id="aa148-126">Type</span></span> |<span data-ttu-id="aa148-127">说明</span><span class="sxs-lookup"><span data-stu-id="aa148-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa148-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="aa148-128">teamsApp</span></span>| [<span data-ttu-id="aa148-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="aa148-129">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="aa148-130">要添加的应用程序。</span><span class="sxs-lookup"><span data-stu-id="aa148-130">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="aa148-131">响应</span><span class="sxs-lookup"><span data-stu-id="aa148-131">Response</span></span>

<span data-ttu-id="aa148-p103">如果成功，此方法返回 `201 Created` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aa148-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa148-134">示例</span><span class="sxs-lookup"><span data-stu-id="aa148-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa148-135">请求</span><span class="sxs-lookup"><span data-stu-id="aa148-135">Request</span></span>

<span data-ttu-id="aa148-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa148-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aa148-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa148-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="aa148-138">C#</span><span class="sxs-lookup"><span data-stu-id="aa148-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa148-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa148-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa148-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa148-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa148-141">Java</span><span class="sxs-lookup"><span data-stu-id="aa148-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa148-142">响应</span><span class="sxs-lookup"><span data-stu-id="aa148-142">Response</span></span>

<span data-ttu-id="aa148-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa148-143">The following is an example of the response.</span></span>

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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

