---
title: 删除 directoryObject
description: 删除 directoryObject。
author: lleonard-msft
ms.openlocfilehash: dec525e72b523e7bbe95996d4c863c68e01baa15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313200"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="3c9f8-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="3c9f8-103">Delete directoryObject</span></span>

<span data-ttu-id="3c9f8-104">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c9f8-105">权限</span><span class="sxs-lookup"><span data-stu-id="3c9f8-105">Permissions</span></span>
<span data-ttu-id="3c9f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3c9f8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c9f8-108">Permission type</span></span>      | <span data-ttu-id="3c9f8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c9f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c9f8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c9f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c9f8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c9f8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c9f8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c9f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c9f8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-113">Not supported.</span></span>    |
|<span data-ttu-id="3c9f8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c9f8-114">Application</span></span> | <span data-ttu-id="3c9f8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c9f8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c9f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3c9f8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c9f8-117">Request headers</span></span>
| <span data-ttu-id="3c9f8-118">Name</span><span class="sxs-lookup"><span data-stu-id="3c9f8-118">Name</span></span>       | <span data-ttu-id="3c9f8-119">类型</span><span class="sxs-lookup"><span data-stu-id="3c9f8-119">Type</span></span> | <span data-ttu-id="3c9f8-120">说明</span><span class="sxs-lookup"><span data-stu-id="3c9f8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c9f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c9f8-121">Authorization</span></span>  | <span data-ttu-id="3c9f8-122">string</span><span class="sxs-lookup"><span data-stu-id="3c9f8-122">string</span></span>  | <span data-ttu-id="3c9f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c9f8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c9f8-125">Request body</span></span>
<span data-ttu-id="3c9f8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c9f8-127">响应</span><span class="sxs-lookup"><span data-stu-id="3c9f8-127">Response</span></span>

<span data-ttu-id="3c9f8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c9f8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c9f8-130">示例</span><span class="sxs-lookup"><span data-stu-id="3c9f8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c9f8-131">请求</span><span class="sxs-lookup"><span data-stu-id="3c9f8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="3c9f8-132">响应</span><span class="sxs-lookup"><span data-stu-id="3c9f8-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->