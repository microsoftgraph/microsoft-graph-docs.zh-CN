---
title: 获取分区
description: 检索 section 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2c8724c672efa9d7eafa152fdcddfd5681e286a6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979548"
---
# <a name="get-section"></a><span data-ttu-id="7f8b1-103">获取分区</span><span class="sxs-lookup"><span data-stu-id="7f8b1-103">Get section</span></span>

<span data-ttu-id="7f8b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f8b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f8b1-105">检索 [section](../resources/onenotesection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-105">Retrieve the properties and relationships of a [section](../resources/onenotesection.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f8b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f8b1-106">Permissions</span></span>
<span data-ttu-id="7f8b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f8b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f8b1-109">Permission type</span></span>      | <span data-ttu-id="7f8b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f8b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f8b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f8b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f8b1-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f8b1-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f8b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f8b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f8b1-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f8b1-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7f8b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f8b1-115">Application</span></span> | <span data-ttu-id="7f8b1-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f8b1-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f8b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f8b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f8b1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f8b1-118">Optional query parameters</span></span>
<span data-ttu-id="7f8b1-119">此方法支持 `select` 和 `expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-119">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="7f8b1-120">默认查询将展开 `parentNotebook` 并选择其 `id` 、 `displayName` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="7f8b1-121">`expand`节的有效值为 `parentNotebook` 和 `parentSectionGroup` 。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f8b1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f8b1-122">Request headers</span></span>
| <span data-ttu-id="7f8b1-123">名称</span><span class="sxs-lookup"><span data-stu-id="7f8b1-123">Name</span></span>       | <span data-ttu-id="7f8b1-124">类型</span><span class="sxs-lookup"><span data-stu-id="7f8b1-124">Type</span></span> | <span data-ttu-id="7f8b1-125">说明</span><span class="sxs-lookup"><span data-stu-id="7f8b1-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f8b1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f8b1-126">Authorization</span></span>  | <span data-ttu-id="7f8b1-127">string</span><span class="sxs-lookup"><span data-stu-id="7f8b1-127">string</span></span>  | <span data-ttu-id="7f8b1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f8b1-130">接受</span><span class="sxs-lookup"><span data-stu-id="7f8b1-130">Accept</span></span> | <span data-ttu-id="7f8b1-131">string</span><span class="sxs-lookup"><span data-stu-id="7f8b1-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7f8b1-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f8b1-132">Request body</span></span>
<span data-ttu-id="7f8b1-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f8b1-134">响应</span><span class="sxs-lookup"><span data-stu-id="7f8b1-134">Response</span></span>

<span data-ttu-id="7f8b1-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [onenoteSection](../resources/onenotesection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-135">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f8b1-136">示例</span><span class="sxs-lookup"><span data-stu-id="7f8b1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f8b1-137">请求</span><span class="sxs-lookup"><span data-stu-id="7f8b1-137">Request</span></span>
<span data-ttu-id="7f8b1-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f8b1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f8b1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
# <a name="c"></a>[<span data-ttu-id="7f8b1-140">C#</span><span class="sxs-lookup"><span data-stu-id="7f8b1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f8b1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f8b1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f8b1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f8b1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f8b1-143">Java</span><span class="sxs-lookup"><span data-stu-id="7f8b1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-section-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f8b1-144">响应</span><span class="sxs-lookup"><span data-stu-id="7f8b1-144">Response</span></span>
<span data-ttu-id="7f8b1-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f8b1-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
