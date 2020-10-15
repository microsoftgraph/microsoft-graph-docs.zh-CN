---
title: 获取分区
description: 检索 onenoteSection 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 87ff9efd1aceaa9f238e2cb861dd93d00fcf1bb6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458918"
---
# <a name="get-section"></a><span data-ttu-id="217a0-103">获取分区</span><span class="sxs-lookup"><span data-stu-id="217a0-103">Get section</span></span>

<span data-ttu-id="217a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="217a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="217a0-105">检索 [onenoteSection](../resources/section.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="217a0-105">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="217a0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="217a0-106">Permissions</span></span>
<span data-ttu-id="217a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="217a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="217a0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="217a0-109">Permission type</span></span>      | <span data-ttu-id="217a0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="217a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="217a0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="217a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="217a0-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="217a0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="217a0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="217a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="217a0-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="217a0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="217a0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="217a0-115">Application</span></span> | <span data-ttu-id="217a0-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="217a0-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="217a0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="217a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="217a0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="217a0-118">Optional query parameters</span></span>
<span data-ttu-id="217a0-119">此方法支持 `select` 和 `expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="217a0-119">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="217a0-120">默认查询将展开 `parentNotebook` 并选择其 `id` 、 `displayName` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="217a0-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="217a0-121">`expand`节的有效值为 `parentNotebook` 和 `parentSectionGroup` 。</span><span class="sxs-lookup"><span data-stu-id="217a0-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="217a0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="217a0-122">Request headers</span></span>
| <span data-ttu-id="217a0-123">名称</span><span class="sxs-lookup"><span data-stu-id="217a0-123">Name</span></span>       | <span data-ttu-id="217a0-124">类型</span><span class="sxs-lookup"><span data-stu-id="217a0-124">Type</span></span> | <span data-ttu-id="217a0-125">说明</span><span class="sxs-lookup"><span data-stu-id="217a0-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="217a0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="217a0-126">Authorization</span></span>  | <span data-ttu-id="217a0-127">string</span><span class="sxs-lookup"><span data-stu-id="217a0-127">string</span></span>  | <span data-ttu-id="217a0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="217a0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="217a0-130">接受</span><span class="sxs-lookup"><span data-stu-id="217a0-130">Accept</span></span> | <span data-ttu-id="217a0-131">string</span><span class="sxs-lookup"><span data-stu-id="217a0-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="217a0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="217a0-132">Request body</span></span>
<span data-ttu-id="217a0-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="217a0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="217a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="217a0-134">Response</span></span>

<span data-ttu-id="217a0-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [onenoteSection](../resources/section.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="217a0-135">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="217a0-136">示例</span><span class="sxs-lookup"><span data-stu-id="217a0-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="217a0-137">请求</span><span class="sxs-lookup"><span data-stu-id="217a0-137">Request</span></span>
<span data-ttu-id="217a0-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="217a0-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="217a0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="217a0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
# <a name="c"></a>[<span data-ttu-id="217a0-140">C#</span><span class="sxs-lookup"><span data-stu-id="217a0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="217a0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="217a0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="217a0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="217a0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="217a0-143">Java</span><span class="sxs-lookup"><span data-stu-id="217a0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-section-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="217a0-144">响应</span><span class="sxs-lookup"><span data-stu-id="217a0-144">Response</span></span>
<span data-ttu-id="217a0-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="217a0-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
