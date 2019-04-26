---
title: 创建页面
description: 在指定分区中新建页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7e0ecd6792758d6a48626f47b21c879dd110daba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331447"
---
# <a name="create-page"></a><span data-ttu-id="2b9ee-103">创建页面</span><span class="sxs-lookup"><span data-stu-id="2b9ee-103">Create page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b9ee-104">在指定分区中新建[页面](../resources/onenotepage.md)。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-104">Create a new [page](../resources/onenotepage.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b9ee-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b9ee-105">Permissions</span></span>
<span data-ttu-id="2b9ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b9ee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b9ee-108">Permission type</span></span>      | <span data-ttu-id="2b9ee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b9ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b9ee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b9ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b9ee-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b9ee-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b9ee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b9ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b9ee-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b9ee-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2b9ee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b9ee-114">Application</span></span> | <span data-ttu-id="2b9ee-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b9ee-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b9ee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b9ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="2b9ee-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b9ee-117">Request headers</span></span>
| <span data-ttu-id="2b9ee-118">名称</span><span class="sxs-lookup"><span data-stu-id="2b9ee-118">Name</span></span>       | <span data-ttu-id="2b9ee-119">类型</span><span class="sxs-lookup"><span data-stu-id="2b9ee-119">Type</span></span> | <span data-ttu-id="2b9ee-120">说明</span><span class="sxs-lookup"><span data-stu-id="2b9ee-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2b9ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b9ee-121">Authorization</span></span>  | <span data-ttu-id="2b9ee-122">string</span><span class="sxs-lookup"><span data-stu-id="2b9ee-122">string</span></span>  | <span data-ttu-id="2b9ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b9ee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b9ee-125">Content-Type</span></span> | <span data-ttu-id="2b9ee-126">string</span><span class="sxs-lookup"><span data-stu-id="2b9ee-126">string</span></span> | <span data-ttu-id="2b9ee-p103">HTML 内容（包括多部分请求必备的“演示”部分）的 `text/html` 或 `application/xhtml+xml`。多部分请求使用 `multipart/form-data; boundary=your-boundary` 内容类型。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b9ee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b9ee-129">Request body</span></span>
<span data-ttu-id="2b9ee-130">在请求正文中，提供页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-130">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="2b9ee-p104">正文可以将 HTML 直接置于请求正文中，或者其可以包含多部分消息格式，如示例中所示。如果要发送二进制数据，则必须发送多部分请求。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="2b9ee-133">响应</span><span class="sxs-lookup"><span data-stu-id="2b9ee-133">Response</span></span>

<span data-ttu-id="2b9ee-134">如果成功, 此方法在`201 Created`响应正文中返回响应代码和新的[onenotePage](../resources/onenotepage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-134">If successful, this method returns `201 Created` response code and the new [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b9ee-135">示例</span><span class="sxs-lookup"><span data-stu-id="2b9ee-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b9ee-136">请求</span><span class="sxs-lookup"><span data-stu-id="2b9ee-136">Request</span></span>
<span data-ttu-id="2b9ee-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-137">Here is an example of the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="2b9ee-138">响应</span><span class="sxs-lookup"><span data-stu-id="2b9ee-138">Response</span></span>
<span data-ttu-id="2b9ee-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b9ee-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
