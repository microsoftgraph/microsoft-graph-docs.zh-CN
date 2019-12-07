---
title: 删除 openShiftChangeRequest
description: 删除 openShiftChangeRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b3370a17b6f16351b3a9db944f9ae636560fe3a
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895599"
---
# <a name="delete-openshiftchangerequest"></a><span data-ttu-id="1798d-103">删除 openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="1798d-103">Delete openShiftChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1798d-104">删除[openShiftChangeRequest](../resources/openshiftchangerequest.md)。</span><span class="sxs-lookup"><span data-stu-id="1798d-104">Delete an [openShiftChangeRequest](../resources/openshiftchangerequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1798d-105">权限</span><span class="sxs-lookup"><span data-stu-id="1798d-105">Permissions</span></span>

<span data-ttu-id="1798d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1798d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1798d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1798d-108">Permission type</span></span>                        | <span data-ttu-id="1798d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1798d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1798d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1798d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1798d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1798d-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1798d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1798d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1798d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1798d-113">Not supported.</span></span> |
| <span data-ttu-id="1798d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1798d-114">Application</span></span>                            | <span data-ttu-id="1798d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1798d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1798d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1798d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="1798d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1798d-117">Request headers</span></span>

| <span data-ttu-id="1798d-118">名称</span><span class="sxs-lookup"><span data-stu-id="1798d-118">Name</span></span>          | <span data-ttu-id="1798d-119">说明</span><span class="sxs-lookup"><span data-stu-id="1798d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1798d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1798d-120">Authorization</span></span> | <span data-ttu-id="1798d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1798d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1798d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1798d-123">Request body</span></span>

<span data-ttu-id="1798d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1798d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1798d-125">响应</span><span class="sxs-lookup"><span data-stu-id="1798d-125">Response</span></span>

<span data-ttu-id="1798d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1798d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1798d-128">示例</span><span class="sxs-lookup"><span data-stu-id="1798d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1798d-129">请求</span><span class="sxs-lookup"><span data-stu-id="1798d-129">Request</span></span>

<span data-ttu-id="1798d-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1798d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_openshiftchangerequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="1798d-131">响应</span><span class="sxs-lookup"><span data-stu-id="1798d-131">Response</span></span>

<span data-ttu-id="1798d-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1798d-132">The following is an example of the response.</span></span>

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
  "description": "Delete openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
