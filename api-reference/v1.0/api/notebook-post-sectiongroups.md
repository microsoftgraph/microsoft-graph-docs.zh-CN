---
title: 创建 sectionGroup
description: 在指定的笔记本中新建分区组。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 50eae841aafc3e6ed296f2e596755a602331346f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374454"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="3f7fc-103">创建 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="3f7fc-103">Create sectionGroup</span></span>

<span data-ttu-id="3f7fc-104">在指定的笔记本中新建[分区组](../resources/sectiongroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-104">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f7fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="3f7fc-105">Permissions</span></span>
<span data-ttu-id="3f7fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f7fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f7fc-108">Permission type</span></span>      | <span data-ttu-id="3f7fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f7fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f7fc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f7fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f7fc-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f7fc-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f7fc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f7fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f7fc-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f7fc-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3f7fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f7fc-114">Application</span></span> | <span data-ttu-id="3f7fc-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f7fc-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f7fc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f7fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="3f7fc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f7fc-117">Request headers</span></span>
| <span data-ttu-id="3f7fc-118">名称</span><span class="sxs-lookup"><span data-stu-id="3f7fc-118">Name</span></span>       | <span data-ttu-id="3f7fc-119">类型</span><span class="sxs-lookup"><span data-stu-id="3f7fc-119">Type</span></span> | <span data-ttu-id="3f7fc-120">说明</span><span class="sxs-lookup"><span data-stu-id="3f7fc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3f7fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f7fc-121">Authorization</span></span>  | <span data-ttu-id="3f7fc-122">string</span><span class="sxs-lookup"><span data-stu-id="3f7fc-122">string</span></span>  | <span data-ttu-id="3f7fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f7fc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f7fc-125">Content-Type</span></span> | <span data-ttu-id="3f7fc-126">string</span><span class="sxs-lookup"><span data-stu-id="3f7fc-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3f7fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f7fc-127">Request body</span></span>
<span data-ttu-id="3f7fc-128">在请求正文中，提供分区组名称。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="3f7fc-p103">在同一个层次结构级别中，分区组名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="3f7fc-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="3f7fc-131">响应</span><span class="sxs-lookup"><span data-stu-id="3f7fc-131">Response</span></span>

<span data-ttu-id="3f7fc-132">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[sectionGroup](../resources/sectiongroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-132">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f7fc-133">示例</span><span class="sxs-lookup"><span data-stu-id="3f7fc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f7fc-134">请求</span><span class="sxs-lookup"><span data-stu-id="3f7fc-134">Request</span></span>
<span data-ttu-id="3f7fc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f7fc-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3f7fc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f7fc-137">C#</span><span class="sxs-lookup"><span data-stu-id="3f7fc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f7fc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f7fc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f7fc-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="3f7fc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3f7fc-140">Java</span><span class="sxs-lookup"><span data-stu-id="3f7fc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f7fc-141">响应</span><span class="sxs-lookup"><span data-stu-id="3f7fc-141">Response</span></span>
<span data-ttu-id="3f7fc-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f7fc-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
