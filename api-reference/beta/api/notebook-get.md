---
title: 获取笔记本
description: 检索 notebook 对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: af8d358a7f05ed60b48e6df6a3cc60319e009e34
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515781"
---
# <a name="get-notebook"></a><span data-ttu-id="a0484-103">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="a0484-103">Get notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0484-104">检索 [notebook](../resources/notebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0484-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0484-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0484-105">Permissions</span></span>
<span data-ttu-id="a0484-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0484-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0484-108">Permission type</span></span>      | <span data-ttu-id="a0484-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0484-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0484-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0484-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0484-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0484-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0484-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0484-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0484-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0484-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a0484-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0484-114">Application</span></span> | <span data-ttu-id="a0484-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0484-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0484-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0484-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0484-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0484-117">Optional query parameters</span></span>
<span data-ttu-id="a0484-118">此方法支持 `select` 和 `expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0484-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a0484-119">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="a0484-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0484-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0484-120">Request headers</span></span>
| <span data-ttu-id="a0484-121">名称</span><span class="sxs-lookup"><span data-stu-id="a0484-121">Name</span></span>       | <span data-ttu-id="a0484-122">类型</span><span class="sxs-lookup"><span data-stu-id="a0484-122">Type</span></span> | <span data-ttu-id="a0484-123">说明</span><span class="sxs-lookup"><span data-stu-id="a0484-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a0484-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0484-124">Authorization</span></span>  | <span data-ttu-id="a0484-125">string</span><span class="sxs-lookup"><span data-stu-id="a0484-125">string</span></span>  | <span data-ttu-id="a0484-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0484-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0484-128">Accept</span><span class="sxs-lookup"><span data-stu-id="a0484-128">Accept</span></span> | <span data-ttu-id="a0484-129">string</span><span class="sxs-lookup"><span data-stu-id="a0484-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a0484-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0484-130">Request body</span></span>
<span data-ttu-id="a0484-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0484-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0484-132">响应</span><span class="sxs-lookup"><span data-stu-id="a0484-132">Response</span></span>

<span data-ttu-id="a0484-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0484-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0484-134">示例</span><span class="sxs-lookup"><span data-stu-id="a0484-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0484-135">请求</span><span class="sxs-lookup"><span data-stu-id="a0484-135">Request</span></span>
<span data-ttu-id="a0484-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0484-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="a0484-137">响应</span><span class="sxs-lookup"><span data-stu-id="a0484-137">Response</span></span>
<span data-ttu-id="a0484-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0484-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
