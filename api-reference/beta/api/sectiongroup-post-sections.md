---
title: 创建分区
description: 在指定的分区组中新建分区。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8d65b742ad68de5cdf95f68b2a3eea1ede7f89aa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266953"
---
# <a name="create-section"></a><span data-ttu-id="82f7d-103">创建分区</span><span class="sxs-lookup"><span data-stu-id="82f7d-103">Create section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82f7d-104">在指定的分区组中新建[分区](../resources/onenotesection.md)。</span><span class="sxs-lookup"><span data-stu-id="82f7d-104">Create a new [section](../resources/onenotesection.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="82f7d-105">权限</span><span class="sxs-lookup"><span data-stu-id="82f7d-105">Permissions</span></span>
<span data-ttu-id="82f7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82f7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f7d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="82f7d-108">Permission type</span></span>      | <span data-ttu-id="82f7d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82f7d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82f7d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82f7d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82f7d-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f7d-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="82f7d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82f7d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82f7d-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82f7d-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="82f7d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="82f7d-114">Application</span></span> | <span data-ttu-id="82f7d-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f7d-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82f7d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82f7d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="82f7d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="82f7d-117">Request headers</span></span>
| <span data-ttu-id="82f7d-118">名称</span><span class="sxs-lookup"><span data-stu-id="82f7d-118">Name</span></span>       | <span data-ttu-id="82f7d-119">类型</span><span class="sxs-lookup"><span data-stu-id="82f7d-119">Type</span></span> | <span data-ttu-id="82f7d-120">说明</span><span class="sxs-lookup"><span data-stu-id="82f7d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82f7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82f7d-121">Authorization</span></span>  | <span data-ttu-id="82f7d-122">string</span><span class="sxs-lookup"><span data-stu-id="82f7d-122">string</span></span>  | <span data-ttu-id="82f7d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82f7d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82f7d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82f7d-125">Content-Type</span></span> | <span data-ttu-id="82f7d-126">string</span><span class="sxs-lookup"><span data-stu-id="82f7d-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="82f7d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="82f7d-127">Request body</span></span>
<span data-ttu-id="82f7d-128">在请求正文中，提供分区名称。</span><span class="sxs-lookup"><span data-stu-id="82f7d-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="82f7d-p103">在同一个层次结构级别中，分区名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="82f7d-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="82f7d-131">响应</span><span class="sxs-lookup"><span data-stu-id="82f7d-131">Response</span></span>

<span data-ttu-id="82f7d-132">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[onenoteSection](../resources/onenotesection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82f7d-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82f7d-133">示例</span><span class="sxs-lookup"><span data-stu-id="82f7d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82f7d-134">请求</span><span class="sxs-lookup"><span data-stu-id="82f7d-134">Request</span></span>
<span data-ttu-id="82f7d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82f7d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="82f7d-136">响应</span><span class="sxs-lookup"><span data-stu-id="82f7d-136">Response</span></span>
<span data-ttu-id="82f7d-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82f7d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="82f7d-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="82f7d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82f7d-141">C#</span><span class="sxs-lookup"><span data-stu-id="82f7d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_section_from_sectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82f7d-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="82f7d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_section_from_sectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="82f7d-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="82f7d-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_section_from_sectiongroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-post-sections.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/sectiongroup-post-sections.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/sectiongroup-post-sections.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
