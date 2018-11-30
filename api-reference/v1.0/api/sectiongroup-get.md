---
title: 获取 sectionGroup
description: 检索 sectionGroup 对象的属性和关系。
ms.openlocfilehash: 080e9390153a8af36e25bb823bbe8560953d1c19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009437"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="e13c6-103">获取 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="e13c6-103">Get sectionGroup</span></span>

<span data-ttu-id="e13c6-104">检索 [sectionGroup](../resources/sectiongroup.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e13c6-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e13c6-105">权限</span><span class="sxs-lookup"><span data-stu-id="e13c6-105">Permissions</span></span>
<span data-ttu-id="e13c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e13c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e13c6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e13c6-108">Permission type</span></span>      | <span data-ttu-id="e13c6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e13c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e13c6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e13c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e13c6-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e13c6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e13c6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e13c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13c6-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e13c6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e13c6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e13c6-114">Application</span></span> | <span data-ttu-id="e13c6-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e13c6-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e13c6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e13c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e13c6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e13c6-117">Optional query parameters</span></span>
<span data-ttu-id="e13c6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e13c6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e13c6-p102">默认查询展开 `parentNotebook`，并选择其 `id`、`name` 和 `self` 属性。分区组的有效 `expand` 值为 `parentNotebook` 和`parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="e13c6-p102">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e13c6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e13c6-121">Request headers</span></span>
| <span data-ttu-id="e13c6-122">名称</span><span class="sxs-lookup"><span data-stu-id="e13c6-122">Name</span></span>       | <span data-ttu-id="e13c6-123">类型</span><span class="sxs-lookup"><span data-stu-id="e13c6-123">Type</span></span> | <span data-ttu-id="e13c6-124">说明</span><span class="sxs-lookup"><span data-stu-id="e13c6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e13c6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e13c6-125">Authorization</span></span>  | <span data-ttu-id="e13c6-126">string</span><span class="sxs-lookup"><span data-stu-id="e13c6-126">string</span></span>  | <span data-ttu-id="e13c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e13c6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e13c6-129">Accept</span><span class="sxs-lookup"><span data-stu-id="e13c6-129">Accept</span></span> | <span data-ttu-id="e13c6-130">string</span><span class="sxs-lookup"><span data-stu-id="e13c6-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e13c6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e13c6-131">Request body</span></span>
<span data-ttu-id="e13c6-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e13c6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13c6-133">响应</span><span class="sxs-lookup"><span data-stu-id="e13c6-133">Response</span></span>

<span data-ttu-id="e13c6-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e13c6-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e13c6-135">示例</span><span class="sxs-lookup"><span data-stu-id="e13c6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e13c6-136">请求</span><span class="sxs-lookup"><span data-stu-id="e13c6-136">Request</span></span>
<span data-ttu-id="e13c6-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e13c6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="e13c6-138">响应</span><span class="sxs-lookup"><span data-stu-id="e13c6-138">Response</span></span>
<span data-ttu-id="e13c6-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e13c6-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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