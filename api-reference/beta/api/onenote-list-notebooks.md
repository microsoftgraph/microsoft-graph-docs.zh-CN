---
title: 列出笔记本
description: 检索 notebook 对象列表。
ms.openlocfilehash: 0f9bf502973be0d178db70e42f25a0716263e323
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043719"
---
# <a name="list-notebooks"></a><span data-ttu-id="f41a3-103">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="f41a3-103">List notebooks</span></span>

> <span data-ttu-id="f41a3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f41a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f41a3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f41a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f41a3-106">检索 [notebook](../resources/notebook.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="f41a3-106">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f41a3-107">权限</span><span class="sxs-lookup"><span data-stu-id="f41a3-107">Permissions</span></span>
<span data-ttu-id="f41a3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f41a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f41a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f41a3-110">Permission type</span></span>      | <span data-ttu-id="f41a3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f41a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f41a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f41a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f41a3-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f41a3-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f41a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f41a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f41a3-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f41a3-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f41a3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f41a3-116">Application</span></span> | <span data-ttu-id="f41a3-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f41a3-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f41a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f41a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f41a3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f41a3-119">Optional query parameters</span></span>
<span data-ttu-id="f41a3-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f41a3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f41a3-121">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="f41a3-121">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="f41a3-122">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="f41a3-122">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f41a3-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f41a3-123">Request headers</span></span>
| <span data-ttu-id="f41a3-124">名称</span><span class="sxs-lookup"><span data-stu-id="f41a3-124">Name</span></span>       | <span data-ttu-id="f41a3-125">类型</span><span class="sxs-lookup"><span data-stu-id="f41a3-125">Type</span></span> | <span data-ttu-id="f41a3-126">说明</span><span class="sxs-lookup"><span data-stu-id="f41a3-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f41a3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f41a3-127">Authorization</span></span>  | <span data-ttu-id="f41a3-128">string</span><span class="sxs-lookup"><span data-stu-id="f41a3-128">string</span></span>  | <span data-ttu-id="f41a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f41a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f41a3-131">Accept</span><span class="sxs-lookup"><span data-stu-id="f41a3-131">Accept</span></span> | <span data-ttu-id="f41a3-132">string</span><span class="sxs-lookup"><span data-stu-id="f41a3-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f41a3-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f41a3-133">Request body</span></span>
<span data-ttu-id="f41a3-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f41a3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f41a3-135">响应</span><span class="sxs-lookup"><span data-stu-id="f41a3-135">Response</span></span>

<span data-ttu-id="f41a3-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f41a3-136">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f41a3-137">示例</span><span class="sxs-lookup"><span data-stu-id="f41a3-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f41a3-138">请求</span><span class="sxs-lookup"><span data-stu-id="f41a3-138">Request</span></span>
<span data-ttu-id="f41a3-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f41a3-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="f41a3-140">响应</span><span class="sxs-lookup"><span data-stu-id="f41a3-140">Response</span></span>
<span data-ttu-id="f41a3-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f41a3-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->