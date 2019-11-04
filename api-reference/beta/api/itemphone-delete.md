---
title: 删除 itemPhone
description: 从用户的配置文件中删除 itemPhone 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 87f7f468fbaf8de25dd1fdabd6840f85409e6822
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938006"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="8f47d-103">删除 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8f47d-103">Delete itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f47d-104">从用户的[配置文件](../resources/profile.md)中删除[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8f47d-104">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f47d-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f47d-105">Permissions</span></span>

<span data-ttu-id="8f47d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f47d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f47d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f47d-108">Permission type</span></span>                        | <span data-ttu-id="8f47d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f47d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f47d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f47d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f47d-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="8f47d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8f47d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f47d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f47d-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="8f47d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8f47d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f47d-114">Application</span></span>                            | <span data-ttu-id="8f47d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f47d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8f47d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f47d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f47d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f47d-117">Request headers</span></span>

| <span data-ttu-id="8f47d-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f47d-118">Name</span></span>           |<span data-ttu-id="8f47d-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f47d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8f47d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f47d-120">Authorization</span></span>  | <span data-ttu-id="8f47d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f47d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8f47d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f47d-123">Content-Type</span></span>   | <span data-ttu-id="8f47d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8f47d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f47d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f47d-126">Request body</span></span>

<span data-ttu-id="8f47d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f47d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f47d-128">响应</span><span class="sxs-lookup"><span data-stu-id="8f47d-128">Response</span></span>

<span data-ttu-id="8f47d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f47d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f47d-131">示例</span><span class="sxs-lookup"><span data-stu-id="8f47d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f47d-132">请求</span><span class="sxs-lookup"><span data-stu-id="8f47d-132">Request</span></span>

<span data-ttu-id="8f47d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8f47d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/phones/{id}
```

### <a name="response"></a><span data-ttu-id="8f47d-134">响应</span><span class="sxs-lookup"><span data-stu-id="8f47d-134">Response</span></span>

<span data-ttu-id="8f47d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f47d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->