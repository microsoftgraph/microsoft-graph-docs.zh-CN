---
title: 删除域
description: 从租户中删除域。
ms.openlocfilehash: 2ed3772d767099e8ccd7fd5453c7a8231c9ea96c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044884"
---
# <a name="delete-domain"></a><span data-ttu-id="bb318-103">删除域</span><span class="sxs-lookup"><span data-stu-id="bb318-103">Delete domain</span></span>

> <span data-ttu-id="bb318-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bb318-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb318-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb318-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb318-106">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="bb318-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="bb318-107">**重要：** 不能恢复已删除的域。</span><span class="sxs-lookup"><span data-stu-id="bb318-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb318-108">权限</span><span class="sxs-lookup"><span data-stu-id="bb318-108">Permissions</span></span>

<span data-ttu-id="bb318-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb318-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bb318-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb318-111">Permission type</span></span>      | <span data-ttu-id="bb318-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb318-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb318-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb318-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bb318-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb318-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb318-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb318-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb318-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb318-116">Not supported.</span></span>    |
|<span data-ttu-id="bb318-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb318-117">Application</span></span> | <span data-ttu-id="bb318-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb318-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb318-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb318-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="bb318-120">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="bb318-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb318-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb318-121">Request headers</span></span>

| <span data-ttu-id="bb318-122">名称</span><span class="sxs-lookup"><span data-stu-id="bb318-122">Name</span></span>       | <span data-ttu-id="bb318-123">说明</span><span class="sxs-lookup"><span data-stu-id="bb318-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb318-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb318-124">Authorization</span></span>  | <span data-ttu-id="bb318-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb318-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb318-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb318-127">Content-Type</span></span>  | <span data-ttu-id="bb318-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bb318-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb318-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb318-129">Request body</span></span>

<span data-ttu-id="bb318-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb318-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb318-131">响应</span><span class="sxs-lookup"><span data-stu-id="bb318-131">Response</span></span>

<span data-ttu-id="bb318-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="bb318-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb318-134">示例</span><span class="sxs-lookup"><span data-stu-id="bb318-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb318-135">请求</span><span class="sxs-lookup"><span data-stu-id="bb318-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="bb318-136">响应</span><span class="sxs-lookup"><span data-stu-id="bb318-136">Response</span></span>

<span data-ttu-id="bb318-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb318-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->