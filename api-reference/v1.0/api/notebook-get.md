---
title: 获取笔记本
description: 检索笔记本对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 360478d78ffe3cb1833fa3de29eeac1e65dabc1c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274562"
---
# <a name="get-notebook"></a><span data-ttu-id="cea63-103">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="cea63-103">Get notebook</span></span>

<span data-ttu-id="cea63-104">检索[笔记本](../resources/notebook.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cea63-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cea63-105">权限</span><span class="sxs-lookup"><span data-stu-id="cea63-105">Permissions</span></span>
<span data-ttu-id="cea63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cea63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cea63-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cea63-108">Permission type</span></span>      | <span data-ttu-id="cea63-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cea63-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cea63-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cea63-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cea63-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cea63-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cea63-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cea63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cea63-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cea63-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="cea63-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cea63-114">Application</span></span> | <span data-ttu-id="cea63-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cea63-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cea63-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cea63-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cea63-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cea63-117">Optional query parameters</span></span>
<span data-ttu-id="cea63-118">此方法支持`select`和`expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cea63-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cea63-119">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="cea63-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cea63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cea63-120">Request headers</span></span>
| <span data-ttu-id="cea63-121">名称</span><span class="sxs-lookup"><span data-stu-id="cea63-121">Name</span></span>       | <span data-ttu-id="cea63-122">类型</span><span class="sxs-lookup"><span data-stu-id="cea63-122">Type</span></span> | <span data-ttu-id="cea63-123">说明</span><span class="sxs-lookup"><span data-stu-id="cea63-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cea63-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cea63-124">Authorization</span></span>  | <span data-ttu-id="cea63-125">string</span><span class="sxs-lookup"><span data-stu-id="cea63-125">string</span></span>  | <span data-ttu-id="cea63-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cea63-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cea63-128">接受</span><span class="sxs-lookup"><span data-stu-id="cea63-128">Accept</span></span> | <span data-ttu-id="cea63-129">string</span><span class="sxs-lookup"><span data-stu-id="cea63-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cea63-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cea63-130">Request body</span></span>
<span data-ttu-id="cea63-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cea63-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cea63-132">响应</span><span class="sxs-lookup"><span data-stu-id="cea63-132">Response</span></span>

<span data-ttu-id="cea63-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[笔记本](../resources/notebook.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cea63-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cea63-134">示例</span><span class="sxs-lookup"><span data-stu-id="cea63-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cea63-135">请求</span><span class="sxs-lookup"><span data-stu-id="cea63-135">Request</span></span>
<span data-ttu-id="cea63-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cea63-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="cea63-137">响应</span><span class="sxs-lookup"><span data-stu-id="cea63-137">Response</span></span>
<span data-ttu-id="cea63-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cea63-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cea63-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cea63-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cea63-142">C#</span><span class="sxs-lookup"><span data-stu-id="cea63-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_notebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cea63-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="cea63-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_notebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cea63-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="cea63-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_notebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
