---
title: 删除 directoryObject
description: 删除 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: e291004f13eaf6d0f24750002c8068d3e97b3052
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865194"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="391f4-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="391f4-103">Delete directoryObject</span></span>

> <span data-ttu-id="391f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="391f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="391f4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="391f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="391f4-106">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="391f4-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="391f4-107">权限</span><span class="sxs-lookup"><span data-stu-id="391f4-107">Permissions</span></span>
<span data-ttu-id="391f4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="391f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="391f4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="391f4-110">Permission type</span></span>      | <span data-ttu-id="391f4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="391f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="391f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="391f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="391f4-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="391f4-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="391f4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="391f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="391f4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="391f4-115">Not supported.</span></span>    |
|<span data-ttu-id="391f4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="391f4-116">Application</span></span> | <span data-ttu-id="391f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="391f4-117">Not supported.</span></span> |

<span data-ttu-id="391f4-118">**注意：** 用户、 组和联系人是目录对象的类型。</span><span class="sxs-lookup"><span data-stu-id="391f4-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="391f4-119">因此，如果您需要删除用户，则以下权限将可以应使用： User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391f4-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="391f4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="391f4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="391f4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="391f4-121">Request headers</span></span>
| <span data-ttu-id="391f4-122">名称</span><span class="sxs-lookup"><span data-stu-id="391f4-122">Name</span></span>       | <span data-ttu-id="391f4-123">类型</span><span class="sxs-lookup"><span data-stu-id="391f4-123">Type</span></span> | <span data-ttu-id="391f4-124">说明</span><span class="sxs-lookup"><span data-stu-id="391f4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="391f4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="391f4-125">Authorization</span></span>  | <span data-ttu-id="391f4-126">string</span><span class="sxs-lookup"><span data-stu-id="391f4-126">string</span></span>  | <span data-ttu-id="391f4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="391f4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="391f4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="391f4-129">Request body</span></span>
<span data-ttu-id="391f4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="391f4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="391f4-131">响应</span><span class="sxs-lookup"><span data-stu-id="391f4-131">Response</span></span>

<span data-ttu-id="391f4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="391f4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="391f4-134">示例</span><span class="sxs-lookup"><span data-stu-id="391f4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="391f4-135">请求</span><span class="sxs-lookup"><span data-stu-id="391f4-135">Request</span></span>
<span data-ttu-id="391f4-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="391f4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="391f4-137">响应</span><span class="sxs-lookup"><span data-stu-id="391f4-137">Response</span></span>
<span data-ttu-id="391f4-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="391f4-138">Here is an example of the response.</span></span> 
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
