---
title: 列出笔记本
description: 检索 notebook 对象列表。
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 184ee93567cc55b52e8f3ae0c4ea473ec0e7c3d5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274506"
---
# <a name="list-notebooks"></a><span data-ttu-id="8f81b-103">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="8f81b-103">List notebooks</span></span>

<span data-ttu-id="8f81b-104">检索 [notebook](../resources/notebook.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8f81b-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f81b-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f81b-105">Permissions</span></span>
<span data-ttu-id="8f81b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f81b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f81b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f81b-108">Permission type</span></span>      | <span data-ttu-id="8f81b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f81b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f81b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f81b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f81b-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f81b-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f81b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f81b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f81b-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f81b-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8f81b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f81b-114">Application</span></span> | <span data-ttu-id="8f81b-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f81b-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f81b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f81b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8f81b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8f81b-117">Optional query parameters</span></span>
<span data-ttu-id="8f81b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8f81b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8f81b-119">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="8f81b-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="8f81b-120">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="8f81b-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f81b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f81b-121">Request headers</span></span>
| <span data-ttu-id="8f81b-122">名称</span><span class="sxs-lookup"><span data-stu-id="8f81b-122">Name</span></span>       | <span data-ttu-id="8f81b-123">类型</span><span class="sxs-lookup"><span data-stu-id="8f81b-123">Type</span></span> | <span data-ttu-id="8f81b-124">说明</span><span class="sxs-lookup"><span data-stu-id="8f81b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f81b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f81b-125">Authorization</span></span>  | <span data-ttu-id="8f81b-126">string</span><span class="sxs-lookup"><span data-stu-id="8f81b-126">string</span></span>  | <span data-ttu-id="8f81b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f81b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f81b-129">接受</span><span class="sxs-lookup"><span data-stu-id="8f81b-129">Accept</span></span> | <span data-ttu-id="8f81b-130">string</span><span class="sxs-lookup"><span data-stu-id="8f81b-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8f81b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f81b-131">Request body</span></span>
<span data-ttu-id="8f81b-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f81b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f81b-133">响应</span><span class="sxs-lookup"><span data-stu-id="8f81b-133">Response</span></span>

<span data-ttu-id="8f81b-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8f81b-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f81b-135">示例</span><span class="sxs-lookup"><span data-stu-id="8f81b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f81b-136">请求</span><span class="sxs-lookup"><span data-stu-id="8f81b-136">Request</span></span>
<span data-ttu-id="8f81b-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f81b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="8f81b-138">响应</span><span class="sxs-lookup"><span data-stu-id="8f81b-138">Response</span></span>
<span data-ttu-id="8f81b-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f81b-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
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
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f81b-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8f81b-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f81b-143">C#</span><span class="sxs-lookup"><span data-stu-id="8f81b-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_notebooks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f81b-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f81b-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_notebooks-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8f81b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f81b-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_notebooks-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/onenote-list-notebooks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/onenote-list-notebooks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/onenote-list-notebooks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
