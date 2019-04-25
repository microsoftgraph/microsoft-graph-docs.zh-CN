---
title: 获取页面
description: 检索 page 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 57a2c75bbe671086c89818a84f7f8266b90713c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539388"
---
# <a name="get-page"></a><span data-ttu-id="5473d-103">获取页面</span><span class="sxs-lookup"><span data-stu-id="5473d-103">Get page</span></span>

<span data-ttu-id="5473d-104">检索[page](../resources/page.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5473d-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="5473d-105">**获取页面信息**</span><span class="sxs-lookup"><span data-stu-id="5473d-105">**Getting page information**</span></span>

<span data-ttu-id="5473d-106">按页面标识符访问页面的元数据:</span><span class="sxs-lookup"><span data-stu-id="5473d-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="5473d-107">**获取页面内容**</span><span class="sxs-lookup"><span data-stu-id="5473d-107">**Getting page content**</span></span>

<span data-ttu-id="5473d-108">您可以使用页面的`content`终结点获取页面的 HTML 内容:</span><span class="sxs-lookup"><span data-stu-id="5473d-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="5473d-109">`includeIDs=true`查询选项用于[更新页面](../api/page-update.md)。</span><span class="sxs-lookup"><span data-stu-id="5473d-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5473d-110">权限</span><span class="sxs-lookup"><span data-stu-id="5473d-110">Permissions</span></span>
<span data-ttu-id="5473d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5473d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5473d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5473d-113">Permission type</span></span>      | <span data-ttu-id="5473d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5473d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5473d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5473d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5473d-116">请参阅 "注意,"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="5473d-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5473d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5473d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5473d-118">注意: Read、notes。读写</span><span class="sxs-lookup"><span data-stu-id="5473d-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5473d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5473d-119">Application</span></span> | <span data-ttu-id="5473d-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5473d-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5473d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5473d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5473d-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5473d-122">Optional query parameters</span></span>
<span data-ttu-id="5473d-123">此方法支持`select`和`expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5473d-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5473d-124">默认响应将展开`parentSection`并选择节的`id`、 `name`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="5473d-124">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="5473d-125">页面`expand`的`parentNotebook`有效值为和`parentSection`。</span><span class="sxs-lookup"><span data-stu-id="5473d-125">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5473d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="5473d-126">Request headers</span></span>
| <span data-ttu-id="5473d-127">名称</span><span class="sxs-lookup"><span data-stu-id="5473d-127">Name</span></span>       | <span data-ttu-id="5473d-128">类型</span><span class="sxs-lookup"><span data-stu-id="5473d-128">Type</span></span> | <span data-ttu-id="5473d-129">说明</span><span class="sxs-lookup"><span data-stu-id="5473d-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5473d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5473d-130">Authorization</span></span>  | <span data-ttu-id="5473d-131">string</span><span class="sxs-lookup"><span data-stu-id="5473d-131">string</span></span>  | <span data-ttu-id="5473d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5473d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5473d-134">接受</span><span class="sxs-lookup"><span data-stu-id="5473d-134">Accept</span></span> | <span data-ttu-id="5473d-135">string</span><span class="sxs-lookup"><span data-stu-id="5473d-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5473d-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5473d-136">Request body</span></span>
<span data-ttu-id="5473d-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5473d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5473d-138">响应</span><span class="sxs-lookup"><span data-stu-id="5473d-138">Response</span></span>

<span data-ttu-id="5473d-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[page](../resources/page.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5473d-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5473d-140">示例</span><span class="sxs-lookup"><span data-stu-id="5473d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5473d-141">请求</span><span class="sxs-lookup"><span data-stu-id="5473d-141">Request</span></span>
<span data-ttu-id="5473d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5473d-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="5473d-143">响应</span><span class="sxs-lookup"><span data-stu-id="5473d-143">Response</span></span>
<span data-ttu-id="5473d-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5473d-144">Here is an example of the response.</span></span> <span data-ttu-id="5473d-145">注意: 为简洁起见, 此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="5473d-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="5473d-146">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5473d-146">All of the properties will be returned from an actual call.</span></span>
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
