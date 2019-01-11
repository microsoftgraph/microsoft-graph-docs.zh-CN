---
title: 获取笔记本
description: 检索 notebook 对象的属性和关系。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7193e7ac0e94c15c467c0d9c49d41fb73eff324b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838575"
---
# <a name="get-notebook"></a><span data-ttu-id="27897-103">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="27897-103">Get notebook</span></span>

> <span data-ttu-id="27897-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27897-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27897-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27897-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27897-106">检索 [notebook](../resources/notebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27897-106">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27897-107">权限</span><span class="sxs-lookup"><span data-stu-id="27897-107">Permissions</span></span>
<span data-ttu-id="27897-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27897-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27897-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27897-110">Permission type</span></span>      | <span data-ttu-id="27897-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27897-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27897-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27897-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27897-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27897-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="27897-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27897-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27897-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27897-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="27897-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="27897-116">Application</span></span> | <span data-ttu-id="27897-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27897-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27897-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27897-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27897-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="27897-119">Optional query parameters</span></span>
<span data-ttu-id="27897-120">此方法支持 `select` 和 `expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="27897-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="27897-121">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="27897-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27897-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="27897-122">Request headers</span></span>
| <span data-ttu-id="27897-123">名称</span><span class="sxs-lookup"><span data-stu-id="27897-123">Name</span></span>       | <span data-ttu-id="27897-124">类型</span><span class="sxs-lookup"><span data-stu-id="27897-124">Type</span></span> | <span data-ttu-id="27897-125">说明</span><span class="sxs-lookup"><span data-stu-id="27897-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="27897-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="27897-126">Authorization</span></span>  | <span data-ttu-id="27897-127">string</span><span class="sxs-lookup"><span data-stu-id="27897-127">string</span></span>  | <span data-ttu-id="27897-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27897-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27897-130">Accept</span><span class="sxs-lookup"><span data-stu-id="27897-130">Accept</span></span> | <span data-ttu-id="27897-131">string</span><span class="sxs-lookup"><span data-stu-id="27897-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="27897-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="27897-132">Request body</span></span>
<span data-ttu-id="27897-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27897-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27897-134">响应</span><span class="sxs-lookup"><span data-stu-id="27897-134">Response</span></span>

<span data-ttu-id="27897-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27897-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27897-136">示例</span><span class="sxs-lookup"><span data-stu-id="27897-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27897-137">请求</span><span class="sxs-lookup"><span data-stu-id="27897-137">Request</span></span>
<span data-ttu-id="27897-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27897-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="27897-139">响应</span><span class="sxs-lookup"><span data-stu-id="27897-139">Response</span></span>
<span data-ttu-id="27897-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27897-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
