---
title: 创建 sectionGroup
description: 在指定分区组中新建分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: de952489d8337772dca6b35471eda6bb02cbcbd7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024726"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="1898e-103">创建 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="1898e-103">Create sectionGroup</span></span>

<span data-ttu-id="1898e-104">在指定分区组中新建[分区组](../resources/sectiongroup.md)。</span><span class="sxs-lookup"><span data-stu-id="1898e-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="1898e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1898e-105">Permissions</span></span>
<span data-ttu-id="1898e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1898e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1898e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1898e-108">Permission type</span></span>      | <span data-ttu-id="1898e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1898e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1898e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1898e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1898e-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1898e-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1898e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1898e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1898e-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1898e-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1898e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1898e-114">Application</span></span> | <span data-ttu-id="1898e-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1898e-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1898e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1898e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="1898e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1898e-117">Request headers</span></span>
| <span data-ttu-id="1898e-118">名称</span><span class="sxs-lookup"><span data-stu-id="1898e-118">Name</span></span>       | <span data-ttu-id="1898e-119">类型</span><span class="sxs-lookup"><span data-stu-id="1898e-119">Type</span></span> | <span data-ttu-id="1898e-120">说明</span><span class="sxs-lookup"><span data-stu-id="1898e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1898e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1898e-121">Authorization</span></span>  | <span data-ttu-id="1898e-122">string</span><span class="sxs-lookup"><span data-stu-id="1898e-122">string</span></span>  | <span data-ttu-id="1898e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1898e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1898e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1898e-125">Content-Type</span></span> | <span data-ttu-id="1898e-126">string</span><span class="sxs-lookup"><span data-stu-id="1898e-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1898e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1898e-127">Request body</span></span>
<span data-ttu-id="1898e-128">在请求正文中，提供分区组名称。</span><span class="sxs-lookup"><span data-stu-id="1898e-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="1898e-p103">在同一个层次结构级别中，分区组名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="1898e-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="1898e-131">响应</span><span class="sxs-lookup"><span data-stu-id="1898e-131">Response</span></span>

<span data-ttu-id="1898e-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1898e-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1898e-133">示例</span><span class="sxs-lookup"><span data-stu-id="1898e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1898e-134">请求</span><span class="sxs-lookup"><span data-stu-id="1898e-134">Request</span></span>
<span data-ttu-id="1898e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1898e-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1898e-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1898e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1898e-137">C#</span><span class="sxs-lookup"><span data-stu-id="1898e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1898e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="1898e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1898e-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="1898e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1898e-140">Java</span><span class="sxs-lookup"><span data-stu-id="1898e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1898e-141">响应</span><span class="sxs-lookup"><span data-stu-id="1898e-141">Response</span></span>
<span data-ttu-id="1898e-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1898e-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
