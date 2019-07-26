---
title: 'teamsAppInstallation: upgrade'
description: 在用户的个人作用域中升级应用程序安装
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7461c6e320ffcacc0d26ccffe90681ab6215db15
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908535"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="b04b8-103">teamsAppInstallation: upgrade</span><span class="sxs-lookup"><span data-stu-id="b04b8-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b04b8-104">将指定[用户](../resources/user.md)的个人作用域中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b04b8-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="b04b8-105">权限</span><span class="sxs-lookup"><span data-stu-id="b04b8-105">Permissions</span></span>

<span data-ttu-id="b04b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b04b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b04b8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b04b8-108">Permission type</span></span>      | <span data-ttu-id="b04b8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b04b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b04b8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b04b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b04b8-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b04b8-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="b04b8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b04b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b04b8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b04b8-113">Not supported.</span></span>    |
|<span data-ttu-id="b04b8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b04b8-114">Application</span></span> | <span data-ttu-id="b04b8-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b04b8-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b04b8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b04b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="b04b8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b04b8-117">Request headers</span></span>

| <span data-ttu-id="b04b8-118">标头</span><span class="sxs-lookup"><span data-stu-id="b04b8-118">Header</span></span>       | <span data-ttu-id="b04b8-119">值</span><span class="sxs-lookup"><span data-stu-id="b04b8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b04b8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b04b8-120">Authorization</span></span>  | <span data-ttu-id="b04b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b04b8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b04b8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b04b8-123">Request body</span></span>

<span data-ttu-id="b04b8-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b04b8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b04b8-125">响应</span><span class="sxs-lookup"><span data-stu-id="b04b8-125">Response</span></span>

<span data-ttu-id="b04b8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b04b8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b04b8-128">示例</span><span class="sxs-lookup"><span data-stu-id="b04b8-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="b04b8-129">请求</span><span class="sxs-lookup"><span data-stu-id="b04b8-129">Request</span></span>

<span data-ttu-id="b04b8-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b04b8-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="b04b8-131">响应</span><span class="sxs-lookup"><span data-stu-id="b04b8-131">Response</span></span>

<span data-ttu-id="b04b8-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b04b8-132">The following is an example of the response.</span></span>

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
