---
title: 创建页面
description: 在默认笔记本的默认分区中新建 OneNote 页面。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d82971bdb3b1e8db4c89e69880681c43ab913939
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965206"
---
# <a name="create-page"></a><span data-ttu-id="faf1c-103">创建页面</span><span class="sxs-lookup"><span data-stu-id="faf1c-103">Create page</span></span>

> <span data-ttu-id="faf1c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="faf1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faf1c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="faf1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faf1c-106">在默认笔记本的默认分区中新建 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="faf1c-106">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="faf1c-p102">若要在默认笔记本的不同分区中创建页面，可以使用 `sectionName` 查询参数。示例：`../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="faf1c-p102">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="faf1c-p103">`POST /onenote/pages` 操作仅用于在当前用户的默认笔记本中创建页面。如果你将其他笔记本作为目标，则可以[在指定分区中创建页面](../api/section-post-pages.md)。</span><span class="sxs-lookup"><span data-stu-id="faf1c-p103">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="faf1c-111">权限</span><span class="sxs-lookup"><span data-stu-id="faf1c-111">Permissions</span></span>
<span data-ttu-id="faf1c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="faf1c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf1c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="faf1c-114">Permission type</span></span>      | <span data-ttu-id="faf1c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="faf1c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faf1c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faf1c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="faf1c-117">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf1c-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="faf1c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faf1c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faf1c-119">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="faf1c-119">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="faf1c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="faf1c-120">Application</span></span> | <span data-ttu-id="faf1c-121">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf1c-121">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="faf1c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faf1c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="faf1c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="faf1c-123">Request headers</span></span>  
| <span data-ttu-id="faf1c-124">名称</span><span class="sxs-lookup"><span data-stu-id="faf1c-124">Name</span></span>       | <span data-ttu-id="faf1c-125">类型</span><span class="sxs-lookup"><span data-stu-id="faf1c-125">Type</span></span> | <span data-ttu-id="faf1c-126">说明</span><span class="sxs-lookup"><span data-stu-id="faf1c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="faf1c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="faf1c-127">Authorization</span></span>  | <span data-ttu-id="faf1c-128">string</span><span class="sxs-lookup"><span data-stu-id="faf1c-128">string</span></span>  | <span data-ttu-id="faf1c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="faf1c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="faf1c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="faf1c-131">Content-Type</span></span> | <span data-ttu-id="faf1c-132">string</span><span class="sxs-lookup"><span data-stu-id="faf1c-132">string</span></span> | <span data-ttu-id="faf1c-p106">HTML 内容（包括多部分请求必备的“演示”部分）的 `text/html` 或 `application/xhtml+xml`。多部分请求使用 `multipart/form-data; boundary=your-boundary` 内容类型。</span><span class="sxs-lookup"><span data-stu-id="faf1c-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="faf1c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="faf1c-135">Request body</span></span>
<span data-ttu-id="faf1c-136">在请求正文中，提供页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="faf1c-136">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="faf1c-p107">正文可以将 HTML 直接置于请求正文中，或者其可以包含多部分消息格式，如示例中所示。如果要发送二进制数据，则必须发送多部分请求。</span><span class="sxs-lookup"><span data-stu-id="faf1c-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="faf1c-139">响应</span><span class="sxs-lookup"><span data-stu-id="faf1c-139">Response</span></span>

<span data-ttu-id="faf1c-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新的 [page](../resources/page.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="faf1c-140">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf1c-141">示例</span><span class="sxs-lookup"><span data-stu-id="faf1c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="faf1c-142">请求</span><span class="sxs-lookup"><span data-stu-id="faf1c-142">Request</span></span>
<span data-ttu-id="faf1c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="faf1c-143">Here is an example of the request.</span></span>

<span data-ttu-id="faf1c-p108">在 `../onenote/pages` 路径下，可以使用 `sectionName` 查询参数在默认笔记本的特定分区中创建页面。示例：`../onenote/pages?sectionName=My%20section`。如果分区不存在（或已重命名），API 将创建新的分区。</span><span class="sxs-lookup"><span data-stu-id="faf1c-p108">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages
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
##### <a name="response"></a><span data-ttu-id="faf1c-147">响应</span><span class="sxs-lookup"><span data-stu-id="faf1c-147">Response</span></span>
<span data-ttu-id="faf1c-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="faf1c-148">Here is an example of the response.</span></span> <span data-ttu-id="faf1c-149">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="faf1c-149">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="faf1c-150">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="faf1c-150">All of the properties will be returned from an actual call.</span></span>
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
  "content": "content-value",
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
