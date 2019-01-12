---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: 发布页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e59a7aea74e165945757f2513102a66baf64be1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920238"
---
# <a name="sitepage-publish"></a><span data-ttu-id="1a087-102">sitePage： 发布</span><span class="sxs-lookup"><span data-stu-id="1a087-102">sitePage: publish</span></span>

> <span data-ttu-id="1a087-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a087-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a087-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a087-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a087-105">发布[sitePage][]资源，使页面的版本可供所有用户的最新版本。</span><span class="sxs-lookup"><span data-stu-id="1a087-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="1a087-106">如果页已签出，签入此页面并将其发布。</span><span class="sxs-lookup"><span data-stu-id="1a087-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="1a087-107">如果页已签出到此 api 呼叫者，页是自动签入，然后发布。</span><span class="sxs-lookup"><span data-stu-id="1a087-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="1a087-109">权限</span><span class="sxs-lookup"><span data-stu-id="1a087-109">Permissions</span></span>

<span data-ttu-id="1a087-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a087-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a087-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a087-112">Permission type</span></span>      | <span data-ttu-id="1a087-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a087-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a087-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a087-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1a087-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a087-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a087-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a087-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a087-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a087-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a087-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a087-118">Application</span></span> | <span data-ttu-id="1a087-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a087-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a087-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a087-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="1a087-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a087-121">Request body</span></span>

<span data-ttu-id="1a087-122">此消息没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a087-122">This message does not have a request body.</span></span> <span data-ttu-id="1a087-123">发送任何请求正文将被忽略。</span><span class="sxs-lookup"><span data-stu-id="1a087-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="1a087-124">响应</span><span class="sxs-lookup"><span data-stu-id="1a087-124">Response</span></span>

<span data-ttu-id="1a087-125">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="1a087-125">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
