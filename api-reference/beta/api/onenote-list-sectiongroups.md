---
title: 列出 sectionGroups
description: 检索 sectionGroup 对象的列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: aba942fa0712e36bf7e5d9a93bd27ffbff7818b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456563"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="1ac57-103">列出 sectionGroups</span><span class="sxs-lookup"><span data-stu-id="1ac57-103">List sectionGroups</span></span>

<span data-ttu-id="1ac57-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1ac57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ac57-105">检索[sectionGroup](../resources/sectiongroup.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1ac57-105">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ac57-106">权限</span><span class="sxs-lookup"><span data-stu-id="1ac57-106">Permissions</span></span>
<span data-ttu-id="1ac57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ac57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ac57-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ac57-109">Permission type</span></span>      | <span data-ttu-id="1ac57-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ac57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ac57-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ac57-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ac57-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ac57-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ac57-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ac57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ac57-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ac57-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1ac57-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ac57-115">Application</span></span> | <span data-ttu-id="1ac57-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ac57-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ac57-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ac57-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ac57-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ac57-118">Optional query parameters</span></span>
<span data-ttu-id="1ac57-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ac57-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1ac57-120">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="1ac57-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="1ac57-121">默认查询将展开`parentNotebook`并选择其`id`、 `displayName`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="1ac57-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="1ac57-122">节`expand`组`sections`的有效值为`sectionGroups`、 `parentNotebook`、和。 `parentSectionGroup`</span><span class="sxs-lookup"><span data-stu-id="1ac57-122">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ac57-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ac57-123">Request headers</span></span>
| <span data-ttu-id="1ac57-124">名称</span><span class="sxs-lookup"><span data-stu-id="1ac57-124">Name</span></span>       | <span data-ttu-id="1ac57-125">类型</span><span class="sxs-lookup"><span data-stu-id="1ac57-125">Type</span></span> | <span data-ttu-id="1ac57-126">说明</span><span class="sxs-lookup"><span data-stu-id="1ac57-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ac57-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ac57-127">Authorization</span></span>  | <span data-ttu-id="1ac57-128">string</span><span class="sxs-lookup"><span data-stu-id="1ac57-128">string</span></span>  | <span data-ttu-id="1ac57-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ac57-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ac57-131">接受</span><span class="sxs-lookup"><span data-stu-id="1ac57-131">Accept</span></span> | <span data-ttu-id="1ac57-132">string</span><span class="sxs-lookup"><span data-stu-id="1ac57-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1ac57-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ac57-133">Request body</span></span>
<span data-ttu-id="1ac57-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ac57-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ac57-135">响应</span><span class="sxs-lookup"><span data-stu-id="1ac57-135">Response</span></span>

<span data-ttu-id="1ac57-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和[sectionGroup](../resources/sectiongroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ac57-136">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ac57-137">示例</span><span class="sxs-lookup"><span data-stu-id="1ac57-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ac57-138">请求</span><span class="sxs-lookup"><span data-stu-id="1ac57-138">Request</span></span>
<span data-ttu-id="1ac57-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ac57-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ac57-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ac57-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "onenote_get_sectiongroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups
```
# <a name="c"></a>[<span data-ttu-id="1ac57-141">C#</span><span class="sxs-lookup"><span data-stu-id="1ac57-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/onenote-get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ac57-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ac57-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/onenote-get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ac57-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ac57-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/onenote-get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1ac57-144">响应</span><span class="sxs-lookup"><span data-stu-id="1ac57-144">Response</span></span>
<span data-ttu-id="1ac57-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ac57-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
