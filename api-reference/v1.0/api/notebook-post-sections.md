---
title: 创建分区
description: 指定笔记本中创建新 onenoteSection。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: b39ae58dd67e7eaa666845b108632eea4aa3ac57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882283"
---
# <a name="create-section"></a><span data-ttu-id="8bbf0-103">创建分区</span><span class="sxs-lookup"><span data-stu-id="8bbf0-103">Create section</span></span>

<span data-ttu-id="8bbf0-104">指定笔记本中创建新[onenoteSection](../resources/section.md) 。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-104">Create a new [onenoteSection](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bbf0-105">权限</span><span class="sxs-lookup"><span data-stu-id="8bbf0-105">Permissions</span></span>
<span data-ttu-id="8bbf0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bbf0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bbf0-108">Permission type</span></span>      | <span data-ttu-id="8bbf0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bbf0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bbf0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bbf0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bbf0-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bbf0-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bbf0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bbf0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bbf0-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bbf0-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8bbf0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bbf0-114">Application</span></span> | <span data-ttu-id="8bbf0-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bbf0-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bbf0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bbf0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="8bbf0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bbf0-117">Request headers</span></span>
| <span data-ttu-id="8bbf0-118">名称</span><span class="sxs-lookup"><span data-stu-id="8bbf0-118">Name</span></span>       | <span data-ttu-id="8bbf0-119">类型</span><span class="sxs-lookup"><span data-stu-id="8bbf0-119">Type</span></span> | <span data-ttu-id="8bbf0-120">说明</span><span class="sxs-lookup"><span data-stu-id="8bbf0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8bbf0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bbf0-121">Authorization</span></span>  | <span data-ttu-id="8bbf0-122">string</span><span class="sxs-lookup"><span data-stu-id="8bbf0-122">string</span></span>  | <span data-ttu-id="8bbf0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bbf0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bbf0-125">Content-Type</span></span> | <span data-ttu-id="8bbf0-126">string</span><span class="sxs-lookup"><span data-stu-id="8bbf0-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8bbf0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bbf0-127">Request body</span></span>
<span data-ttu-id="8bbf0-128">在请求正文中，提供分区名称。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="8bbf0-p103">在同一个层次结构级别中，分区名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="8bbf0-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="8bbf0-131">响应</span><span class="sxs-lookup"><span data-stu-id="8bbf0-131">Response</span></span>

<span data-ttu-id="8bbf0-132">如果成功，此方法返回`201 Created`响应代码和响应正文中的[onenoteSection](../resources/section.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bbf0-133">示例</span><span class="sxs-lookup"><span data-stu-id="8bbf0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bbf0-134">请求</span><span class="sxs-lookup"><span data-stu-id="8bbf0-134">Request</span></span>
<span data-ttu-id="8bbf0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="8bbf0-136">响应</span><span class="sxs-lookup"><span data-stu-id="8bbf0-136">Response</span></span>
<span data-ttu-id="8bbf0-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bbf0-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
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
