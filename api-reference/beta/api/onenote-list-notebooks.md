---
title: 列出笔记本
description: 检索 notebook 对象列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a1a0b9df816f8781efb2c3e45719fa204397736a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414649"
---
# <a name="list-notebooks"></a><span data-ttu-id="cfce1-103">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="cfce1-103">List notebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfce1-104">检索 [notebook](../resources/notebook.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="cfce1-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfce1-105">权限</span><span class="sxs-lookup"><span data-stu-id="cfce1-105">Permissions</span></span>
<span data-ttu-id="cfce1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfce1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfce1-108">Permission type</span></span>      | <span data-ttu-id="cfce1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfce1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfce1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfce1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfce1-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfce1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfce1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfce1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfce1-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfce1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="cfce1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfce1-114">Application</span></span> | <span data-ttu-id="cfce1-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfce1-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfce1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfce1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cfce1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cfce1-117">Optional query parameters</span></span>
<span data-ttu-id="cfce1-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cfce1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cfce1-119">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="cfce1-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="cfce1-120">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="cfce1-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfce1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfce1-121">Request headers</span></span>
| <span data-ttu-id="cfce1-122">名称</span><span class="sxs-lookup"><span data-stu-id="cfce1-122">Name</span></span>       | <span data-ttu-id="cfce1-123">类型</span><span class="sxs-lookup"><span data-stu-id="cfce1-123">Type</span></span> | <span data-ttu-id="cfce1-124">说明</span><span class="sxs-lookup"><span data-stu-id="cfce1-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cfce1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfce1-125">Authorization</span></span>  | <span data-ttu-id="cfce1-126">string</span><span class="sxs-lookup"><span data-stu-id="cfce1-126">string</span></span>  | <span data-ttu-id="cfce1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfce1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfce1-129">接受</span><span class="sxs-lookup"><span data-stu-id="cfce1-129">Accept</span></span> | <span data-ttu-id="cfce1-130">string</span><span class="sxs-lookup"><span data-stu-id="cfce1-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cfce1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfce1-131">Request body</span></span>
<span data-ttu-id="cfce1-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfce1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfce1-133">响应</span><span class="sxs-lookup"><span data-stu-id="cfce1-133">Response</span></span>

<span data-ttu-id="cfce1-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cfce1-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cfce1-135">示例</span><span class="sxs-lookup"><span data-stu-id="cfce1-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfce1-136">请求</span><span class="sxs-lookup"><span data-stu-id="cfce1-136">Request</span></span>
<span data-ttu-id="cfce1-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfce1-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cfce1-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cfce1-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfce1-139">C#</span><span class="sxs-lookup"><span data-stu-id="cfce1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfce1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfce1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfce1-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="cfce1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cfce1-142">响应</span><span class="sxs-lookup"><span data-stu-id="cfce1-142">Response</span></span>
<span data-ttu-id="cfce1-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cfce1-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
