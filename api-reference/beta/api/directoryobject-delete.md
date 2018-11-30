---
title: 删除 directoryObject
description: 删除 directoryObject。
ms.openlocfilehash: a1377b0493c5c8a6833225faf33a16f596a23240
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044580"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="3e5b2-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="3e5b2-103">Delete directoryObject</span></span>

> <span data-ttu-id="3e5b2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e5b2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e5b2-106">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e5b2-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e5b2-107">Permissions</span></span>
<span data-ttu-id="3e5b2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3e5b2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e5b2-110">Permission type</span></span>      | <span data-ttu-id="3e5b2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e5b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e5b2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e5b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e5b2-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e5b2-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e5b2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e5b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e5b2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-115">Not supported.</span></span>    |
|<span data-ttu-id="3e5b2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e5b2-116">Application</span></span> | <span data-ttu-id="3e5b2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-117">Not supported.</span></span> |

<span data-ttu-id="3e5b2-118">**注意：** 用户、 组和联系人是目录对象的类型。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="3e5b2-119">因此，如果您需要删除用户，则以下权限将可以应使用： User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e5b2-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="3e5b2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e5b2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3e5b2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e5b2-121">Request headers</span></span>
| <span data-ttu-id="3e5b2-122">名称</span><span class="sxs-lookup"><span data-stu-id="3e5b2-122">Name</span></span>       | <span data-ttu-id="3e5b2-123">类型</span><span class="sxs-lookup"><span data-stu-id="3e5b2-123">Type</span></span> | <span data-ttu-id="3e5b2-124">说明</span><span class="sxs-lookup"><span data-stu-id="3e5b2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e5b2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e5b2-125">Authorization</span></span>  | <span data-ttu-id="3e5b2-126">string</span><span class="sxs-lookup"><span data-stu-id="3e5b2-126">string</span></span>  | <span data-ttu-id="3e5b2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e5b2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e5b2-129">Request body</span></span>
<span data-ttu-id="3e5b2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e5b2-131">响应</span><span class="sxs-lookup"><span data-stu-id="3e5b2-131">Response</span></span>

<span data-ttu-id="3e5b2-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e5b2-134">示例</span><span class="sxs-lookup"><span data-stu-id="3e5b2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e5b2-135">请求</span><span class="sxs-lookup"><span data-stu-id="3e5b2-135">Request</span></span>
<span data-ttu-id="3e5b2-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="3e5b2-137">响应</span><span class="sxs-lookup"><span data-stu-id="3e5b2-137">Response</span></span>
<span data-ttu-id="3e5b2-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e5b2-138">Here is an example of the response.</span></span> 
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