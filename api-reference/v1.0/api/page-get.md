---
title: 获取页面
description: 检索 page 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 98c15b4638ce41debc9e8dd040d77d610ad1665b
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402000"
---
# <a name="get-page"></a><span data-ttu-id="ab1d3-103">获取页面</span><span class="sxs-lookup"><span data-stu-id="ab1d3-103">Get page</span></span>

<span data-ttu-id="ab1d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab1d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab1d3-105">检索 [page](../resources/page.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-105">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="ab1d3-106">**获取页面信息**</span><span class="sxs-lookup"><span data-stu-id="ab1d3-106">**Getting page information**</span></span>

<span data-ttu-id="ab1d3-107">按页面标识符访问页面的元数据：</span><span class="sxs-lookup"><span data-stu-id="ab1d3-107">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="ab1d3-108">**获取页面内容**</span><span class="sxs-lookup"><span data-stu-id="ab1d3-108">**Getting page content**</span></span>

<span data-ttu-id="ab1d3-109">您可以使用页面的 `content` 终结点获取页面的 HTML 内容：</span><span class="sxs-lookup"><span data-stu-id="ab1d3-109">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="ab1d3-110">`includeIDs=true`查询选项用于[更新页面](../api/page-update.md)。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-110">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab1d3-111">权限</span><span class="sxs-lookup"><span data-stu-id="ab1d3-111">Permissions</span></span>
<span data-ttu-id="ab1d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab1d3-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab1d3-114">Permission type</span></span>      | <span data-ttu-id="ab1d3-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab1d3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab1d3-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab1d3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ab1d3-117">请参阅 "注意，"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="ab1d3-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab1d3-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab1d3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab1d3-119">注意： Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="ab1d3-119">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ab1d3-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab1d3-120">Application</span></span> | <span data-ttu-id="ab1d3-121">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab1d3-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab1d3-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab1d3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab1d3-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab1d3-123">Optional query parameters</span></span>
<span data-ttu-id="ab1d3-124">此方法支持 `select` 和 `expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-124">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="ab1d3-125">默认响应将展开 `parentSection` 并选择节的 `id` 、 `name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-125">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="ab1d3-126">`expand`页面的有效值为 `parentNotebook` 和 `parentSection` 。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-126">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab1d3-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab1d3-127">Request headers</span></span>
| <span data-ttu-id="ab1d3-128">名称</span><span class="sxs-lookup"><span data-stu-id="ab1d3-128">Name</span></span>       | <span data-ttu-id="ab1d3-129">类型</span><span class="sxs-lookup"><span data-stu-id="ab1d3-129">Type</span></span> | <span data-ttu-id="ab1d3-130">说明</span><span class="sxs-lookup"><span data-stu-id="ab1d3-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ab1d3-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab1d3-131">Authorization</span></span>  | <span data-ttu-id="ab1d3-132">string</span><span class="sxs-lookup"><span data-stu-id="ab1d3-132">string</span></span>  | <span data-ttu-id="ab1d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab1d3-135">接受</span><span class="sxs-lookup"><span data-stu-id="ab1d3-135">Accept</span></span> | <span data-ttu-id="ab1d3-136">string</span><span class="sxs-lookup"><span data-stu-id="ab1d3-136">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ab1d3-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab1d3-137">Request body</span></span>
<span data-ttu-id="ab1d3-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab1d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="ab1d3-139">Response</span></span>

<span data-ttu-id="ab1d3-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [page](../resources/page.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-140">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab1d3-141">示例</span><span class="sxs-lookup"><span data-stu-id="ab1d3-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab1d3-142">请求</span><span class="sxs-lookup"><span data-stu-id="ab1d3-142">Request</span></span>
<span data-ttu-id="ab1d3-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-143">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="ab1d3-144">响应</span><span class="sxs-lookup"><span data-stu-id="ab1d3-144">Response</span></span>
<span data-ttu-id="ab1d3-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-145">Here is an example of the response.</span></span> <span data-ttu-id="ab1d3-146">注意：为简洁起见，此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-146">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="ab1d3-147">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab1d3-147">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->