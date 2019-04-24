---
title: 删除 contactFolder
description: 删除默认 contactFolder 以外的 contactFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 01b8303723c4a59b8fdc4ac3f5d7d4f6cb491fd1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455648"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="19ead-103">删除 contactFolder</span><span class="sxs-lookup"><span data-stu-id="19ead-103">Delete contactFolder</span></span>

<span data-ttu-id="19ead-104">删除默认 contactFolder 以外的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="19ead-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="19ead-105">权限</span><span class="sxs-lookup"><span data-stu-id="19ead-105">Permissions</span></span>
<span data-ttu-id="19ead-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19ead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ead-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19ead-108">Permission type</span></span>      | <span data-ttu-id="19ead-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19ead-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19ead-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19ead-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19ead-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ead-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="19ead-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19ead-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ead-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ead-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="19ead-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19ead-114">Application</span></span> | <span data-ttu-id="19ead-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ead-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ead-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19ead-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="19ead-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="19ead-117">Request headers</span></span>
| <span data-ttu-id="19ead-118">名称</span><span class="sxs-lookup"><span data-stu-id="19ead-118">Name</span></span>       | <span data-ttu-id="19ead-119">类型</span><span class="sxs-lookup"><span data-stu-id="19ead-119">Type</span></span> | <span data-ttu-id="19ead-120">说明</span><span class="sxs-lookup"><span data-stu-id="19ead-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19ead-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ead-121">Authorization</span></span>  | <span data-ttu-id="19ead-122">string</span><span class="sxs-lookup"><span data-stu-id="19ead-122">string</span></span>  | <span data-ttu-id="19ead-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19ead-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19ead-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="19ead-125">Request body</span></span>
<span data-ttu-id="19ead-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19ead-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19ead-127">响应</span><span class="sxs-lookup"><span data-stu-id="19ead-127">Response</span></span>

<span data-ttu-id="19ead-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="19ead-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ead-130">示例</span><span class="sxs-lookup"><span data-stu-id="19ead-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19ead-131">请求</span><span class="sxs-lookup"><span data-stu-id="19ead-131">Request</span></span>
<span data-ttu-id="19ead-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19ead-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="19ead-133">响应</span><span class="sxs-lookup"><span data-stu-id="19ead-133">Response</span></span>
<span data-ttu-id="19ead-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19ead-134">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
