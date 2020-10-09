---
title: 列出分区
description: 检索 onenoteSection 对象的列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 4b096b11b34b1cfd68b7e9d3d7c584a40ebf01b5
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405972"
---
# <a name="list-sections"></a><span data-ttu-id="bbcea-103">列出分区</span><span class="sxs-lookup"><span data-stu-id="bbcea-103">List sections</span></span>

<span data-ttu-id="bbcea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbcea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbcea-105">检索 [onenoteSection](../resources/section.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bbcea-105">Retrieve a list of [onenoteSection](../resources/section.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bbcea-106">权限</span><span class="sxs-lookup"><span data-stu-id="bbcea-106">Permissions</span></span>
<span data-ttu-id="bbcea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbcea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbcea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbcea-109">Permission type</span></span>      | <span data-ttu-id="bbcea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbcea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbcea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbcea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbcea-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbcea-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbcea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbcea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbcea-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbcea-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bbcea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbcea-115">Application</span></span> | <span data-ttu-id="bbcea-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbcea-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbcea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbcea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbcea-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bbcea-118">Optional query parameters</span></span>
<span data-ttu-id="bbcea-119">此方法支持 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bbcea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="bbcea-120">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="bbcea-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="bbcea-121">默认查询将展开 `parentNotebook` 并选择其 `id` 、 `displayName` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="bbcea-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="bbcea-122">`expand`节的有效值为 `parentNotebook` 和 `parentSectionGroup` 。</span><span class="sxs-lookup"><span data-stu-id="bbcea-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbcea-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbcea-123">Request headers</span></span>
| <span data-ttu-id="bbcea-124">名称</span><span class="sxs-lookup"><span data-stu-id="bbcea-124">Name</span></span>       | <span data-ttu-id="bbcea-125">类型</span><span class="sxs-lookup"><span data-stu-id="bbcea-125">Type</span></span> | <span data-ttu-id="bbcea-126">说明</span><span class="sxs-lookup"><span data-stu-id="bbcea-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bbcea-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbcea-127">Authorization</span></span>  | <span data-ttu-id="bbcea-128">string</span><span class="sxs-lookup"><span data-stu-id="bbcea-128">string</span></span>  | <span data-ttu-id="bbcea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbcea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbcea-131">接受</span><span class="sxs-lookup"><span data-stu-id="bbcea-131">Accept</span></span> | <span data-ttu-id="bbcea-132">string</span><span class="sxs-lookup"><span data-stu-id="bbcea-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bbcea-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbcea-133">Request body</span></span>
<span data-ttu-id="bbcea-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbcea-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbcea-135">响应</span><span class="sxs-lookup"><span data-stu-id="bbcea-135">Response</span></span>

<span data-ttu-id="bbcea-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [onenoteSection](../resources/section.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bbcea-136">If successful, this method returns a `200 OK` response code and collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bbcea-137">示例</span><span class="sxs-lookup"><span data-stu-id="bbcea-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbcea-138">请求</span><span class="sxs-lookup"><span data-stu-id="bbcea-138">Request</span></span>
<span data-ttu-id="bbcea-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbcea-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bbcea-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbcea-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "onenote_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sections
```
# <a name="c"></a>[<span data-ttu-id="bbcea-141">C#</span><span class="sxs-lookup"><span data-stu-id="bbcea-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/onenote-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbcea-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbcea-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/onenote-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbcea-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbcea-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/onenote-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbcea-144">Java</span><span class="sxs-lookup"><span data-stu-id="bbcea-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/onenote-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bbcea-145">响应</span><span class="sxs-lookup"><span data-stu-id="bbcea-145">Response</span></span>
<span data-ttu-id="bbcea-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbcea-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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