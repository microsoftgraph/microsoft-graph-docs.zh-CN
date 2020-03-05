---
title: 获取页面
description: 检索 page 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 13a4953c2ffa94ef85a836a3796f88a6cee149c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456006"
---
# <a name="get-page"></a><span data-ttu-id="f628e-103">获取页面</span><span class="sxs-lookup"><span data-stu-id="f628e-103">Get page</span></span>

<span data-ttu-id="f628e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f628e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f628e-105">检索[page](../resources/onenotepage.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f628e-105">Retrieve the properties and relationships of a [page](../resources/onenotepage.md) object.</span></span>

<span data-ttu-id="f628e-106">**获取页面信息**</span><span class="sxs-lookup"><span data-stu-id="f628e-106">**Getting page information**</span></span>

<span data-ttu-id="f628e-107">按页面标识符访问页面的元数据：</span><span class="sxs-lookup"><span data-stu-id="f628e-107">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="f628e-108">**获取页面内容**</span><span class="sxs-lookup"><span data-stu-id="f628e-108">**Getting page content**</span></span>

<span data-ttu-id="f628e-109">您可以使用页面的`content`终结点获取页面的 HTML 内容：</span><span class="sxs-lookup"><span data-stu-id="f628e-109">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="f628e-110">`includeIDs=true`查询选项用于[更新页面](../api/page-update.md)。</span><span class="sxs-lookup"><span data-stu-id="f628e-110">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f628e-111">权限</span><span class="sxs-lookup"><span data-stu-id="f628e-111">Permissions</span></span>
<span data-ttu-id="f628e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f628e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f628e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f628e-114">Permission type</span></span>      | <span data-ttu-id="f628e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f628e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f628e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f628e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f628e-117">请参阅 "注意，"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="f628e-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f628e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f628e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f628e-119">注意： Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="f628e-119">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f628e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f628e-120">Application</span></span> | <span data-ttu-id="f628e-121">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f628e-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f628e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f628e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f628e-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f628e-123">Optional query parameters</span></span>
<span data-ttu-id="f628e-124">此方法支持`select`和`expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f628e-124">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f628e-125">默认响应将展开`parentSection`并选择节的`id`、 `name`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="f628e-125">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="f628e-126">页面`expand`的`parentNotebook`有效值为和`parentSection`。</span><span class="sxs-lookup"><span data-stu-id="f628e-126">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f628e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="f628e-127">Request headers</span></span>
| <span data-ttu-id="f628e-128">名称</span><span class="sxs-lookup"><span data-stu-id="f628e-128">Name</span></span>       | <span data-ttu-id="f628e-129">类型</span><span class="sxs-lookup"><span data-stu-id="f628e-129">Type</span></span> | <span data-ttu-id="f628e-130">说明</span><span class="sxs-lookup"><span data-stu-id="f628e-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f628e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f628e-131">Authorization</span></span>  | <span data-ttu-id="f628e-132">string</span><span class="sxs-lookup"><span data-stu-id="f628e-132">string</span></span>  | <span data-ttu-id="f628e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f628e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f628e-135">接受</span><span class="sxs-lookup"><span data-stu-id="f628e-135">Accept</span></span> | <span data-ttu-id="f628e-136">string</span><span class="sxs-lookup"><span data-stu-id="f628e-136">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f628e-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="f628e-137">Request body</span></span>
<span data-ttu-id="f628e-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f628e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f628e-139">响应</span><span class="sxs-lookup"><span data-stu-id="f628e-139">Response</span></span>

<span data-ttu-id="f628e-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和[onenotePage](../resources/onenotepage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f628e-140">If successful, this method returns a `200 OK` response code and the [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f628e-141">示例</span><span class="sxs-lookup"><span data-stu-id="f628e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f628e-142">请求</span><span class="sxs-lookup"><span data-stu-id="f628e-142">Request</span></span>
<span data-ttu-id="f628e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f628e-143">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="f628e-144">响应</span><span class="sxs-lookup"><span data-stu-id="f628e-144">Response</span></span>
<span data-ttu-id="f628e-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f628e-145">Here is an example of the response.</span></span> <span data-ttu-id="f628e-146">注意：为简洁起见，此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="f628e-146">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="f628e-147">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f628e-147">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
