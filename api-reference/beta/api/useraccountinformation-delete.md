---
title: 删除 userAccountInformation
description: 删除 userAccountInformation 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1cd1130b89104f1154425e94443a45e375012a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451579"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="07ec3-103">删除 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="07ec3-103">Delete userAccountInformation</span></span>

<span data-ttu-id="07ec3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="07ec3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07ec3-105">从用户的[配置文件](../resources/profile.md)中删除[userAccountInformation](../resources/useraccountinformation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="07ec3-105">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="07ec3-106">权限</span><span class="sxs-lookup"><span data-stu-id="07ec3-106">Permissions</span></span>

<span data-ttu-id="07ec3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07ec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07ec3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="07ec3-109">Permission type</span></span>                        | <span data-ttu-id="07ec3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07ec3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="07ec3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07ec3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="07ec3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="07ec3-112">Not supported.</span></span>                              |
| <span data-ttu-id="07ec3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07ec3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07ec3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="07ec3-114">Not supported.</span></span>                              |
| <span data-ttu-id="07ec3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="07ec3-115">Application</span></span>                            | <span data-ttu-id="07ec3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07ec3-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="07ec3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07ec3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="07ec3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="07ec3-118">Request headers</span></span>

| <span data-ttu-id="07ec3-119">名称</span><span class="sxs-lookup"><span data-stu-id="07ec3-119">Name</span></span>           |<span data-ttu-id="07ec3-120">说明</span><span class="sxs-lookup"><span data-stu-id="07ec3-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="07ec3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="07ec3-121">Authorization</span></span>  | <span data-ttu-id="07ec3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07ec3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07ec3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="07ec3-124">Request body</span></span>

<span data-ttu-id="07ec3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="07ec3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07ec3-126">响应</span><span class="sxs-lookup"><span data-stu-id="07ec3-126">Response</span></span>

<span data-ttu-id="07ec3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="07ec3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07ec3-129">示例</span><span class="sxs-lookup"><span data-stu-id="07ec3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07ec3-130">请求</span><span class="sxs-lookup"><span data-stu-id="07ec3-130">Request</span></span>

<span data-ttu-id="07ec3-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07ec3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="07ec3-132">响应</span><span class="sxs-lookup"><span data-stu-id="07ec3-132">Response</span></span>

<span data-ttu-id="07ec3-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07ec3-133">The following is an example of the response.</span></span>

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
  "description": "Delete userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
