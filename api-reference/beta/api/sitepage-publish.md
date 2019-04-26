---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: 发布页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9bf699c0038e785a11560ee7326cfb2324345f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335886"
---
# <a name="sitepage-publish"></a><span data-ttu-id="d2d0d-102">sitePage: 发布</span><span class="sxs-lookup"><span data-stu-id="d2d0d-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2d0d-103">发布[sitePage][]资源的最新版本, 使页面的版本可供所有用户使用。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="d2d0d-104">如果该页面已签出, 请签入该页面并发布它。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="d2d0d-105">如果页面已签出到此 API 的调用方, 则会自动签入并发布该页面。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="d2d0d-107">权限</span><span class="sxs-lookup"><span data-stu-id="d2d0d-107">Permissions</span></span>

<span data-ttu-id="d2d0d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d0d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2d0d-110">Permission type</span></span>      | <span data-ttu-id="d2d0d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2d0d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2d0d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2d0d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2d0d-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d0d-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2d0d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2d0d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d0d-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d0d-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2d0d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2d0d-116">Application</span></span> | <span data-ttu-id="d2d0d-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d0d-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2d0d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2d0d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="d2d0d-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2d0d-119">Request body</span></span>

<span data-ttu-id="d2d0d-120">此邮件没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-120">This message does not have a request body.</span></span> <span data-ttu-id="d2d0d-121">发送的任何请求正文都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="d2d0d-122">响应</span><span class="sxs-lookup"><span data-stu-id="d2d0d-122">Response</span></span>

<span data-ttu-id="d2d0d-123">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="d2d0d-123">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->
