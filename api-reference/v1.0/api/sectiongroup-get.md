---
title: 获取 sectionGroup
description: 检索 sectionGroup 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 04abdc0f9a3d38681ef2d47c1fe6b7794d153f1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509897"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="57ec8-103">获取 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="57ec8-103">Get sectionGroup</span></span>

<span data-ttu-id="57ec8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ec8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57ec8-105">检索[sectionGroup](../resources/sectiongroup.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57ec8-105">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="57ec8-106">权限</span><span class="sxs-lookup"><span data-stu-id="57ec8-106">Permissions</span></span>
<span data-ttu-id="57ec8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57ec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ec8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="57ec8-109">Permission type</span></span>      | <span data-ttu-id="57ec8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57ec8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57ec8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57ec8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57ec8-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ec8-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="57ec8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57ec8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57ec8-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57ec8-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="57ec8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="57ec8-115">Application</span></span> | <span data-ttu-id="57ec8-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ec8-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57ec8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57ec8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57ec8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="57ec8-118">Optional query parameters</span></span>
<span data-ttu-id="57ec8-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="57ec8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="57ec8-120">默认查询将展开`parentNotebook`并选择其`id`、 `name`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="57ec8-120">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="57ec8-121">节`expand`组的有效值为`parentNotebook`和`parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="57ec8-121">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57ec8-122">请求头</span><span class="sxs-lookup"><span data-stu-id="57ec8-122">Request headers</span></span>
| <span data-ttu-id="57ec8-123">名称</span><span class="sxs-lookup"><span data-stu-id="57ec8-123">Name</span></span>       | <span data-ttu-id="57ec8-124">类型</span><span class="sxs-lookup"><span data-stu-id="57ec8-124">Type</span></span> | <span data-ttu-id="57ec8-125">说明</span><span class="sxs-lookup"><span data-stu-id="57ec8-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="57ec8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="57ec8-126">Authorization</span></span>  | <span data-ttu-id="57ec8-127">string</span><span class="sxs-lookup"><span data-stu-id="57ec8-127">string</span></span>  | <span data-ttu-id="57ec8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57ec8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57ec8-130">接受</span><span class="sxs-lookup"><span data-stu-id="57ec8-130">Accept</span></span> | <span data-ttu-id="57ec8-131">string</span><span class="sxs-lookup"><span data-stu-id="57ec8-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="57ec8-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="57ec8-132">Request body</span></span>
<span data-ttu-id="57ec8-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="57ec8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57ec8-134">响应</span><span class="sxs-lookup"><span data-stu-id="57ec8-134">Response</span></span>

<span data-ttu-id="57ec8-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57ec8-135">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57ec8-136">示例</span><span class="sxs-lookup"><span data-stu-id="57ec8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57ec8-137">请求</span><span class="sxs-lookup"><span data-stu-id="57ec8-137">Request</span></span>
<span data-ttu-id="57ec8-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57ec8-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57ec8-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="57ec8-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="57ec8-140">C#</span><span class="sxs-lookup"><span data-stu-id="57ec8-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57ec8-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57ec8-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57ec8-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57ec8-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57ec8-143">Java</span><span class="sxs-lookup"><span data-stu-id="57ec8-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="57ec8-144">响应</span><span class="sxs-lookup"><span data-stu-id="57ec8-144">Response</span></span>
<span data-ttu-id="57ec8-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57ec8-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
