---
title: 获取 sectionGroup
description: 检索 sectionGroup 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: b574c1a0cdfe8b615e24a7cf44a438c3eec139d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871755"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="820d3-103">获取 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="820d3-103">Get sectionGroup</span></span>

<span data-ttu-id="820d3-104">检索 [sectionGroup](../resources/sectiongroup.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="820d3-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="820d3-105">权限</span><span class="sxs-lookup"><span data-stu-id="820d3-105">Permissions</span></span>
<span data-ttu-id="820d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="820d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="820d3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="820d3-108">Permission type</span></span>      | <span data-ttu-id="820d3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="820d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="820d3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="820d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="820d3-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820d3-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="820d3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="820d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="820d3-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="820d3-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="820d3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="820d3-114">Application</span></span> | <span data-ttu-id="820d3-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820d3-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="820d3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="820d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="820d3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="820d3-117">Optional query parameters</span></span>
<span data-ttu-id="820d3-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="820d3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="820d3-p102">默认查询展开 `parentNotebook`，并选择其 `id`、`name` 和 `self` 属性。分区组的有效 `expand` 值为 `parentNotebook` 和`parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="820d3-p102">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="820d3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="820d3-121">Request headers</span></span>
| <span data-ttu-id="820d3-122">名称</span><span class="sxs-lookup"><span data-stu-id="820d3-122">Name</span></span>       | <span data-ttu-id="820d3-123">类型</span><span class="sxs-lookup"><span data-stu-id="820d3-123">Type</span></span> | <span data-ttu-id="820d3-124">说明</span><span class="sxs-lookup"><span data-stu-id="820d3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="820d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="820d3-125">Authorization</span></span>  | <span data-ttu-id="820d3-126">string</span><span class="sxs-lookup"><span data-stu-id="820d3-126">string</span></span>  | <span data-ttu-id="820d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="820d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="820d3-129">Accept</span><span class="sxs-lookup"><span data-stu-id="820d3-129">Accept</span></span> | <span data-ttu-id="820d3-130">string</span><span class="sxs-lookup"><span data-stu-id="820d3-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="820d3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="820d3-131">Request body</span></span>
<span data-ttu-id="820d3-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="820d3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="820d3-133">响应</span><span class="sxs-lookup"><span data-stu-id="820d3-133">Response</span></span>

<span data-ttu-id="820d3-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="820d3-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="820d3-135">示例</span><span class="sxs-lookup"><span data-stu-id="820d3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="820d3-136">请求</span><span class="sxs-lookup"><span data-stu-id="820d3-136">Request</span></span>
<span data-ttu-id="820d3-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="820d3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="820d3-138">响应</span><span class="sxs-lookup"><span data-stu-id="820d3-138">Response</span></span>
<span data-ttu-id="820d3-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="820d3-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
