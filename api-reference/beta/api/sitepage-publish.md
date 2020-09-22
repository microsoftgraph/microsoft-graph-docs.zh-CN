---
author: rahmit
description: 发布 sitePage 资源的最新版本，使页面的版本可供所有用户使用。 如果该页面已签出，请签入该页面并发布它。 如果页面已签出到此 API 的调用方，则会自动签入并发布该页面。
ms.date: 09/10/2018
title: 发布页面
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e40f864ce224916a2c60e5c82e0aecbfff213fbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044377"
---
# <a name="sitepage-publish"></a><span data-ttu-id="28145-105">sitePage：发布</span><span class="sxs-lookup"><span data-stu-id="28145-105">sitePage: publish</span></span>

<span data-ttu-id="28145-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28145-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28145-107">发布 [sitePage][] 资源的最新版本，使页面的版本可供所有用户使用。</span><span class="sxs-lookup"><span data-stu-id="28145-107">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="28145-108">如果该页面已签出，请签入该页面并发布它。</span><span class="sxs-lookup"><span data-stu-id="28145-108">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="28145-109">如果页面已签出到此 API 的调用方，则会自动签入并发布该页面。</span><span class="sxs-lookup"><span data-stu-id="28145-109">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="28145-111">权限</span><span class="sxs-lookup"><span data-stu-id="28145-111">Permissions</span></span>

<span data-ttu-id="28145-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28145-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28145-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="28145-114">Permission type</span></span>      | <span data-ttu-id="28145-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28145-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28145-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28145-116">Delegated (work or school account)</span></span> | <span data-ttu-id="28145-117">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28145-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="28145-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28145-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28145-119">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28145-119">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="28145-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="28145-120">Application</span></span> | <span data-ttu-id="28145-121">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28145-121">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28145-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28145-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="28145-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="28145-123">Request body</span></span>

<span data-ttu-id="28145-124">此邮件没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="28145-124">This message does not have a request body.</span></span> <span data-ttu-id="28145-125">发送的任何请求正文都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="28145-125">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="28145-126">响应</span><span class="sxs-lookup"><span data-stu-id="28145-126">Response</span></span>

<span data-ttu-id="28145-127">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="28145-127">If successful, the API call returns a `204 No Content`.</span></span>

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


