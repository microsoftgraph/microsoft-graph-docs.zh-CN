---
title: 列出 sectionGroups
description: 从指定笔记本中检索分区组列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 1f692103c1114b4976ffec4c77c719b3768a368a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028530"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="7f87c-103">列出 sectionGroups</span><span class="sxs-lookup"><span data-stu-id="7f87c-103">List sectionGroups</span></span>

<span data-ttu-id="7f87c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f87c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f87c-105">从指定笔记本中检索 [分区组](../resources/sectiongroup.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="7f87c-105">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f87c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f87c-106">Permissions</span></span>
<span data-ttu-id="7f87c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f87c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f87c-109">Permission type</span></span>      | <span data-ttu-id="7f87c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f87c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f87c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f87c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f87c-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f87c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f87c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f87c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f87c-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f87c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7f87c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f87c-115">Application</span></span> | <span data-ttu-id="7f87c-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f87c-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f87c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f87c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f87c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f87c-118">Optional query parameters</span></span>
<span data-ttu-id="7f87c-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f87c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7f87c-120">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="7f87c-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="7f87c-121">默认查询将展开 `parentNotebook` 并选择其 `id` 、 `displayName` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="7f87c-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="7f87c-122">`expand`节组的有效值为 `sections` 、、 `sectionGroups` `parentNotebook` 和 `parentSectionGroup` 。</span><span class="sxs-lookup"><span data-stu-id="7f87c-122">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f87c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f87c-123">Request headers</span></span>
| <span data-ttu-id="7f87c-124">名称</span><span class="sxs-lookup"><span data-stu-id="7f87c-124">Name</span></span>       | <span data-ttu-id="7f87c-125">类型</span><span class="sxs-lookup"><span data-stu-id="7f87c-125">Type</span></span> | <span data-ttu-id="7f87c-126">说明</span><span class="sxs-lookup"><span data-stu-id="7f87c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f87c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f87c-127">Authorization</span></span>  | <span data-ttu-id="7f87c-128">string</span><span class="sxs-lookup"><span data-stu-id="7f87c-128">string</span></span>  | <span data-ttu-id="7f87c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f87c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f87c-131">接受</span><span class="sxs-lookup"><span data-stu-id="7f87c-131">Accept</span></span> | <span data-ttu-id="7f87c-132">string</span><span class="sxs-lookup"><span data-stu-id="7f87c-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7f87c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f87c-133">Request body</span></span>
<span data-ttu-id="7f87c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f87c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f87c-135">响应</span><span class="sxs-lookup"><span data-stu-id="7f87c-135">Response</span></span>

<span data-ttu-id="7f87c-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7f87c-136">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f87c-137">示例</span><span class="sxs-lookup"><span data-stu-id="7f87c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f87c-138">请求</span><span class="sxs-lookup"><span data-stu-id="7f87c-138">Request</span></span>
<span data-ttu-id="7f87c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f87c-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f87c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f87c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sectiongroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
# <a name="c"></a>[<span data-ttu-id="7f87c-141">C#</span><span class="sxs-lookup"><span data-stu-id="7f87c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f87c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f87c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f87c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f87c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f87c-144">Java</span><span class="sxs-lookup"><span data-stu-id="7f87c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-get-sectiongroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f87c-145">响应</span><span class="sxs-lookup"><span data-stu-id="7f87c-145">Response</span></span>
<span data-ttu-id="7f87c-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f87c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

