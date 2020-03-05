---
title: 创建页面
description: 在指定分区中新建页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 73c58b9855d73d7b7809f4d8e0503f28fbe110e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453651"
---
# <a name="create-page"></a><span data-ttu-id="80273-103">创建页面</span><span class="sxs-lookup"><span data-stu-id="80273-103">Create page</span></span>

<span data-ttu-id="80273-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="80273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80273-105">在指定分区中新建[页面](../resources/onenotepage.md)。</span><span class="sxs-lookup"><span data-stu-id="80273-105">Create a new [page](../resources/onenotepage.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="80273-106">权限</span><span class="sxs-lookup"><span data-stu-id="80273-106">Permissions</span></span>
<span data-ttu-id="80273-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80273-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80273-109">Permission type</span></span>      | <span data-ttu-id="80273-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80273-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80273-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80273-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80273-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80273-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="80273-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80273-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80273-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80273-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="80273-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80273-115">Application</span></span> | <span data-ttu-id="80273-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80273-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80273-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80273-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="80273-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80273-118">Request headers</span></span>
| <span data-ttu-id="80273-119">名称</span><span class="sxs-lookup"><span data-stu-id="80273-119">Name</span></span>       | <span data-ttu-id="80273-120">类型</span><span class="sxs-lookup"><span data-stu-id="80273-120">Type</span></span> | <span data-ttu-id="80273-121">说明</span><span class="sxs-lookup"><span data-stu-id="80273-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80273-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80273-122">Authorization</span></span>  | <span data-ttu-id="80273-123">string</span><span class="sxs-lookup"><span data-stu-id="80273-123">string</span></span>  | <span data-ttu-id="80273-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80273-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80273-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80273-126">Content-Type</span></span> | <span data-ttu-id="80273-127">string</span><span class="sxs-lookup"><span data-stu-id="80273-127">string</span></span> | <span data-ttu-id="80273-p103">HTML 内容（包括多部分请求必备的“演示”部分）的 `text/html` 或 `application/xhtml+xml`。多部分请求使用 `multipart/form-data; boundary=your-boundary` 内容类型。</span><span class="sxs-lookup"><span data-stu-id="80273-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80273-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="80273-130">Request body</span></span>
<span data-ttu-id="80273-131">在请求正文中，提供页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="80273-131">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="80273-p104">正文可以将 HTML 直接置于请求正文中，或者其可以包含多部分消息格式，如示例中所示。如果要发送二进制数据，则必须发送多部分请求。</span><span class="sxs-lookup"><span data-stu-id="80273-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="80273-134">响应</span><span class="sxs-lookup"><span data-stu-id="80273-134">Response</span></span>

<span data-ttu-id="80273-135">如果成功，此方法在`201 Created`响应正文中返回响应代码和新的[onenotePage](../resources/onenotepage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80273-135">If successful, this method returns `201 Created` response code and the new [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80273-136">示例</span><span class="sxs-lookup"><span data-stu-id="80273-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80273-137">请求</span><span class="sxs-lookup"><span data-stu-id="80273-137">Request</span></span>
<span data-ttu-id="80273-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80273-138">Here is an example of the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="80273-139">响应</span><span class="sxs-lookup"><span data-stu-id="80273-139">Response</span></span>
<span data-ttu-id="80273-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80273-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
