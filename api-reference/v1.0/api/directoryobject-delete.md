---
title: 删除 directoryObject
description: 删除 directoryObject。
ms.openlocfilehash: 2ecd16163a7241b34adc74ebc1aa8c11406cb800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011005"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="bbb09-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="bbb09-103">Delete directoryObject</span></span>

<span data-ttu-id="bbb09-104">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="bbb09-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbb09-105">权限</span><span class="sxs-lookup"><span data-stu-id="bbb09-105">Permissions</span></span>
<span data-ttu-id="bbb09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbb09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bbb09-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbb09-108">Permission type</span></span>      | <span data-ttu-id="bbb09-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbb09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbb09-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbb09-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbb09-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bbb09-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bbb09-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbb09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbb09-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbb09-113">Not supported.</span></span>    |
|<span data-ttu-id="bbb09-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbb09-114">Application</span></span> | <span data-ttu-id="bbb09-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbb09-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbb09-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbb09-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bbb09-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbb09-117">Request headers</span></span>
| <span data-ttu-id="bbb09-118">名称</span><span class="sxs-lookup"><span data-stu-id="bbb09-118">Name</span></span>       | <span data-ttu-id="bbb09-119">类型</span><span class="sxs-lookup"><span data-stu-id="bbb09-119">Type</span></span> | <span data-ttu-id="bbb09-120">说明</span><span class="sxs-lookup"><span data-stu-id="bbb09-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bbb09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbb09-121">Authorization</span></span>  | <span data-ttu-id="bbb09-122">string</span><span class="sxs-lookup"><span data-stu-id="bbb09-122">string</span></span>  | <span data-ttu-id="bbb09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbb09-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbb09-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbb09-125">Request body</span></span>
<span data-ttu-id="bbb09-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbb09-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbb09-127">响应</span><span class="sxs-lookup"><span data-stu-id="bbb09-127">Response</span></span>

<span data-ttu-id="bbb09-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bbb09-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb09-130">示例</span><span class="sxs-lookup"><span data-stu-id="bbb09-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbb09-131">请求</span><span class="sxs-lookup"><span data-stu-id="bbb09-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="bbb09-132">响应</span><span class="sxs-lookup"><span data-stu-id="bbb09-132">Response</span></span>

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