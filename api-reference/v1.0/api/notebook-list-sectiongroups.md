---
title: 列出 sectionGroups
description: 从指定笔记本中检索分区组列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e24c0d9fb59c05b02d36402a2d181db0c696e3c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562179"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="bccac-103">列出 sectionGroups</span><span class="sxs-lookup"><span data-stu-id="bccac-103">List sectionGroups</span></span>

<span data-ttu-id="bccac-104">从指定笔记本中检索[分区组](../resources/sectiongroup.md)列表。</span><span class="sxs-lookup"><span data-stu-id="bccac-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="bccac-105">权限</span><span class="sxs-lookup"><span data-stu-id="bccac-105">Permissions</span></span>
<span data-ttu-id="bccac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bccac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bccac-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bccac-108">Permission type</span></span>      | <span data-ttu-id="bccac-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bccac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bccac-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bccac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bccac-111">注意: Create、notes、read、read. all、all、all</span><span class="sxs-lookup"><span data-stu-id="bccac-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bccac-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bccac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bccac-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bccac-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bccac-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bccac-114">Application</span></span> | <span data-ttu-id="bccac-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bccac-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bccac-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bccac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bccac-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bccac-117">Optional query parameters</span></span>
<span data-ttu-id="bccac-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bccac-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bccac-119">默认排序顺序为`name asc`。</span><span class="sxs-lookup"><span data-stu-id="bccac-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="bccac-120">默认查询将展开`parentNotebook`并选择其`id`、 `displayName`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="bccac-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="bccac-121">节`expand`组`sections`的有效值为`sectionGroups`、 `parentNotebook`、和。 `parentSectionGroup`</span><span class="sxs-lookup"><span data-stu-id="bccac-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bccac-122">请求头</span><span class="sxs-lookup"><span data-stu-id="bccac-122">Request headers</span></span>
| <span data-ttu-id="bccac-123">名称</span><span class="sxs-lookup"><span data-stu-id="bccac-123">Name</span></span>       | <span data-ttu-id="bccac-124">类型</span><span class="sxs-lookup"><span data-stu-id="bccac-124">Type</span></span> | <span data-ttu-id="bccac-125">说明</span><span class="sxs-lookup"><span data-stu-id="bccac-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bccac-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bccac-126">Authorization</span></span>  | <span data-ttu-id="bccac-127">string</span><span class="sxs-lookup"><span data-stu-id="bccac-127">string</span></span>  | <span data-ttu-id="bccac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bccac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bccac-130">接受</span><span class="sxs-lookup"><span data-stu-id="bccac-130">Accept</span></span> | <span data-ttu-id="bccac-131">string</span><span class="sxs-lookup"><span data-stu-id="bccac-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bccac-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="bccac-132">Request body</span></span>
<span data-ttu-id="bccac-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bccac-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bccac-134">响应</span><span class="sxs-lookup"><span data-stu-id="bccac-134">Response</span></span>

<span data-ttu-id="bccac-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[sectionGroup](../resources/sectiongroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="bccac-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bccac-136">示例</span><span class="sxs-lookup"><span data-stu-id="bccac-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bccac-137">请求</span><span class="sxs-lookup"><span data-stu-id="bccac-137">Request</span></span>
<span data-ttu-id="bccac-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bccac-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="bccac-139">响应</span><span class="sxs-lookup"><span data-stu-id="bccac-139">Response</span></span>
<span data-ttu-id="bccac-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bccac-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
