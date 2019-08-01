---
title: 创建页面
description: 在默认笔记本的默认分区中创建新的 OneNote 页面。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9db168bda1c79232bb18b76464732e10e75331e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976367"
---
# <a name="create-page"></a><span data-ttu-id="ed18a-103">创建页面</span><span class="sxs-lookup"><span data-stu-id="ed18a-103">Create page</span></span>

<span data-ttu-id="ed18a-104">在默认笔记本的默认分区中创建新的 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="ed18a-104">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="ed18a-105">若要在默认笔记本的不同节中创建页面, 可以使用`sectionName`查询参数。</span><span class="sxs-lookup"><span data-stu-id="ed18a-105">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.</span></span>  <span data-ttu-id="ed18a-106">示例：`../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="ed18a-106">Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="ed18a-107">该`POST /onenote/pages`操作仅用于在当前用户的默认笔记本中创建页面。</span><span class="sxs-lookup"><span data-stu-id="ed18a-107">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook.</span></span> <span data-ttu-id="ed18a-108">如果要将其他笔记本作为目标, 可以[在指定分区中创建页面](../api/section-post-pages.md)。</span><span class="sxs-lookup"><span data-stu-id="ed18a-108">If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="ed18a-109">权限</span><span class="sxs-lookup"><span data-stu-id="ed18a-109">Permissions</span></span>
<span data-ttu-id="ed18a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed18a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed18a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed18a-112">Permission type</span></span>      | <span data-ttu-id="ed18a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed18a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed18a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed18a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ed18a-115">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed18a-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed18a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed18a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed18a-117">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed18a-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ed18a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed18a-118">Application</span></span> | <span data-ttu-id="ed18a-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed18a-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed18a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed18a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="ed18a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed18a-121">Request headers</span></span>  
| <span data-ttu-id="ed18a-122">名称</span><span class="sxs-lookup"><span data-stu-id="ed18a-122">Name</span></span>       | <span data-ttu-id="ed18a-123">类型</span><span class="sxs-lookup"><span data-stu-id="ed18a-123">Type</span></span> | <span data-ttu-id="ed18a-124">说明</span><span class="sxs-lookup"><span data-stu-id="ed18a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed18a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed18a-125">Authorization</span></span>  | <span data-ttu-id="ed18a-126">string</span><span class="sxs-lookup"><span data-stu-id="ed18a-126">string</span></span>  | <span data-ttu-id="ed18a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed18a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed18a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed18a-129">Content-Type</span></span> | <span data-ttu-id="ed18a-130">string</span><span class="sxs-lookup"><span data-stu-id="ed18a-130">string</span></span> | <span data-ttu-id="ed18a-p105">HTML 内容（包括多部分请求必备的“演示”部分）的 `text/html` 或 `application/xhtml+xml`。多部分请求使用 `multipart/form-data; boundary=your-boundary` 内容类型。</span><span class="sxs-lookup"><span data-stu-id="ed18a-p105">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed18a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed18a-133">Request body</span></span>
<span data-ttu-id="ed18a-134">在请求正文中, 提供页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="ed18a-134">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="ed18a-p106">正文可以将 HTML 直接置于请求正文中，或者其可以包含多部分消息格式，如示例中所示。如果要发送二进制数据，则必须发送多部分请求。</span><span class="sxs-lookup"><span data-stu-id="ed18a-p106">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="ed18a-137">响应</span><span class="sxs-lookup"><span data-stu-id="ed18a-137">Response</span></span>

<span data-ttu-id="ed18a-138">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[page](../resources/page.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ed18a-138">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed18a-139">示例</span><span class="sxs-lookup"><span data-stu-id="ed18a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed18a-140">请求</span><span class="sxs-lookup"><span data-stu-id="ed18a-140">Request</span></span>
<span data-ttu-id="ed18a-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed18a-141">Here is an example of the request.</span></span>

<span data-ttu-id="ed18a-142">在`../onenote/pages`路径中, 可以使用`sectionName`查询参数在默认笔记本的特定节中创建页面。</span><span class="sxs-lookup"><span data-stu-id="ed18a-142">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook.</span></span> <span data-ttu-id="ed18a-143">示例：`../onenote/pages?sectionName=My%20section`。</span><span class="sxs-lookup"><span data-stu-id="ed18a-143">Example: `../onenote/pages?sectionName=My%20section`.</span></span> <span data-ttu-id="ed18a-144">如果该节不存在 (或已重命名), API 将创建一个新分区。</span><span class="sxs-lookup"><span data-stu-id="ed18a-144">If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages
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
##### <a name="response"></a><span data-ttu-id="ed18a-145">响应</span><span class="sxs-lookup"><span data-stu-id="ed18a-145">Response</span></span>
<span data-ttu-id="ed18a-p108">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed18a-p108">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
