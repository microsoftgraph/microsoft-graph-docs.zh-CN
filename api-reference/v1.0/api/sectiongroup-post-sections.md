---
title: 创建分区
description: 在指定的节组中创建新 onenoteSection。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 91ed02c363de0fc39af594e2e0932e4c4ad605bf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947076"
---
# <a name="create-section"></a><span data-ttu-id="0bd64-103">创建分区</span><span class="sxs-lookup"><span data-stu-id="0bd64-103">Create section</span></span>

<span data-ttu-id="0bd64-104">在指定的节组中创建新[onenoteSection](../resources/section.md) 。</span><span class="sxs-lookup"><span data-stu-id="0bd64-104">Create a new [onenoteSection](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="0bd64-105">权限</span><span class="sxs-lookup"><span data-stu-id="0bd64-105">Permissions</span></span>
<span data-ttu-id="0bd64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bd64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bd64-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bd64-108">Permission type</span></span>      | <span data-ttu-id="0bd64-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bd64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bd64-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bd64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0bd64-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bd64-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0bd64-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bd64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bd64-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bd64-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0bd64-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bd64-114">Application</span></span> | <span data-ttu-id="0bd64-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bd64-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bd64-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bd64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="0bd64-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bd64-117">Request headers</span></span>
| <span data-ttu-id="0bd64-118">名称</span><span class="sxs-lookup"><span data-stu-id="0bd64-118">Name</span></span>       | <span data-ttu-id="0bd64-119">类型</span><span class="sxs-lookup"><span data-stu-id="0bd64-119">Type</span></span> | <span data-ttu-id="0bd64-120">说明</span><span class="sxs-lookup"><span data-stu-id="0bd64-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0bd64-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bd64-121">Authorization</span></span>  | <span data-ttu-id="0bd64-122">string</span><span class="sxs-lookup"><span data-stu-id="0bd64-122">string</span></span>  | <span data-ttu-id="0bd64-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0bd64-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bd64-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bd64-125">Content-Type</span></span> | <span data-ttu-id="0bd64-126">string</span><span class="sxs-lookup"><span data-stu-id="0bd64-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0bd64-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bd64-127">Request body</span></span>
<span data-ttu-id="0bd64-128">在请求正文中，提供分区名称。</span><span class="sxs-lookup"><span data-stu-id="0bd64-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="0bd64-p103">在同一个层次结构级别中，分区名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="0bd64-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="0bd64-131">响应</span><span class="sxs-lookup"><span data-stu-id="0bd64-131">Response</span></span>

<span data-ttu-id="0bd64-132">如果成功，此方法返回`201 Created`响应代码和响应正文中的[onenoteSection](../resources/section.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0bd64-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd64-133">示例</span><span class="sxs-lookup"><span data-stu-id="0bd64-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bd64-134">请求</span><span class="sxs-lookup"><span data-stu-id="0bd64-134">Request</span></span>
<span data-ttu-id="0bd64-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bd64-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="0bd64-136">响应</span><span class="sxs-lookup"><span data-stu-id="0bd64-136">Response</span></span>
<span data-ttu-id="0bd64-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bd64-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
