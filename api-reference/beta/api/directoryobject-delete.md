---
title: 删除 directoryObject
description: 删除 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8bf24eae152fb31c766f2b395d2c6c37e2c91ddd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326055"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="5be7c-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="5be7c-103">Delete directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5be7c-104">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="5be7c-104">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="5be7c-105">权限</span><span class="sxs-lookup"><span data-stu-id="5be7c-105">Permissions</span></span>
<span data-ttu-id="5be7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5be7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5be7c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5be7c-108">Permission type</span></span>      | <span data-ttu-id="5be7c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5be7c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5be7c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5be7c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5be7c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5be7c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5be7c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5be7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5be7c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5be7c-113">Not supported.</span></span>    |
|<span data-ttu-id="5be7c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5be7c-114">Application</span></span> | <span data-ttu-id="5be7c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5be7c-115">Not supported.</span></span> |

<span data-ttu-id="5be7c-116">**注意：** 用户、组和联系人是 directory 对象的类型。</span><span class="sxs-lookup"><span data-stu-id="5be7c-116">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="5be7c-117">因此, 如果需要删除用户, 可以且应使用以下权限: User. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="5be7c-117">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="5be7c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5be7c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5be7c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5be7c-119">Request headers</span></span>
| <span data-ttu-id="5be7c-120">名称</span><span class="sxs-lookup"><span data-stu-id="5be7c-120">Name</span></span>       | <span data-ttu-id="5be7c-121">类型</span><span class="sxs-lookup"><span data-stu-id="5be7c-121">Type</span></span> | <span data-ttu-id="5be7c-122">说明</span><span class="sxs-lookup"><span data-stu-id="5be7c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5be7c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5be7c-123">Authorization</span></span>  | <span data-ttu-id="5be7c-124">string</span><span class="sxs-lookup"><span data-stu-id="5be7c-124">string</span></span>  | <span data-ttu-id="5be7c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5be7c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5be7c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5be7c-127">Request body</span></span>
<span data-ttu-id="5be7c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5be7c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5be7c-129">响应</span><span class="sxs-lookup"><span data-stu-id="5be7c-129">Response</span></span>

<span data-ttu-id="5be7c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5be7c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5be7c-132">示例</span><span class="sxs-lookup"><span data-stu-id="5be7c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5be7c-133">请求</span><span class="sxs-lookup"><span data-stu-id="5be7c-133">Request</span></span>
<span data-ttu-id="5be7c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5be7c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="5be7c-135">响应</span><span class="sxs-lookup"><span data-stu-id="5be7c-135">Response</span></span>
<span data-ttu-id="5be7c-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5be7c-136">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
