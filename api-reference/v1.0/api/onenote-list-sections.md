---
title: 列出分区
description: 检索 onenoteSection 对象的列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d0b24af0d0ec34d60bf30d1a8d7348236222f4bb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35435974"
---
# <a name="list-sections"></a><span data-ttu-id="06ebf-103">列出分区</span><span class="sxs-lookup"><span data-stu-id="06ebf-103">List sections</span></span>

<span data-ttu-id="06ebf-104">检索[onenoteSection](../resources/section.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="06ebf-104">Retrieve a list of [onenoteSection](../resources/section.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="06ebf-105">权限</span><span class="sxs-lookup"><span data-stu-id="06ebf-105">Permissions</span></span>
<span data-ttu-id="06ebf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06ebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ebf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="06ebf-108">Permission type</span></span>      | <span data-ttu-id="06ebf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06ebf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06ebf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06ebf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06ebf-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ebf-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="06ebf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06ebf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06ebf-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06ebf-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="06ebf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="06ebf-114">Application</span></span> | <span data-ttu-id="06ebf-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ebf-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06ebf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06ebf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06ebf-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="06ebf-117">Optional query parameters</span></span>
<span data-ttu-id="06ebf-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06ebf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="06ebf-119">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="06ebf-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="06ebf-120">默认查询将展开`parentNotebook`并选择其`id`、 `displayName`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="06ebf-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="06ebf-121">节`expand`的`parentNotebook`有效值为和`parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="06ebf-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06ebf-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="06ebf-122">Request headers</span></span>
| <span data-ttu-id="06ebf-123">名称</span><span class="sxs-lookup"><span data-stu-id="06ebf-123">Name</span></span>       | <span data-ttu-id="06ebf-124">类型</span><span class="sxs-lookup"><span data-stu-id="06ebf-124">Type</span></span> | <span data-ttu-id="06ebf-125">说明</span><span class="sxs-lookup"><span data-stu-id="06ebf-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06ebf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="06ebf-126">Authorization</span></span>  | <span data-ttu-id="06ebf-127">string</span><span class="sxs-lookup"><span data-stu-id="06ebf-127">string</span></span>  | <span data-ttu-id="06ebf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06ebf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06ebf-130">接受</span><span class="sxs-lookup"><span data-stu-id="06ebf-130">Accept</span></span> | <span data-ttu-id="06ebf-131">string</span><span class="sxs-lookup"><span data-stu-id="06ebf-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="06ebf-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="06ebf-132">Request body</span></span>
<span data-ttu-id="06ebf-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06ebf-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06ebf-134">响应</span><span class="sxs-lookup"><span data-stu-id="06ebf-134">Response</span></span>

<span data-ttu-id="06ebf-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenoteSection](../resources/section.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="06ebf-135">If successful, this method returns a `200 OK` response code and collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06ebf-136">示例</span><span class="sxs-lookup"><span data-stu-id="06ebf-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06ebf-137">请求</span><span class="sxs-lookup"><span data-stu-id="06ebf-137">Request</span></span>
<span data-ttu-id="06ebf-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06ebf-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06ebf-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="06ebf-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06ebf-140">C#</span><span class="sxs-lookup"><span data-stu-id="06ebf-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06ebf-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="06ebf-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06ebf-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="06ebf-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06ebf-143">响应</span><span class="sxs-lookup"><span data-stu-id="06ebf-143">Response</span></span>
<span data-ttu-id="06ebf-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06ebf-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
