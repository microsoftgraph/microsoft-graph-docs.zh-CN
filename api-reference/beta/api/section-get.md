---
title: 获取分区
description: 检索 section 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: b9746715d01a51f0a35da3936e64b850020629ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846947"
---
# <a name="get-section"></a><span data-ttu-id="f9581-103">获取分区</span><span class="sxs-lookup"><span data-stu-id="f9581-103">Get section</span></span>

> <span data-ttu-id="f9581-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9581-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9581-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9581-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9581-106">检索 [section](../resources/section.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9581-106">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9581-107">权限</span><span class="sxs-lookup"><span data-stu-id="f9581-107">Permissions</span></span>
<span data-ttu-id="f9581-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9581-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9581-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9581-110">Permission type</span></span>      | <span data-ttu-id="f9581-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9581-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9581-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9581-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9581-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9581-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9581-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9581-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9581-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9581-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f9581-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9581-116">Application</span></span> | <span data-ttu-id="f9581-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9581-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9581-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9581-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9581-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9581-119">Optional query parameters</span></span>
<span data-ttu-id="f9581-120">此方法支持 `select` 和 `expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f9581-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f9581-p103">默认查询展开 `parentNotebook`，并选择其 `id`、`displayName` 和 `self` 属性。分区的有效 `expand` 值为 `parentNotebook` 和 `parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="f9581-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9581-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9581-123">Request headers</span></span>
| <span data-ttu-id="f9581-124">名称</span><span class="sxs-lookup"><span data-stu-id="f9581-124">Name</span></span>       | <span data-ttu-id="f9581-125">类型</span><span class="sxs-lookup"><span data-stu-id="f9581-125">Type</span></span> | <span data-ttu-id="f9581-126">说明</span><span class="sxs-lookup"><span data-stu-id="f9581-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9581-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9581-127">Authorization</span></span>  | <span data-ttu-id="f9581-128">string</span><span class="sxs-lookup"><span data-stu-id="f9581-128">string</span></span>  | <span data-ttu-id="f9581-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9581-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9581-131">Accept</span><span class="sxs-lookup"><span data-stu-id="f9581-131">Accept</span></span> | <span data-ttu-id="f9581-132">string</span><span class="sxs-lookup"><span data-stu-id="f9581-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f9581-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9581-133">Request body</span></span>
<span data-ttu-id="f9581-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9581-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9581-135">响应</span><span class="sxs-lookup"><span data-stu-id="f9581-135">Response</span></span>

<span data-ttu-id="f9581-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [section](../resources/section.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9581-136">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9581-137">示例</span><span class="sxs-lookup"><span data-stu-id="f9581-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9581-138">请求</span><span class="sxs-lookup"><span data-stu-id="f9581-138">Request</span></span>
<span data-ttu-id="f9581-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9581-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="f9581-140">响应</span><span class="sxs-lookup"><span data-stu-id="f9581-140">Response</span></span>
<span data-ttu-id="f9581-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9581-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
