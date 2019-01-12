---
title: 创建页面
description: 在指定分区中新建页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8957609ffd3768edb456835b522dbbb7a145b6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912790"
---
# <a name="create-page"></a><span data-ttu-id="beaad-103">创建页面</span><span class="sxs-lookup"><span data-stu-id="beaad-103">Create page</span></span>

> <span data-ttu-id="beaad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="beaad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beaad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="beaad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="beaad-106">在指定分区中新建[页面](../resources/page.md)。</span><span class="sxs-lookup"><span data-stu-id="beaad-106">Create a new [page](../resources/page.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="beaad-107">权限</span><span class="sxs-lookup"><span data-stu-id="beaad-107">Permissions</span></span>
<span data-ttu-id="beaad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="beaad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beaad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="beaad-110">Permission type</span></span>      | <span data-ttu-id="beaad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="beaad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beaad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="beaad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="beaad-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beaad-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="beaad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="beaad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beaad-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="beaad-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="beaad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="beaad-116">Application</span></span> | <span data-ttu-id="beaad-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beaad-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="beaad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="beaad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="beaad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="beaad-119">Request headers</span></span>
| <span data-ttu-id="beaad-120">名称</span><span class="sxs-lookup"><span data-stu-id="beaad-120">Name</span></span>       | <span data-ttu-id="beaad-121">类型</span><span class="sxs-lookup"><span data-stu-id="beaad-121">Type</span></span> | <span data-ttu-id="beaad-122">说明</span><span class="sxs-lookup"><span data-stu-id="beaad-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="beaad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="beaad-123">Authorization</span></span>  | <span data-ttu-id="beaad-124">string</span><span class="sxs-lookup"><span data-stu-id="beaad-124">string</span></span>  | <span data-ttu-id="beaad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="beaad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="beaad-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="beaad-127">Content-Type</span></span> | <span data-ttu-id="beaad-128">string</span><span class="sxs-lookup"><span data-stu-id="beaad-128">string</span></span> | <span data-ttu-id="beaad-p104">HTML 内容（包括多部分请求必备的“演示”部分）的 `text/html` 或 `application/xhtml+xml`。多部分请求使用 `multipart/form-data; boundary=your-boundary` 内容类型。</span><span class="sxs-lookup"><span data-stu-id="beaad-p104">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beaad-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="beaad-131">Request body</span></span>
<span data-ttu-id="beaad-132">在请求正文中，提供页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="beaad-132">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="beaad-p105">正文可以将 HTML 直接置于请求正文中，或者其可以包含多部分消息格式，如示例中所示。如果要发送二进制数据，则必须发送多部分请求。</span><span class="sxs-lookup"><span data-stu-id="beaad-p105">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="beaad-135">响应</span><span class="sxs-lookup"><span data-stu-id="beaad-135">Response</span></span>

<span data-ttu-id="beaad-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新的 [page](../resources/page.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="beaad-136">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beaad-137">示例</span><span class="sxs-lookup"><span data-stu-id="beaad-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="beaad-138">请求</span><span class="sxs-lookup"><span data-stu-id="beaad-138">Request</span></span>
<span data-ttu-id="beaad-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="beaad-139">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```
##### <a name="response"></a><span data-ttu-id="beaad-140">响应</span><span class="sxs-lookup"><span data-stu-id="beaad-140">Response</span></span>
<span data-ttu-id="beaad-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="beaad-141">Here is an example of the response.</span></span> <span data-ttu-id="beaad-142">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="beaad-142">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="beaad-143">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="beaad-143">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
