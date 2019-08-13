---
title: 列出 sectionGroups
description: 从指定分区组中检索分区组列表。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b060125d06553b7c7d4d7f2d2e7ab05130a0547c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320042"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="ca473-103">列出 sectionGroups</span><span class="sxs-lookup"><span data-stu-id="ca473-103">List sectionGroups</span></span>

<span data-ttu-id="ca473-104">从指定分区组中检索[分区组](../resources/sectiongroup.md)列表。</span><span class="sxs-lookup"><span data-stu-id="ca473-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca473-105">权限</span><span class="sxs-lookup"><span data-stu-id="ca473-105">Permissions</span></span>
<span data-ttu-id="ca473-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca473-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca473-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca473-108">Permission type</span></span>      | <span data-ttu-id="ca473-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca473-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca473-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca473-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ca473-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca473-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca473-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca473-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca473-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca473-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ca473-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca473-114">Application</span></span> | <span data-ttu-id="ca473-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca473-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca473-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca473-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca473-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ca473-117">Optional query parameters</span></span>
<span data-ttu-id="ca473-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca473-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ca473-119">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="ca473-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="ca473-120">默认查询将展开`parentNotebook`并选择其`id`、 `displayName`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="ca473-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="ca473-121">节`expand`组`sections`的有效值为`sectionGroups`、 `parentNotebook`、和。 `parentSectionGroup`</span><span class="sxs-lookup"><span data-stu-id="ca473-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca473-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca473-122">Request headers</span></span>
| <span data-ttu-id="ca473-123">名称</span><span class="sxs-lookup"><span data-stu-id="ca473-123">Name</span></span>       | <span data-ttu-id="ca473-124">类型</span><span class="sxs-lookup"><span data-stu-id="ca473-124">Type</span></span> | <span data-ttu-id="ca473-125">说明</span><span class="sxs-lookup"><span data-stu-id="ca473-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca473-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca473-126">Authorization</span></span>  | <span data-ttu-id="ca473-127">string</span><span class="sxs-lookup"><span data-stu-id="ca473-127">string</span></span>  | <span data-ttu-id="ca473-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca473-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca473-130">接受</span><span class="sxs-lookup"><span data-stu-id="ca473-130">Accept</span></span> | <span data-ttu-id="ca473-131">string</span><span class="sxs-lookup"><span data-stu-id="ca473-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ca473-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca473-132">Request body</span></span>
<span data-ttu-id="ca473-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca473-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca473-134">响应</span><span class="sxs-lookup"><span data-stu-id="ca473-134">Response</span></span>

<span data-ttu-id="ca473-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[sectionGroup](../resources/sectiongroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ca473-135">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca473-136">示例</span><span class="sxs-lookup"><span data-stu-id="ca473-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca473-137">请求</span><span class="sxs-lookup"><span data-stu-id="ca473-137">Request</span></span>
<span data-ttu-id="ca473-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca473-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ca473-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ca473-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca473-140">C#</span><span class="sxs-lookup"><span data-stu-id="ca473-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca473-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca473-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca473-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="ca473-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ca473-143">Java</span><span class="sxs-lookup"><span data-stu-id="ca473-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sectiongroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca473-144">响应</span><span class="sxs-lookup"><span data-stu-id="ca473-144">Response</span></span>
<span data-ttu-id="ca473-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca473-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
