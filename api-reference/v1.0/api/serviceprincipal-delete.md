---
title: 删除 servicePrincipal
description: 删除 servicePrincipal。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ff4806499b2c32b88ee87f6a1e33691e25f4f25a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291165"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="37f22-103">删除 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="37f22-103">Delete servicePrincipal</span></span>

<span data-ttu-id="37f22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37f22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37f22-105">删除[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="37f22-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37f22-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="37f22-106">Permissions</span></span>
<span data-ttu-id="37f22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f22-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="37f22-109">Permission type</span></span>      | <span data-ttu-id="37f22-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37f22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37f22-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37f22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37f22-112">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="37f22-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37f22-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37f22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37f22-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f22-114">Not supported.</span></span>    |
|<span data-ttu-id="37f22-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="37f22-115">Application</span></span> | <span data-ttu-id="37f22-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="37f22-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37f22-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37f22-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="37f22-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="37f22-118">Request headers</span></span>
| <span data-ttu-id="37f22-119">名称</span><span class="sxs-lookup"><span data-stu-id="37f22-119">Name</span></span>       | <span data-ttu-id="37f22-120">说明</span><span class="sxs-lookup"><span data-stu-id="37f22-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="37f22-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f22-121">Authorization</span></span> | <span data-ttu-id="37f22-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37f22-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37f22-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="37f22-124">Content-type</span></span> | <span data-ttu-id="37f22-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="37f22-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37f22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37f22-127">Request body</span></span>
<span data-ttu-id="37f22-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37f22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37f22-129">响应</span><span class="sxs-lookup"><span data-stu-id="37f22-129">Response</span></span>

<span data-ttu-id="37f22-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="37f22-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37f22-132">示例</span><span class="sxs-lookup"><span data-stu-id="37f22-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="37f22-133">请求</span><span class="sxs-lookup"><span data-stu-id="37f22-133">Request</span></span>
<span data-ttu-id="37f22-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37f22-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
### <a name="response"></a><span data-ttu-id="37f22-135">响应</span><span class="sxs-lookup"><span data-stu-id="37f22-135">Response</span></span>
<span data-ttu-id="37f22-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="37f22-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
