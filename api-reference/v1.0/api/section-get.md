---
title: 获取分区
description: 检索的属性和 onenoteSection 对象的关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d491e0936096296c731e2ebbbc1d6d44dccdef38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941553"
---
# <a name="get-section"></a><span data-ttu-id="9862d-103">获取分区</span><span class="sxs-lookup"><span data-stu-id="9862d-103">Get section</span></span>

<span data-ttu-id="9862d-104">检索的属性和[onenoteSection](../resources/section.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9862d-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9862d-105">权限</span><span class="sxs-lookup"><span data-stu-id="9862d-105">Permissions</span></span>
<span data-ttu-id="9862d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9862d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9862d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9862d-108">Permission type</span></span>      | <span data-ttu-id="9862d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9862d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9862d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9862d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9862d-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9862d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9862d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9862d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9862d-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9862d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9862d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9862d-114">Application</span></span> | <span data-ttu-id="9862d-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9862d-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9862d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9862d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9862d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9862d-117">Optional query parameters</span></span>
<span data-ttu-id="9862d-118">此方法支持 `select` 和 `expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9862d-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9862d-p102">默认查询展开 `parentNotebook`，并选择其 `id`、`displayName` 和 `self` 属性。分区的有效 `expand` 值为 `parentNotebook` 和 `parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="9862d-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9862d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9862d-121">Request headers</span></span>
| <span data-ttu-id="9862d-122">名称</span><span class="sxs-lookup"><span data-stu-id="9862d-122">Name</span></span>       | <span data-ttu-id="9862d-123">类型</span><span class="sxs-lookup"><span data-stu-id="9862d-123">Type</span></span> | <span data-ttu-id="9862d-124">说明</span><span class="sxs-lookup"><span data-stu-id="9862d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9862d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9862d-125">Authorization</span></span>  | <span data-ttu-id="9862d-126">string</span><span class="sxs-lookup"><span data-stu-id="9862d-126">string</span></span>  | <span data-ttu-id="9862d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9862d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9862d-129">Accept</span><span class="sxs-lookup"><span data-stu-id="9862d-129">Accept</span></span> | <span data-ttu-id="9862d-130">string</span><span class="sxs-lookup"><span data-stu-id="9862d-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9862d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9862d-131">Request body</span></span>
<span data-ttu-id="9862d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9862d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9862d-133">响应</span><span class="sxs-lookup"><span data-stu-id="9862d-133">Response</span></span>

<span data-ttu-id="9862d-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[onenoteSection](../resources/section.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9862d-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9862d-135">示例</span><span class="sxs-lookup"><span data-stu-id="9862d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9862d-136">请求</span><span class="sxs-lookup"><span data-stu-id="9862d-136">Request</span></span>
<span data-ttu-id="9862d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9862d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="9862d-138">响应</span><span class="sxs-lookup"><span data-stu-id="9862d-138">Response</span></span>
<span data-ttu-id="9862d-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9862d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
