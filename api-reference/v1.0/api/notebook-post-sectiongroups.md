---
title: 创建 sectionGroup
description: 在指定的笔记本中新建分区组。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 03234624efc5dd2ada63fb7b7b54c2760190a03d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511339"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="1bba2-103">创建 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="1bba2-103">Create sectionGroup</span></span>

<span data-ttu-id="1bba2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bba2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bba2-105">在指定的笔记本中新建[分区组](../resources/sectiongroup.md)。</span><span class="sxs-lookup"><span data-stu-id="1bba2-105">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="1bba2-106">权限</span><span class="sxs-lookup"><span data-stu-id="1bba2-106">Permissions</span></span>
<span data-ttu-id="1bba2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bba2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bba2-109">Permission type</span></span>      | <span data-ttu-id="1bba2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bba2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bba2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bba2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1bba2-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bba2-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1bba2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bba2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bba2-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bba2-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1bba2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bba2-115">Application</span></span> | <span data-ttu-id="1bba2-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bba2-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bba2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bba2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="1bba2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bba2-118">Request headers</span></span>
| <span data-ttu-id="1bba2-119">名称</span><span class="sxs-lookup"><span data-stu-id="1bba2-119">Name</span></span>       | <span data-ttu-id="1bba2-120">类型</span><span class="sxs-lookup"><span data-stu-id="1bba2-120">Type</span></span> | <span data-ttu-id="1bba2-121">说明</span><span class="sxs-lookup"><span data-stu-id="1bba2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bba2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bba2-122">Authorization</span></span>  | <span data-ttu-id="1bba2-123">string</span><span class="sxs-lookup"><span data-stu-id="1bba2-123">string</span></span>  | <span data-ttu-id="1bba2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bba2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1bba2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bba2-126">Content-Type</span></span> | <span data-ttu-id="1bba2-127">string</span><span class="sxs-lookup"><span data-stu-id="1bba2-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1bba2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bba2-128">Request body</span></span>
<span data-ttu-id="1bba2-129">在请求正文中，提供分区组名称。</span><span class="sxs-lookup"><span data-stu-id="1bba2-129">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="1bba2-p103">在同一个层次结构级别中，分区组名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="1bba2-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="1bba2-132">响应</span><span class="sxs-lookup"><span data-stu-id="1bba2-132">Response</span></span>

<span data-ttu-id="1bba2-133">如果成功，此方法在`201 Created`响应正文中返回响应代码和[sectionGroup](../resources/sectiongroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1bba2-133">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bba2-134">示例</span><span class="sxs-lookup"><span data-stu-id="1bba2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bba2-135">请求</span><span class="sxs-lookup"><span data-stu-id="1bba2-135">Request</span></span>
<span data-ttu-id="1bba2-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bba2-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bba2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bba2-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1bba2-138">C#</span><span class="sxs-lookup"><span data-stu-id="1bba2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bba2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bba2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bba2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bba2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bba2-141">Java</span><span class="sxs-lookup"><span data-stu-id="1bba2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1bba2-142">响应</span><span class="sxs-lookup"><span data-stu-id="1bba2-142">Response</span></span>
<span data-ttu-id="1bba2-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bba2-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
