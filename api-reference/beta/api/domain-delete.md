---
title: 删除域
description: 从租户中删除域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a870692e6a2710728dac4f2df55aaf8daf0eb95a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960124"
---
# <a name="delete-domain"></a><span data-ttu-id="b9dc6-103">删除域</span><span class="sxs-lookup"><span data-stu-id="b9dc6-103">Delete domain</span></span>

> <span data-ttu-id="b9dc6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9dc6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9dc6-106">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="b9dc6-107">**重要：** 不能恢复已删除的域。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9dc6-108">权限</span><span class="sxs-lookup"><span data-stu-id="b9dc6-108">Permissions</span></span>

<span data-ttu-id="b9dc6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9dc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9dc6-111">Permission type</span></span>      | <span data-ttu-id="b9dc6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9dc6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9dc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9dc6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9dc6-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9dc6-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9dc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9dc6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9dc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-116">Not supported.</span></span>    |
|<span data-ttu-id="b9dc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9dc6-117">Application</span></span> | <span data-ttu-id="b9dc6-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9dc6-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9dc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9dc6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="b9dc6-120">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9dc6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9dc6-121">Request headers</span></span>

| <span data-ttu-id="b9dc6-122">名称</span><span class="sxs-lookup"><span data-stu-id="b9dc6-122">Name</span></span>       | <span data-ttu-id="b9dc6-123">说明</span><span class="sxs-lookup"><span data-stu-id="b9dc6-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9dc6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9dc6-124">Authorization</span></span>  | <span data-ttu-id="b9dc6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9dc6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9dc6-127">Content-Type</span></span>  | <span data-ttu-id="b9dc6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9dc6-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9dc6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9dc6-129">Request body</span></span>

<span data-ttu-id="b9dc6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9dc6-131">响应</span><span class="sxs-lookup"><span data-stu-id="b9dc6-131">Response</span></span>

<span data-ttu-id="b9dc6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9dc6-134">示例</span><span class="sxs-lookup"><span data-stu-id="b9dc6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9dc6-135">请求</span><span class="sxs-lookup"><span data-stu-id="b9dc6-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="b9dc6-136">响应</span><span class="sxs-lookup"><span data-stu-id="b9dc6-136">Response</span></span>

<span data-ttu-id="b9dc6-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9dc6-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
