---
title: teamsAppInstallation：升级
description: 在用户的个人范围内升级应用安装
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8c087d6676c2829e3796f5f6f3e2fee0b596f966
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060576"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="a5674-103">teamsAppInstallation：升级</span><span class="sxs-lookup"><span data-stu-id="a5674-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="a5674-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5674-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5674-105">将 [指定用户](../resources/teamsappinstallation.md) 的个人范围中的应用 [安装升级到](../resources/user.md) 应用的最新版本。</span><span class="sxs-lookup"><span data-stu-id="a5674-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5674-106">权限</span><span class="sxs-lookup"><span data-stu-id="a5674-106">Permissions</span></span>

<span data-ttu-id="a5674-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5674-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5674-109">Permission type</span></span>      | <span data-ttu-id="a5674-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5674-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5674-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5674-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5674-112">TeamsAppInstallation.ReadWriteSelfForUser、TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="a5674-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="a5674-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5674-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5674-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5674-114">Not supported.</span></span>    |
|<span data-ttu-id="a5674-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5674-115">Application</span></span> | <span data-ttu-id="a5674-116">TeamsAppInstallation.ReadWriteSelfForUser.All、TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="a5674-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5674-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5674-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id | user-principal-name}/teamwork/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="a5674-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5674-118">Request headers</span></span>

| <span data-ttu-id="a5674-119">标头</span><span class="sxs-lookup"><span data-stu-id="a5674-119">Header</span></span>       | <span data-ttu-id="a5674-120">值</span><span class="sxs-lookup"><span data-stu-id="a5674-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5674-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5674-121">Authorization</span></span>  | <span data-ttu-id="a5674-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5674-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5674-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5674-124">Request body</span></span>

<span data-ttu-id="a5674-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5674-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5674-126">响应</span><span class="sxs-lookup"><span data-stu-id="a5674-126">Response</span></span>

<span data-ttu-id="a5674-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a5674-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5674-129">示例</span><span class="sxs-lookup"><span data-stu-id="a5674-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5674-130">请求</span><span class="sxs-lookup"><span data-stu-id="a5674-130">Request</span></span>

<span data-ttu-id="a5674-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a5674-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5674-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5674-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade
```
# <a name="c"></a>[<span data-ttu-id="a5674-133">C#</span><span class="sxs-lookup"><span data-stu-id="a5674-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5674-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5674-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5674-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5674-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5674-136">Java</span><span class="sxs-lookup"><span data-stu-id="a5674-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5674-137">响应</span><span class="sxs-lookup"><span data-stu-id="a5674-137">Response</span></span>

<span data-ttu-id="a5674-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a5674-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


