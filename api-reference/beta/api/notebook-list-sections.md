---
title: 列出分区
description: 从指定的笔记本中检索分区对象的列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 59a8580df694940c6f9acf8b0db6e6e29126589e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460753"
---
# <a name="list-sections"></a><span data-ttu-id="05d3f-103">列出分区</span><span class="sxs-lookup"><span data-stu-id="05d3f-103">List sections</span></span>

<span data-ttu-id="05d3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05d3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05d3f-105">从指定的笔记本中检索 [分区](../resources/onenotesection.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="05d3f-105">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="05d3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="05d3f-106">Permissions</span></span>
<span data-ttu-id="05d3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05d3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05d3f-109">Permission type</span></span>      | <span data-ttu-id="05d3f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05d3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05d3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05d3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05d3f-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05d3f-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="05d3f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05d3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05d3f-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05d3f-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="05d3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05d3f-115">Application</span></span> | <span data-ttu-id="05d3f-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05d3f-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05d3f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05d3f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05d3f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="05d3f-118">Optional query parameters</span></span>
<span data-ttu-id="05d3f-119">此方法支持 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="05d3f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="05d3f-120">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="05d3f-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="05d3f-121">默认查询将展开 `parentNotebook` 并选择其 `id` 、 `displayName` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="05d3f-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="05d3f-122">`expand`节的有效值为 `parentNotebook` 和 `parentSectionGroup` 。</span><span class="sxs-lookup"><span data-stu-id="05d3f-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="05d3f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="05d3f-123">Request headers</span></span>
| <span data-ttu-id="05d3f-124">名称</span><span class="sxs-lookup"><span data-stu-id="05d3f-124">Name</span></span>       | <span data-ttu-id="05d3f-125">类型</span><span class="sxs-lookup"><span data-stu-id="05d3f-125">Type</span></span> | <span data-ttu-id="05d3f-126">说明</span><span class="sxs-lookup"><span data-stu-id="05d3f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="05d3f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="05d3f-127">Authorization</span></span>  | <span data-ttu-id="05d3f-128">string</span><span class="sxs-lookup"><span data-stu-id="05d3f-128">string</span></span>  | <span data-ttu-id="05d3f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05d3f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05d3f-131">接受</span><span class="sxs-lookup"><span data-stu-id="05d3f-131">Accept</span></span> | <span data-ttu-id="05d3f-132">string</span><span class="sxs-lookup"><span data-stu-id="05d3f-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="05d3f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="05d3f-133">Request body</span></span>
<span data-ttu-id="05d3f-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05d3f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05d3f-135">响应</span><span class="sxs-lookup"><span data-stu-id="05d3f-135">Response</span></span>

<span data-ttu-id="05d3f-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [onenoteSection](../resources/onenotesection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="05d3f-136">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05d3f-137">示例</span><span class="sxs-lookup"><span data-stu-id="05d3f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05d3f-138">请求</span><span class="sxs-lookup"><span data-stu-id="05d3f-138">Request</span></span>
<span data-ttu-id="05d3f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05d3f-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05d3f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="05d3f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
# <a name="c"></a>[<span data-ttu-id="05d3f-141">C#</span><span class="sxs-lookup"><span data-stu-id="05d3f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05d3f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05d3f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05d3f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05d3f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="05d3f-144">响应</span><span class="sxs-lookup"><span data-stu-id="05d3f-144">Response</span></span>
<span data-ttu-id="05d3f-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05d3f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "isDefault": true,
      "pagesUrl": "pagesUrl-value",
      "displayName": "name-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "createdBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "lastModifiedBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
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
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
